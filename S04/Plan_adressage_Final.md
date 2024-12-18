# Plan d'adressage pour la société Pharmgreen

## Base technique

**Adresse IP de réseau** : 10.15.0.0/16  
**Adresse de passerelle** : 10.15.255.254  
**Adresse IP DNS** : 10.15.255.254  

## Plan d'adressage


| ID  | Sous-réseau               | Adresses total| Adresse réseau | Masque CIDR | Masque    | Début plage IP  | Fin plage IP     | Adresse broadcast |
|-----|---------------------------|--------------|----------------|-------------|-------------------|-----------------|------------------|-------------------|
| 5   | VLAN DC                   | 4            | 10.15.0.0      | /30         | 255.255.255.252   | 10.15.0.1       | 10.15.0.2        | 10.15.0.3         |
| 10  | VLAN Administration       | 16           | 10.15.0.16     | /28         | 255.255.255.240   | 10.15.0.17      | 10.15.0.30       | 10.15.0.31        |
| 20  | VLAN Serveurs             | 32           | 10.15.0.32     | /27         | 255.255.255.224   | 10.15.0.33      | 10.15.0.62       | 10.15.0.63        |
| 30  | VLAN Téléphonie           | 256          | 10.15.1.0      | /24         | 255.255.255.0     | 10.15.1.1       | 10.15.1.254      | 10.15.1.255       |
| 40  | VLAN Utilisateurs         | 256          | 10.15.2.0      | /24         | 255.255.255.0     | 10.15.2.1       | 10.15.2.254      | 10.15.2.255       |
| 50  | VLAN Wi-Fi Entreprise     | 256          | 10.15.3.0      | /24         | 255.255.255.0     | 10.15.3.1       | 10.15.3.254      | 10.15.3.255       |
| 51  | VLAN Wi-Fi Invités        | 256          | 10.15.4.0      | /24         | 255.255.255.0     | 10.15.4.1       | 10.15.4.254      | 10.15.4.255       |
| 60  | VLAN IoT                  | 128          | 10.15.5.0      | /25         | 255.255.255.128   | 10.15.5.1       | 10.15.5.126      | 10.15.5.127       |
| 70  | VLAN Impressions          | 16           | 10.15.5.128    | /28         | 255.255.255.0     | 10.15.5.129     | 10.15.5.142      | 10.15.5.143       |
| 80  | VLAN Services annexes 1   | 256          | 10.15.6.0      | /24         | 255.255.255.0     | 10.15.6.1       | 10.15.6.254      | 10.15.6.255       |
| 81  | VLAN Services annexes 2   | 256          | 10.15.7.0      | /24         | 255.255.255.0     | 10.15.7.1       | 10.15.7.254      | 10.15.7.255       |
| 90  | VLAN de secours 1         | 256          | 10.15.8.0      | /24         | 255.255.255.0     | 10.15.8.1       | 10.15.8.254      | 10.15.8.255       |
| 91  | VLAN de secours 2         | 256          | 10.15.9.0      | /24         | 255.255.255.0     | 10.15.9.1       | 10.15.9.254      | 10.15.9.255       |