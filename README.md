# Instagram domain list

Этот репозиторий содержит список DNS-запросов, собранных из мобильного приложения Instagram на iOS с использованием техники сниффинга трафика.

Цель проекта — анализ сетевого поведения приложения и создание VPN-туннеля для трафика, исходящего от приложения, используя списки доменных имен.
Я использую маршрутизатор MikroTik с RouterOS, которая позволяет объявить список доменов и промаркировав трафик по признаку **dst-ip = insta-address-list** и завернуть его в VPN-туннель.
Тем самым на всех устройствах в сети, подключенных к маршрутизатору трафик от данного приложение будет отмаршрутизирован в иное место.

This repository contains a list of DNS queries captured from the Instagram iOS mobile application using traffic sniffing techniques.

The purpose of the project is to analyze the network behavior of the application and create a VPN tunnel for the traffic originating from the application using domain name lists. I use a MikroTik router with RouterOS on it, which allows declaring a list of domains and marking traffic with the criterion rule **dst-ip = insta-address-list** and routing it through a VPN tunnel. This way, on all devices in the network connected to the router, the traffic from this application will be routed to a different location.
