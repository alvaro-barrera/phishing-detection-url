# DETECCIÓN DE PHISHING EN URL
Detección de sitios sospechos utilizando Machine Learning

## Dataset
### dataset_full.csv: https://drive.google.com/file/d/1K6gRJgrCuB6o1s-VVf-Q05IwMpUkmmXx/view?usp=sharing
- Número total de registros: 88,647
    - Total de registros legítimos (etiqueta - 0): 58,000
    - Total de registros phishing (etiqueta - 1): 30,647

### dataset_small.csv: https://drive.google.com/file/d/1dXB5XV8dJENIMXipuCEneJ_ZLRkNViLP/view?usp=sharing
- Número total de registros: 58,645
  - Total de registros legítimos (etiqueta - 0): 27,998
  - Total de registros phishing (etiqueta - 1): 30,647
  
## Descripción de contenido

|          Feature           |                   Description                      |
|----------------------------|----------------------------------------------------|
| qty_dot_url                | count (.) in URL                                   |
| qty_hyphen_url             | count (-) in URL                                   |
| qty_underline_url          | count (_) in URL                                   |
| qty_slash_url              | count (/) in URL                                   |
| qty_questionmark_url       | count (?) in URL                                   |
| qty_equal_url              | count (=) in URL                                   |
| qty_at_url                 | count (@) in URL                                   |
| qty_and_url                | count (&) in URL                                   |
| qty_exclamation_url        | count (!) in URL                                   |
| qty_space_url	             | count ( ) in URL                                   |
| qty_tilde_url	             | count (~) in URL                                   |
| qty_comma_url	             | count (,) in URL                                   |
| qty_plus_url	             | count (+) in URL                                   |
| qty_asterisk_url	         | count (*) in URL                                   |
| qty_hashtag_url	         | count (#) in URL                                   |
| qty_dollar_url	         | count ($) in URL                                   |
| qty_percent_url	         | count (%) in URL                                   |
| qty_tld_url	             | top-level-domain length                            |
| length_url	             | URL length                                         |
| qty_dot_domain	         | count (.) in domain                                |
| qty_hyphen_domain	         | count (-) in domain                                |
| qty_underline_domain       | count (_) in domain                                |
| qty_slash_domain	         | count (/) in domain                                |
| qty_questionmark_domain    | count (?) in domain                                |
| qty_equal_domain           | count (=) in domain                                |
| qty_at_domain              | count (@) in domain                                |
| qty_and_domain             | count (&) in domain                                |
| qty_exclamation_domain     | count (!) in domain                                |
| qty_space_domain           | count ( ) in domain                                |
| qty_tilde_domain           | count (~) in domain                                |
| qty_comma_domain           | count (,) in domain                                |
| qty_plus_domain            | count (+) in domain                                |
| qty_asterisk_domain        | count (*) in domain                                |
| qty_hashtag_domain         | count (#) in domain                                |
| qty_dollar_domain          | count ($) in domain                                |
| qty_percent_domain         | count (%) in domain                                |
| qty_vowels_domain          | count vowels in domain                             |
| domain_length              | domain length                                      |
| domain_in_ip               | URL domain in IP address format                    |
| server_client_domain       | domain contains the keywords "server" or "client"  |
| qty_dot_directory	         | count (.) in directory                             |
| qty_hyphen_directory       | count (-) in directory                             |
| qty_underline_directory    | count (_) in directory                             |
| qty_slash_directory        | count (/) in directory                             |
| qty_questionmark_directory | count (?) in directory                             |
| qty_equal_directory        | count (=) in directory                             |
| qty_at_directory           | count (@) in directory                             |
| qty_and_directory          | count (&) in directory                             |
| qty_exclamation_directory	 | count (!) in directory                             |
| qty_space_directory        | count ( ) in directory                             |
| qty_tilde_directory        | count (~) in directory                             |
| qty_comma_directory        | count (,) in directory                             |
| qty_plus_directory         | count (+) in directory                             |
| qty_asterisk_directory     | count (*) in directory                             |
| qty_hashtag_directory      | count (#) in directory                             |
| qty_dollar_directory       | count ($) in directory                             |
| qty_percent_directory      | count (%) in directory                             |
| directory_length           | directory length                                   |
| qty_dot_file               | count (.) in file                                  |
| qty_hyphen_file            | count (-) in file                                  |
| qty_underline_file         | count (_) in file                                  |
| qty_slash_file             | count (/) in file                                  |
| qty_questionmark_file      | count (?) in file                                  |
| qty_equal_file             | count (=) in file                                  |
| qty_at_file                | count (@) in file                                  |
| qty_and_file               | count (&) in file                                  |
| qty_exclamation_file       | count (!) in file                                  |
| qty_space_file             | count ( ) in file                                  |
| qty_tilde_file             | count (~) in file                                  |
| qty_comma_file             | count (,) in file                                  |
| qty_plus_file	             | count (+) in file                                  |
| qty_asterisk_file          | count (*) in file                                  |
| qty_hashtag_file           | count (#) in file                                  |
| qty_dollar_file            | count ($) in file                                  |
| qty_percent_file           | count (%) in file                                  |
| file_length                | file length                                        |
| qty_dot_params             | count (.) in parameters                            |
| qty_hyphen_params          | count (-) in parameters                            |
| qty_underline_params       | count (_) in parameters                            |
| qty_slash_params           | count (/) in parameters                            |
| qty_questionmark_params    | count (?) in parameters                            |
| qty_equal_params           | count (=) in parameters                            |
| qty_at_params              | count (@) in parameters                            |
| qty_and_params             | count (&) in parameters                            |
| qty_exclamation_params     | count (!) in parameters                            |
| qty_space_params           | count ( ) in parameters                            |
| qty_tilde_params           | count (~) in parameters                            |
| qty_comma_params           | count (,) in parameters                            |
| qty_plus_params            | count (+) in parameters                            |
| qty_asterisk_params        | count (*) in parameters                            |
| qty_hashtag_params         | count (#) in parameters                            |
| qty_dollar_params          | count ($) in parameters                            |
| qty_percent_params         | count (%) in parameters                            |
| params_length              | parameters length                                  |
| tld_present_params         | TLD presence in arguments                          |
| qty_params                 | number of parameters                               |
| email_in_url               | email present in URL                               |
| time_response              | search time (response) domain (lookup)             |
| domain_spf                 | domain has SPF                                     |
| asn_ip                     | AS Number (or ASN)                                 |
| time_domain_activation     | time (in days) of domain activation                |
| time_domain_expiration     | time (in days) of domain expiration                |
| qty_ip_resolved            | number of resolved IPs                             |
| qty_nameservers            | number of resolved name servers (NameServers - NS) |
| qty_mx_servers             | number of MX Servers                               |
| ttl_hostname               | time-to-live (TTL) value associated with hostname  |
| tls_ssl_certificate        | valid TLS / SSL Certificate                        |
| qty_redirects              | number of redirects                                |
| url_google_index           | check if URL is indexed on Google                  |
| domain_google_index        | check if domain is indexed on Google               |
| url_shortened              | check if URL is shortened                          |
| phishing                   | is phishing website                                |
