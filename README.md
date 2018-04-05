# Android-DatePicker


```
Calendar calendar = Calendar.getInstance();
        calendar.setTime(new Date());
        DatePickerDialog datePickerDialog = new DatePickerDialog(getActivity(), new DatePickerDialog.OnDateSetListener() {
            @Override
            public void onDateSet(DatePicker datePicker, int year, int month, int dayOfMonth) {
                todaysDate = DateUtil.buildDatePickerStringDate(year, month, dayOfMonth);
                btnStartDate.setText(todaysDate);
            }
        }, calendar.get(Calendar.YEAR), calendar.get(Calendar.MONTH), calendar.get(Calendar.DAY_OF_MONTH));
        datePickerDialog.getDatePicker().setMaxDate(System.currentTimeMillis());
        datePickerDialog.show();
```
