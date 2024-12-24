

<script setup lang="tsx">
import {
     useSlots,
} from 'vue';

const slots = useSlots();


defineSlots<{
    default(props: null): any;
}>();

defineRender(() => {
  return (
            <div>
                {slots.default?.()}
            </div>
        );
});
</script>
