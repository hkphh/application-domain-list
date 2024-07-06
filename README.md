# Application domain list

Этот репозиторий содержит список DNS-запросов, собранных из различных приложений (iOS, Windows) с использованием техники сниффинга трафика.

Цель проекта — анализ сетевого поведения приложений и создание VPN-туннеля для трафика, исходящего от приложения, при помощи списков доменных имен.
Я использую маршрутизатор MikroTik с RouterOS, которая позволяет объявить список доменов и промаркировав трафик по признаку **dst-ip = app-address-list** и завернуть его в VPN-туннель.
Тем самым на всех устройствах в сети, подключенных к маршрутизатору трафик от данного приложения будет отмаршрутизирован в иное место.

This repository contains a list of DNS requests collected from various applications (iOS, Windows) using traffic sniffing techniques.

The project's goal is to analyze the network behavior of applications and create a VPN tunnel for the traffic originating from the applications using the domain name lists.
I am using a MikroTik router with RouterOS, which allows for declaring a list of domains, marking traffic with the attribute dst-ip = app-address-list, and wrapping it in a VPN tunnel.
This way, the traffic from the specified application on all devices connected to the router will be routed to a different location.
