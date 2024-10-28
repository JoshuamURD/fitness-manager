<script lang="ts">
import type { Snippet } from "svelte";

interface BasicProps {
    children: Snippet
}

interface ButtonProps extends BasicProps {
    type?: "button" | "submit" | "reset";
    href?: never;
}
interface LinkProps extends BasicProps {
    href: string;
}

type ComponentProps = ButtonProps | LinkProps;

let {children, href, ...props}: ComponentProps = $props();

</script>

{#if href}
<a href={href}>
    {@render children()}
</a>
{:else}

<button {...props} class="btn">
    {@render children()}
</button>
{/if}