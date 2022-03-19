<script>
    import {count} from '../stores/number'

    const add = () => {
        count.update(n => n+1)
    }

    const sub = () => {
        count.update(n => n-1)
    }

    const mult = () => {
        count.update(n => n*2)
    }

    const div = () => {
        count.update(n => n/2)
    }
</script>

<p>{$count}</p>
<button on:click={add}>Add 1</button><br>
<button on:click={sub}>Sub 1</button><br>
<button on:click={mult}>Multiply 2</button><br>
<button on:click={div}>Divide 2</button>
