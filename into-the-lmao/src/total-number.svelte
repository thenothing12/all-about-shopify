<script lang="ts">
	import { Slide } from "@components";
	import { animate, signal } from "@motion";

    let progress = signal(0)

    animate(async () => {
        await progress.to(5000000)
    })
</script>

<Slide>
    Per Desember 2023, terdapat {$progress.toLocaleString('id', { maximumFractionDigits: 0 })} toko online
</Slide>