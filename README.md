# bookshop-api

symfony serve -d --no-tls
pour créer une base de données:

 php bin/console doctrine:database:create
 php bin/console doctrine:schema:create
 pour installer Maker:
composer require symfony/maker-bundle --dev 


Il y a deux manière de mettre d'ajouter les ressources:
par annotation: 
use ApiPlatform\Core\Annotation\ApiResource;
@ApiResource()

OU 

creer un dossier dans config/packages/apii_platform
creer dedans un fichie resource.yaml
   et ajouter ceci

   resources:
        App\Entity\Post: ~