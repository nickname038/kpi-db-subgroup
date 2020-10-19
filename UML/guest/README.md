# Функції для гостей

### Реєстрація представника організації

#### Учасники: Незареєстрований користувач(представник організації), Система.
#### Передумови: До цього даний представник організації не був зареєстрований.
#### Результат: Обліковий запис представника організації створено.

1.	Користувач натискає кнопку "Реєстрація облікового запису представника";
2.	Система отримує ідентифікатор гостя та надсилає форму для введення електронної пошти;
3.	Користувач заповнює форму (ПІБ, електронна пошта);
4.	Система перевіряє дані на унікальність.;
5.	Система генерує код підтвердження створення облікового записую Надсилає лист на вказану пошту;
6.	Користувач в водить вказаний в отриманому листі код підтвердження. ;
7.	Система перевіряє правильність введеного коду;
8.	Система надсилає форму для внесення інформації про заклад/місце;
9.	Користувач заповнює і відправляє форму ;
10.	Система перевіряє надану інформацію, вносить відповідні записи до бази даних;
11.	Система надсилає користувачу дані для входу в обліковий запис;
12.	Користувач отримує дані для входу;

![Реєстрація представника організації](http://www.plantuml.com/plantuml/svg/fLRBJjjG4DtxAwxe1YGK0eik220s_OVkgb2IWaH95T9DnG8mZouGKMbafAeyslw02JOr0Jk_CFD7dND7E7Ng6AAk4bzVdtFcp9bhBs-rgitMn_SRpaQjtZ9hjUfghUau2_N6PikyRMmqcelbSjbihN-gBSw-N5fOMQ9pykatTScVNvXPMJ9qHI5tU9VtU8TyFcIFsuRwSX5IW6NoPNDC4VN8DvJ8ZHjPYjaJ5Dr_LYea_CL7id6N52DIMf4H0W0yANq2MNRVdP6ju8hiBHSt-6WoNzS8LLFJXdueW3ppG7wnp4iA5LpO7Y0bbTgXn0ZaiIpUo5yAKf5ZwJ5oDpHqZMfCKUt5EgzWd63Syp58UKzLqWLTovf7FK01nd9G7mwCsr1ZztNjpL3s9iMIJW4cv2Ty11nvcY9qxH7EAXo9O5wzVbCkpnlwzc_71Sf0CO8ZNObIy_MYIxTYANj85xlSAUQO5OwV5Yj1D_hoyrd01ISU0sLEbL80KpqAO9IDJW0n50j66ygwy5lTKmBg2iKEhei7z08wq4HD0tfn21m4HWZlr4sdjhcQpljsddVRZZqSd7c3QPEWu3QQpXrC5oZwr6FNJEIV0KacK9hzGQJO7HcgYGeKPKPlMrHaLmGVTEWaF1VxrIqhSn-qa8og39YjkBRDWe4LO9Ldxsqrl8zz048-xeVyruQ4iZUadiuQ5eT2K1dfeZCYckg5DefFiZ8cwP8EwSjq7gy_OFMdSgm2ONeQsSnm6oqBT4gDXH0LiPg4Wm3_hRRZKiNPRBHgfhd-RgrbNbIhzNgrcirRixQAd1dwBe9kHLw4zkeKbZHNWB0oli90I65NK_D4xfsXWoD-Jf0SEXzgA4G1IMkbBkh44vZFr3rs_w_OsKon1Sq_jQe3Yc1mHeqUizs_icnN4sGWBOAzfuqhcJ62WB73k4NPrcT3hpOhCRk2Rft2LyBOHiqDf-ByEVE7sEoc8P32uyTjWnSYAj4iuFq1r1b1yVJ4Avx8i-7XyuGKzgRsY8wCjZ4irXD6yvOd_MJQ0J6EfJGLoas9_jD9JKDktrmezTf6P_0UuuDAhgLvdp_ifeV0m6S-q0vh30k-0OhjlCWSngDf16MhrVXGSPOb4VBT-GS0)

[UML-код](https://github.com/nickname038/kpi-db-subgroup/blob/patch-1/UML/guest/Diagrams/registr_organization.pu)

### Авторизація представника організації

#### Учасники: Гість, Система.
#### Передумови: До цього даний користувач був зареєстрований і має обліковий запис.
#### Результат: Користувач отримує доступ до його облікового запису.

1.	Гість натискає кнопку "Увійти до облікового запису організації».";
2.	Система отримує запит та надсилає форму для авторизації;
3.	Користувач заповнює поля (Логін та Пароль) необхідними даними і натискає кнопку «Увійти»;
4.	Система перевіряє дані на унікальність.;
5.	Система перевіряє поля на заповненість. Перевіряє чи є такий користувач у базі і чи підходить пароль;
6.	Система надає користувачу доступ до його акаунту;
7.	Користувач може вільно користуватись можливостями свого акаунту;

![Авторизація представника організації](http://www.plantuml.com/plantuml/svg/dPNDRX9H5CVtzobkkjB486vS54hwAgsbqGIBeRWnB5h6bWqH4mbDD8gcIpUNATY10IRX2Svv8y__vCu4qe4QaoRbtlFn_vsF2uVdpQD6y_tRcgbLJvlsTVNefDemfdnQFslQL_LQlN5GB1Rj-PiFrOCNBolbumfz9qVt59BRBpy_hbZwJ26tQSaN5CczusiUSCzI8XSJ6lEb69suByGy8sVLyqwk5Zp8_6yAEoLlkIEEbpv7v8M_y03PkVlCqY-AL6b2StAxamrfuj42SLvIc2Niqz8AJbSkx-GZZScfvDIAgXQeUW6Avuwb4JvQ5864t5Vh1L9cWJom8EA-bUiHnLBpJ1rWH2GboBgR-AVGtejMp5qqazkUzsiUr58P8ffp0DKnBRqzqOEbQLhU9f2_p90uAEpUWnyO249zgH9oBQ0BT4EoJXNIcEhPIRPMhJpabj4TDFjh4xMQfWr7mTFspLGieHa7TezkAOG6NBIinwlPidYhkB1N4h2D1MePq6nSFMXichfjCHC5nhQBGwp0_162y0PWZ2VXSbxAJMbRMy2GPqYbjVFy2ImuGE49VKFbKj_2Kmqn3RLsdu9nWZxnbNYCTMnpqlwvz61uy4ZlLx_Ncx-AXV-VsfVuPoUXiX-zTMm8RbI5DKfNeM0D3H_4SaV0yL-gfDdsDuhkZ_259NNX3s6Ke7o-4gqnHT00IjQdKXwzJXVDo9NXOET30w4JmmBc_vWtlgN-qCIYVX1Y6daSRJrrqu2O8WezLKydBHCDjq5jVvprToLpACzOVYN-0W00)

[UML-код](https://github.com/nickname038/kpi-db-subgroup/blob/patch-1/UML/guest/Diagrams/authorization_organization.pu)
