<!-- ABOUT THE PROJECT -->

## About The Project

This simple package converts English Keyboard to Persian inputs and vice versa on-the-go. it also supports Number-Only inputs.
useful for Persian only inputs. so the client doesn't need to switch the keyboard layout.

این پکیج ساده کاراکتر های وارد شده به انگلیسی را به حروف فارسی تبدیل میکند.
این پکیج برای اینپوت هایی که کاربر فقط حروف فارسی باید در آن تایپ کند کاربردیست.
تا کاربر بدون احتاج به عوض کردن زبان کیبورد، فارسی وارد کند.
حمایت از ورودی های عددی اضافه شده

Functions:

- **persianNum:** takes a string and returns only Numbers in Persian chars.
- **persianTellNum:** like persianNum and + sign is allowed.
- **persian:** return string with persian chars. accepts anything, nums, chars, special chars.
- **persianChar:** accepts characters only.
- **englishNum:** turns persian characters to english. returns english numbers of string.
- **english:** turns persian characters to english. accepts anything, nums, chars, special chars.
- **Separator:** separate each three character with a ، .

<!-- GETTING STARTED -->

## Getting Started

### Installation

Install NPM packages

```sh
npm i persiantool
```

<!-- USAGE EXAMPLES -->

## Usage

### persianNum

```JS
persinaNum("1234567890")
// ۱۲۳۴۵۶۷۸۹۰
```

Removes non-number characters

```JS
persinaNum("aAbv1sd2+/}]")
// ۱۲
```

### persianTellNum

accepts + sign

```JS
persianTellNum("+1234567890")
// +۱۲۳۴۵۶۷۸۹۰
```

### persian

num,char,special char

```JS
persian("+1234abcdef")
// +شذزیثب۱۲۳۴
```

### persianChar

Removes Numbers

```JS
persianChar("123abcd")
// شذزی
```

### englishNum

Removes non-Numbers

```JS
englishNum("شسی۱۲۳")
// 123
```

### english

```JS
english("شسی۱۲۳")
// 123asd
```

### Separator

put a camma , each three characters Whether it's Persian or English

```JS
english("1000000")
// 1,000,000
```
