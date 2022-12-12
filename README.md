# tritpo2

# Требования к проекту
---
# Содержание
1 [Введение](#intro)

1.1 [Название продукта](#product_name)                    
1.2 [Назначение документа](#appointment)                     
1.3 [Бизнес-требования](#business_requirements)                      
1.3.1 [Исходные данные](#initial_data)  
1.3.2 [Возможности бизнеса](#business_opportunities)  
1.3.3 [Границы проекта](#project_boundary)  
1.4 [Аналоги](#analogues)  
2 [Требования пользователя](#user_requirements)  
2.1 [Программные интерфейсы](#software_interfaces)                        
2.2 [Интерфейс пользователя](#user_interface)  
2.3 [Характеристики пользователей](#user_specifications)  
2.3.1 [Классы пользователей](#user_classes)  
2.3.2 [Аудитория приложения](#application_audience)  
2.3.2.1 [Целевая аудитория](#target_audience)  
2.3.2.1 [Побочная аудитория](#collateral_audience)  
2.4 [Предположения и зависимости](#assumptions_and_dependencies)  
3 [Системные требования](#system_requirements)  
3.1 [Функциональные требования](#functional_requirements)  
3.1.1 [Основные функции](#main_functions)  
3.1.1.1 [Вход пользователя в приложение](#user_logon_to_the_application)  
3.1.1.2 [Настройка профиля зарегистрированного пользователя](#setting_up_the_profile_of_the_active_user)  
3.1.1.3 [Опрос пользователя о своих предпочтениях](#user_asking)  
3.1.1.4 [Просмотр информации об отдельной анкете](#view_information_about_an_individual_anket)  
3.1.1.5 [Выход зарегистрированного пользователя из учётной записи](#active_user_change)  
3.1.1.6 [Регистрация нового пользователя после входа в приложение](#add_new_user)                      
3.1.1.7 [Просмотр анкет онлайн](#watch_anket)                      
3.1.1.8 [Скачивание изображений](#download_anket)                      
3.1.2 [Ограничения и исключения](#restrictions_and_exclusions)  
3.2 [Нефункциональные требования](#non-functional_requirements)  
3.2.1 [Атрибуты качества](#quality_attributes)  
3.2.1.1 [Требования к удобству использования](#requirements_for_ease_of_use)  
3.2.1.2 [Требования к безопасности](#security_requirements)  
3.2.2 [Внешние интерфейсы](#external_interfaces)  
3.2.3 [Ограничения](#restrictions)  
# 1 Введение
<a name="intro"/>

## 1.1 Название продукта
<a name="product_name"/>
Zoomber

## 1.2 Назначение документа
<a name="appointment"/>
В этом документе описаны функциональные и нефункциональные требования к веб-сервису «Zoomber» для мобильных телефонов.
Этот документ предназначен для команды, которая будет реализовывать и проверять корректность работы веб-сервиса.

## 1.3 Бизнес-требования
<a name="business_requirements"/>

### 1.3.1 Исходные данные
<a name="initial_data"/>
Приложения для знакомств – не теряющая популярности уже который год бизнес-модель. Ведь так или иначе, здесь идет игра на простых желаниях и мечтах человека.
В первую очередь (для пользователей) приложения для знакомств – это место, где предоставляется возможность подать себя с любой стороны. Можно представляться умнее, красивее, лучше, чем ты есть, в надежде встретить человека, который бы в жизни на тебя и не посмотрел. И здесь цели и способы представителей разных полов, естественно, также различны. Если девушки ищут принцев (с мерседесом и яхтой), то молодые люди редко заморачиваются чем-то, кроме внешности партнерши (да и то она важна далеко не для всех).

### 1.3.2 Возможности бизнеса
<a name="business_opportunities"/>
Многие люди желают иметь приложения, позволяющее искать людей по интересам, узнавать что-то новое или просто переписываться. Подобный сервис позволит им тратить меньше времени на поиск людей вживую и использовать сервис в удобное время, чтобы не знакомится со случайным человеком в реальном мире. Интерфейс, спроектированный с учётом всех особенностей похожих технологий, и дополнение веб-сервиса подробной инструкцией позволят увеличить количество людей, использующих данный сервис.
Подбор анкет будет осуществляться по специальному алгоритму, учитывающему общие интересы с другими пользователи.

### 1.3.3 Границы проекта
<a name="project_boundary"/>
Веб-сервис "Zoomber" позволит зарегистрированным пользователям создать свою анкету,оставлять свои личные данные, такие как: возраст, пол, гороскоп, свой город, фотографии, наличие вредных привычек, наличие питомцев, место работы, место учёбы, подключать свои соц. сети(Instagram), просмотр чужих анкет и их информации, возможность поставить лайк или пропустить. Так же можно оформить подписку, после чего будет доступно просмотр анкет, от которых вы получили лайк и отключение рекламы.

## 1.4 Аналоги
<a name="analogues"/>
Tinder  — популярное частично платное приложение для мобильных платформ Android и iOS, предназначенное для романтических знакомств в соответствии с заданными параметрами и с учётом геолокации. Возможно подключение профиля через Facebook, аккаунт Google или даже по номеру телефона. Управляется североамериканской корпорацией Match Group, дочерней компанией IAC. 

Badoo — социальная сеть знакомств, поддерживающая множество языков и работающая с пользователями всех стран мира. Главный офис компании располагается в Сохо, Лондон, однако сама компания зарегистрирована на Кипре, а принадлежит российскому бизнесмену Андрею Андрееву. Социальная сеть Badoo работает фактически со всеми странами мира, но наиболее популярна она в Латинской Америке, Испании, Италии и Франции.

### 1.4.1 Отличия от аналогов
В отличие от Tinder и Badoo пользователи веб-сервиса Zoomber имеет безлимит лайков и безлимит на функцию "Отменить".
Также, в отличие от Tinder, на веб-сервисе скачивание фотографий анкет и загрузка видео в свою анкету.

# 2 Требования пользователя
<a name="user_requirements"/>

## 2.1 Программные интерфейсы
<a name="software_interfaces"/>
Веб-сервис использует ресурс Zoomber.dev, созданный для реализации алгоритмов поиска и подборки
Языки программирования: Java и C#
API: Java SE, Java EE
Фреймворки: Android studio, Java Media Framework
Аппаратная платформа:   Android и iOS

## 2.2 Интерфейс пользователя
<a name="user_interface"/>

Окно входа в сервис. 

![Окно входа в сервис](https://github.com/valik292/Tritpo/blob/main/mockups/%D0%9C%D0%BE%D0%BA%D0%B0%D0%BF%20%D0%BE%D0%BA%D0%BD%D0%B0%20%D0%B2%D1%85%D0%BE%D0%B4%D0%B0%20%D0%B2%20%D0%BF%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5.jpg)

Окно просмотра анкет других пользователей.

![Окно просмотра анкет других пользователей](https://github.com/valik292/Tritpo/blob/main/mockups/%D0%9C%D0%BE%D0%BA%D0%B0%D0%BF%20%D0%BE%D0%BA%D0%BD%D0%B0%20%D0%B0%D0%BD%D0%BA%D0%B5%D1%82%20%D0%B4%D1%80%D1%83%D0%B3%D0%B8%D1%85%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D0%B5%D0%B9.jpg)
 
Окно чата.

![Окно чата](https://github.com/valik292/Tritpo/blob/main/mockups/%D0%9C%D0%BE%D0%BA%D0%B0%D0%BF%20%D0%BE%D0%BA%D0%BD%D0%B0%20%D1%87%D0%B0%D1%82%D0%B0.jpg)

Окно анкеты пользователя.

![Окно анкеты пользователя](https://github.com/valik292/Tritpo/blob/main/mockups/%D0%9C%D0%BE%D0%BA%D0%B0%D0%BF%20%D0%BE%D0%BA%D0%BD%D0%B0%20%D0%B0%D0%BD%D0%BA%D0%B5%D1%82%D1%8B%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8F.jpg)

Окно просмотра настроек пользователя.

![Окно просмотра настроек пользователя](https://github.com/valik292/Tritpo/blob/main/mockups/%D0%9C%D0%BE%D0%BA%D0%B0%D0%BF%20%D0%BE%D0%BA%D0%BD%D0%B0%20%D0%BD%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B5%D0%BA.jpg)

## 2.3 Характеристики пользователей
<a name="user_specifications"/>

### 2.3.1 Классы пользователей
<a name="user_classes"/>
1)Зарегистрированные пользователи - пользователи, которые зарегестрировались в приложение и заполнили свою анкету. Имеют доступ к начальному функционалу функционалу
2)VIP пользователи - пользователи, которые оформили подписку. Имеют доступ к полному функционалу.

### 2.3.2 Аудитория приложения
<a name="application_audience"/>

#### 2.3.2.1 Целевая аудитория
<a name="target_audience"/>

#### 2.3.2.1 Побочная аудитория
<a name="collateral_audience"/>

Приложение расчитано на совершеннолетних пользователей возрастной категории(18-60) лет, обладающие умением взаимодействовать с телефоном.

### 2.4 Предположения и зависимости
<a name="assumptions_and_dependencies"/>
1. Веб-сервис должен иметь возможность обрабатывать значительное количество запросов в секунду;
2. Допустимое время ответа сервера не должно превышать 2 секунды;
3. На сервисе ожидается большое количество пользователей;
4. Требуется хранить значительное количество информации об анкетах пользователей и их чатах.

# 3 Cистемные требования
<a name="system_requirements"/>

## 3.1 Функциональные требования
<a name="functional_requirements"/>

### 3.1.1 Основные функции
<a name="main_functions"/>

#### 3.1.1.1 Вход пользователя в приложение
<a name="user_logon_to_the_application"/>
Описание. Пользователь не имеет возможность использовать приложение без создания собственного профиля либо войдя в свою учётную запись.

| Функция | Требования | 
|:---|:---|
| Вход в приложение без создания собственного профиля | Приложение не предоставляет пользователю возможность войти в приложение анонимно |
| Регистрация нового пользователя | Приложение должно запросить у пользователя ввести свою почту или номер телефона для создания учётной записи.|
| Пользователь с такой почтой(телефоном) уже существует | Приложение должно известить пользователя об ошибке регистрации и запросить ввод уже другой почты или нормера телефона. Пользователь должен либо ввести почту/телефон, либо отменить действие |
| Вход зарегистрированного пользователя в приложение | Приложение должно предоставить пользователю список почт (телефонов) уже зарегестрированных пользователей. Пользователь должен либо выбрать из списка своё имя (псевдоним), либо отменить действие |

#### 3.1.1.2 Настройка профиля зарегистрированного пользователя
<a name="setting_up_the_profile_of_the_active_user"/>
Описание. Зарегистрированный пользователь имеет возможность редактировать свою анкету.

| Функция | Требования | 
|:---|:---|
| Редактирование общей информации о пользователе | Приложение должно предоставить зарегистрированному пользователю поле для ввода общей информации о себе. Пользователь должен либо ввести информацию и подвердить действие, либо отменить его |
| Редактирование параметров рекомендуемых пользователей | Зарегистрированный пользователь имеет возможножность редактировать параметры рекомендуемых пользователей(Возраст, город и т.д.) |

#### 3.1.1.3 Опрос пользователя о своих предпочтениях
<a name="user_asking"/>
Описание. Зарегистрированный пользователь имеет возможность указать приложению свои предпочтения, которые в дальнейшем обработаются приложением и используются для выборки других анкет для пользователя

| Функция | Требования | 
|:---|:---|
| Заполнение анкеты о предпочтениях | Приложение должно предоставить зарегистрированному пользователю поле для ввода информации о предпочтениях, привычках, вкусах и т.д. Пользователь должен либо ввести информацию и подвердить действие, либо пропустить его |

#### 3.1.1.4 Просмотр информации об отдельной анкете
<a name="view_information_about_an_individual_anket"/>
Описание. Зарегистрированный пользователь имеет возможность просматривать краткую и полную информацию о чужой анкете

| Функция | Требования | 
|:---|:---|
| Просмотр предварительной(краткой) информации | Приложение должно предоставить пользователю возможность увидеть краткую информацию о анкете на главной странице |
| Просмотр полной информации | Приложение должно предоставить пользователю возможность увидеть полную информацию о анкете |

#### 3.1.1.5 Выход зарегистрированного пользователя из учетной записи
<a name="active_user_change"/>
Описание. Зарегистрированный пользователь имеет возможность выйти из своего профиля.

Требование. Приложение должно предоставить зарегистрированному пользователю возможность выйти из учётной записи с возвратом к окну входа в приложение.

#### 3.1.1.6 Регистрация нового пользователя после входа в приложение
<a name="add_new_user"/>
Описание. Анонимный пользователь имеет возможность зарегистрироваться в приложении.

Требование. Приложение должно предоставить анонимному пользователю возможность [зарегистрироваться в приложении]

#### 3.1.1.7 Просмотр анкет онлайн
<a name="watch_anket"/>
Описание. Зарегистрированный пользователь имеет возможность просматривать анкет онлайн

Требование. Приложение должно предоставить анонимному пользователю возможность просмотра анкет онлайн, отобразив графический интерфейс просмотра анкет

#### 3.1.1.8 Скачивание изображений
<a name="download_anket"/>
Описание. Зарегистрированный пользователь имеет возможность скачать фотографии с анкет на свое устройство

Требование. Приложение должно предоставить зарегистрированному пользователю возможность скачивания изображений, отобразив графический интерфейс скачивания изображения

### 3.1.2 Ограничения и исключения
<a name="restrictions_and_exclusions"/>
1. Приложение работает только при наличии подключения к Интернету;
2. Приложение функционирует корректно только при корректной работе сервиса Zoomber.dev 

## 3.2 Нефункциональные требования
<a name="non-functional_requirements"/>

### 3.2.1 Атрибуты качества
<a name="quality_attributes"/>

#### 3.2.1.1 Требования к удобству использования
<a name="requirements_for_ease_of_use"/>
1. Доступ к основным функциям приложения не более чем за две операции;
2. Все функциональные элементы пользовательского интерфейса имеют названия, описывающие действие, которое произойдет при выборе элемента;
3. Пошаговая инструкция использования основных функций приложения отображена в справке;
4. Понятный графический интерфейс

#### 3.2.1.2 Требования к безопасности
<a name="security_requirements"/>
Приложение предоставляет возможность просмотра и редактирования профиля только активного пользователя.
Приложение гарантирует безопасность личных данных пользователей.

### 3.2.2 Внешние интерфейсы
<a name="external_interfaces"/>
Окна приложения удобны для использования пользователями с плохим зрением:
  * размер шрифта не менее 14пт;
  * функциональные элементы контрастны фону окна.

### 3.2.3 Ограничения
<a name="restrictions"/>
1. Приложение реализовано на платформе Android Studio;
2. Профиль пользователя хранится в файле с расширением XML, название файла совпадает с почтой (телефоном);
3. Информация о анкетах и чатах хранится в базе данных MySQL.
4. Приложение не работает при отсутствии подключения к Интернету;
5. Приложение не обрабатывает данные анкет, недоступных в момент запроса;
6. Качество изображения зависит от скорости подключения пользователя.
