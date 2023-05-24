# Upto3 Organizations

This project designed to manage and standardize all organizational information for Upto3. 

The goal is to provide an open-source platform for managing the organizational structure upon which event submissions depend.

## Organization JSON Format

Organizations are represented in JSON format with the name info.json and has the following properties:

- `name`: a string representing the organization's name
- `token`: a string representing the organization's token, if it does not exist, please fill in `null`
- `intro`: a string providing a brief introduction to the organization, 20 characters or less
- `links`: an array of objects containing information about the organization's website, twitter accounts, and other relevant links
- `introduce`: a string providing a detailed introduction to the organization

## Organization JSON Example

```json
{
    "name": "Bitcoin",
    "token": "BTC",
    "intro": "Decentralized digital currency",
    "links": [
        {
            "title": "Website",
            "url": "https://bitcoin.org/"
        },
        {
            "title": "Twitter",
            "url": "https://twitter.com/bitcoin"
        },
        {
            "title": "Github",
            "url": "https://github.com/bitcoin/bitcoin"
        }
    ],
    "introduce": "Bitcoin is a decentralized digital currency, without a central bank or single administrator, that can be sent from user to user on the peer-to-peer bitcoin network without the need for intermediaries. Transactions are verified by network nodes through cryptography and recorded in a public distributed ledger called a blockchain. The cryptocurrency was invented in 2008 by an unknown person or group of people using the name Satoshi Nakamoto. The currency began use in 2009 when its implementation was released as open-source software."
}
```

## Submit information

We welcome contributions from the community! To submit to this project, please follow these steps:

1. Fork the repository
2. Create a new branch for your feature
3. Make your changes and commit them
4. Push your changes to your forked repository
5. Open a pull request to merge your changes into the main repository

## Assets Requirements

**You can copy the template folder directly and modify it directly.**

* Create a directory using the organization's name, with all letters in lowercase. If there are spaces in the name, use _ instead.
* All organization logos must be in **JPG/PNG** format with dimensions of **300x300 pixels**, and named logo.jpg or logo.png.

Example:
```
.
├── bitcoin
│   ├── logo.jpg
│   └── info.json
├── ethereum
│   ├── logo.jpg
│   └── info.json
├── ethereum_name_service
│   ├── logo.png
│   └── info.json
```


## License

This project is licensed under the Apache License Version 2.0.
