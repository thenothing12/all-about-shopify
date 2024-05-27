<script lang="ts">
	import { Slide } from "@components";
	import { animate, signal } from "@motion";

    let progress = signal(0)

    animate(async () => {
        await progress.to(11000)
    })
</script>

<Slide>
    {$progress.toLocaleString('id', { maximumFractionDigits: 0 })} toko online di Indonesia
</Slide>