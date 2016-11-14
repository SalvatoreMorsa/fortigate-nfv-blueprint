[![Build Status](https://circleci.com/gh/cloudify-examples/openstack-fortigate-nfv-blueprint.svg?style=shield&circle-token=:circle-token)](https://circleci.com/gh/cloudify-examples/openstack-fortigate-nfv-blueprint)

# Fortigate NVF Blueprint

## Requirements

* Openstack Kilo Environment or AWS Account
* Licensed Fortigate VM Snapshot

## Contents

* Main Network (Network, Router, Subnet, Port)
* Zone1 Network (Network, Subnet, Port1, Port2)
* Compute (Security Group, Key, Floating, IP, Fortigate VM, Test Server)
* Fortigate Configuration (Vlan A and Vlan X configurations)

The Fortigate VM should be a Snapshot of a valid-licensed Fortigate Server.

## Instructions:

* Create your inputs file. An example is provided.
* Run this command: `cfy install -p fortigate-nfv-blueprint/openstack-blueprint.yaml --task-retry-interval=10 --task-retries=25 -i inputs.yaml`

