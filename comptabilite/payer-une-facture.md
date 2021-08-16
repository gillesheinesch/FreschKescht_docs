# Payer une facture

Dans le dossier **"À payer"** du trimestre en cours il y a maintenant toutes les factures qui doivent être payées et toutes les notes de crédit qui doivent être retenus sur les factures suivantes. 

Une fois qu'une facture a été payée, elle doit être renommée en `%{FOURNISSEUR}_${NUMERO_DE_FACTURE}`. Une fois cela fait, il faut le déplacer du dossier "**À payer**" vers le dossier **"Achats"**. Ce dossier contient toutes les factures et crédits payés.

* `%{FOURNISSEUR}`: Nom du fournisseur qui a crée la facture/note de crédit. Utilisez toujours le nom de fournisseur précédemment utilisé comme réference et tout en gros caractères
* `%{NUMERO_DE_FACTURE}`_:_ Numéro de facture/note de crédit qui est **écrit sur la facture** 

**Exemple:** _AMAZON\_AEU-INV-DE-2021-260902131_

{% hint style="warning" %}
**Si il n'y a pas de numéro de facture/note de crédit**, regardez dans les fichiers de factures précedantes sous quel nom on a sauvegardé les factures précédantes de ce fournisseur. S'il n'y en a pas, utilisez une réference qui vous semble logique comme numéro de facture.
{% endhint %}

{% hint style="info" %}
### Informations utiles

* Comme un **"/"** ne peut pas être utilisé dans les noms de fichiers, ils sont remplacés par un point **"."**
* Les noms de fichiers n'ont pas le droit d'avoir des espaces. Par exemple, si le numéro de facture d'Amazon est **"INV 931 AEU"**, le nom du fichier sera **"AMAZON\_INV931AEU"**
* Si une facture a été payée par **carte VISA** ou **prélèvement SEPA** \(via un extrait de compte bancaire\), la facture peut être déplacée directement du dossier "À payer" dans le fichier correspondant
{% endhint %}

