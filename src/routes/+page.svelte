<script lang="ts">
    import {base} from "$app/paths"
</script>

<img src="{base}/caovo.png" alt="a dog that looks like an egg" id="caovo-img" />

<style>
    @keyframes rotate {
        0% {
            transform: rotate3d(1,1,1, 0);
        }
        50% {
            transform: rotate3d(1,1,1, 720deg);
        }
        100% {
            transform: rotate3d(1,1,1, 360deg);
        }
    }

    #caovo-img {
        max-height: 60vh;
        animation-name: rotate;
        animation-duration: 3s;
        animation-iteration-count: infinite;
        animation-direction: alternate;
        animation-timing-function: ease-in-out;
    }
    
    #caovo-img:active {
        animation-name: none;
        transform: scale(0.5);
    }
</style>
