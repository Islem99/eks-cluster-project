# EKS-Terraform



## Les prérequis

- Créer une instance Ubuntu 22.04
- Assurez-vous que vous avez correctement configuré vos informations d'identification AWS avec Terraform sinon vous pouvez les configurer comme suit:

  * Assurez-vous d'avoir installé l'AWS CLI sur votre système

  * Exécutez la commande aws configure. Vous serez invité à entrer les informations suivantes :

     *AWS Access Key ID : Entrez votre identifiant de clé d'accès AWS.

     *AWS Secret Access Key : Entrez votre clé d'accès secrète AWS.

     *Default region name : Entrez la région AWS par défaut que vous souhaitez utiliser (par exemple, "us-west-2" pour la région US     West (Oregon)).

     *Default output format : Vous pouvez laisser cette valeur vide ou spécifier un format de sortie par défaut pour les commandes AWS. Entrez "json", "text" ou "table" selon vos préférences.


## Les objectifs de projet Terraform

En utilisant Terraform, vous pouvez automatiser entièrement le processus de création du cluster EKS, y compris la configuration de la sécurité, les rôles IAM, les sous-réseaux, les groupes de sécurité, etc. Cela vous permet de provisionner facilement un cluster EKS avec une configuration cohérente et reproductible.

Dans notre projet nous allons:

1) créer VPC pour les "worker Nodes"
2) créer les "worker Nodes"

## Lancement de Terraform

 Initialisation

 `terraform init`

 Prévisualiser les actions que Terraform va effectuer

 `terraform plan`

  Appliquer les modifications spécifiées dans les fichiers de configuration Terraform sur notre infrastructure

 `terraform apply`

