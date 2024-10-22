<script setup>
import { LinearGaugeComponent as EjsLineargauge, AxesDirective as EAxes, AxisDirective as EAxis,
  PointerDirective as EPointer, PointersDirective as EPointers,
  RangesDirective as ERanges, RangeDirective as ERange
 } from '@syncfusion/ej2-vue-lineargauge';
const line = {
      height: 350,
      width: 7,
      color: '#4286f4'
};
const labelStyle = {
  format: "{value}°C"
};
</script>

<template>
  <ejs-lineargauge >
        <e-axes>
          <e-axis :line='line' :labelStyle='labelStyle'>
            <e-pointers>
              <e-pointer value=80></e-pointer>
            </e-pointers>
            <e-ranges>
                <e-range start=30 end=60></e-range>
                <e-range start=60 end=90 color="#41f47f"></e-range>
            </e-ranges>
          </e-axis>
        </e-axes>
      </ejs-lineargauge>
</template>

<style>

</style>
