# Cobblemon Server
An Ansible role designed to deploy a Minecraft server with the Cobblemon modpack using the Fabric mod loader.

## About
This Ansible role automates the setup of a Minecraft server running the Cobblemon modpack. Cobblemon is a mod that brings Pokémon-inspired gameplay to Minecraft, allowing players to catch, train, and battle Pokémon within the Minecraft world. This role utilizes the Fabric mod loader to ensure compatibility and performance.

## Requirements
* Ansible 2.9 or higher
* A supported operating system (e.g., Ubuntu, CentOS)
* A Linux machine to be the server

## Setup
Clone the repository:

```bash
git clone https://github.com/winiciusallan/cobblemon-server.git
cd cobblemon-server
```

* Configure your inventory file (inventory.ini) with your server details.
* Customize the `group_vars/all.yml` as needed to set your desired configurations.

Run the playbook:
```bash
ansible-playbook -i inventory.ini main.yml
```

If you want to just reconfigure the server you can run:
```bash
ansible-playbook -i inventory.ini main.yml -t setup
```

## Contributing

Contributions are welcome! If you'd like to help improve this project, follow these steps:

1. **Fork the repository**
   Click the "Fork" button in the top right of the repository page.

2. **Create a new branch**
   Use a descriptive name for your feature or fix.
   ```bash
   git checkout -b my-feature-name
   ```

3. Make your changes and open a PR

## License
This project is licensed under the MIT License - see the LICENSE file for details.
