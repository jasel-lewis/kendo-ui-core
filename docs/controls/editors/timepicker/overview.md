---
title: Overview
page_title: Overview | Kendo UI TimePicker Widget
description: "Learn how to initialize the Kendo UI TimePicker widget and configure its behaviors."
slug: overview_kendoui_timepicker_widget
position: 1
---

# TimePicker Overview

The [Kendo UI TimePicker widget](http://demos.telerik.com/kendo-ui/timepicker/index) lets users select time values from a predefined list or enter new ones. It supports configurable options for the format, minimum/maximum time, and interval between the predefined values in the list.

## Getting Started

### Initialize the TimePicker

The DatePicker can be initialized via an `id` selector as demonstrated in the example below.

###### Example

    <input id="timePicker" />

    <script>
        $(document).ready(function(){
            $("#timePicker").kendoTimePicker();
        });
    </script>

> **Important**
>
> The widget copies any styles and CSS classes from the input element to the wrapper element.

## Configuration

Kendo UI DatePicker provides default configuration options that can be set during initialization. Some of the properties that can be overriden and controlled are:

*   Selected time
*   Minimum and/or maximum time
*   Time format
*   Define interval between predefined values in the list

### Selected, Min, and Max Time

The example below demonstrates how to define selected, min, and max times.

###### Example

    <input id="timePicker" />

    <script>
        $("#timePicker").kendoTimePicker({
            value: new Date(2000, 10, 10, 10, 0, 0),
            min: new Date(1950, 0, 1, 8, 0, 0),
            max: new Date(2049, 11, 31, 18, 0, 0)
        });
    </script>

The TimePicker will set the value only if the entered time is valid and within the defined range.

### Time Format

The exampe below demonstrates how to define the time format.

###### Example

    <input id="timePicker" />

    <script>
        $("#timePicker").kendoTimePicker({
            format: "hh:mm:ss tt"
        });
    </script>

### Interval between List Values

The example below demonstrates how to define the interval in minutes between values in the list.

###### Example

    <input id="timePicker" />

    <script>
        $("#timePicker").kendoTimePicker({
            interval: 15
        });
    </script>

## See Also

Other articles on Kendo UI TimePicker:

* [Overview of the ASP.NET MVC HtmlHelper Extension](/aspnet-mvc/helpers/timepicker/overview)
* [Overview of the JSP Tag](/jsp/tags/timepicker/overview)
* [Overview of the PHP Class](/php/widgets/timepicker/overview)
* [JavaScript API Reference](/api/javascript/ui/timepicker)

Articles on Kendo UI DatePicker:

* [Overview]({% slug overview_kendoui_datepicker_widget %})
* [How to Set the First Weekday]({% slug howto_set_first_weekday_datepicker %})
* [How to Create Date Masking]({% slug howto_create_date_masking_datepicker %})
* [How to Persist Entered Dates]({% slug howto_persist_entered_dates_datepicker %})
* [How to Resize Calendar Based on Input Width]({% slug howto_use_resize_calendar_basedon_input_width_datepicker %})
* [JavaScript API Reference](/api/javascript/ui/datepicker)

Articles on Kendo UI DateTimePicker:

* [Overview]({% slug overview_kendoui_datetimepicker_widget %})
* [How to Prevent Invalid Values]({% slug howto_prevent_invalid_values_datetimepicker %})
* [How to Validate Custom Dates]({% slug howto_validate_custom_dates_datetimepicker %})
* [How to Limit Navigation to Months]({% slug howto_limit_navigation_tomonths_datetimepicker %})
* [How to Override Hours in the Popup]({% slug howto_override_hours_inpopup_datetimepicker %})
* [JavaScript API Reference](/api/javascript/ui/datetimepicker)

Articles on Kendo UI Calendar:

* [Overview]({% slug overview_kendoui_calendar_widget %})
* [How to Control the Header Format]({% slug howto_control_header_format_calendar %})
* [JavaScript API Reference](/api/javascript/ui/calendar)
