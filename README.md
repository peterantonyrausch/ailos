# ailos



```abap
method m_send_single_message.

data: vl_message type string.

data: ol_connection type y_http_client.

me->m_connect_stablishing( importing e_return = r_return changing ch_connection = ol_connection ).

check r_return = 'SUCCESS'.

me->m_set_header( changing ch_connection = ol_connection ).
me->m_set_authentication( changing ch_connection = ol_connection ).
me->m_set_data( exporting
```
