---
title: Tipo de recurso itemPatent
description: Tipo de recurso itemPatent
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a6e53816f9e239de0f1c928763d1e329cc8cb63f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063619"
---
# <a name="itempatent-resource-type"></a>Tipo de recurso itemPatent
 
Namespace: microsoft.graph

Representa uma patente concedida ou arquivada que foi adicionada ao perfil de um [usuário.](../resources/profile.md)

Herda do [itemFacet](../resources/itemfacet.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar patentes](../api/profile-list-patents.md)|[coleção itemPatent](../resources/itempatent.md)|Obter os recursos itemPatent da propriedade de navegação de patentes.|
|[Criar itemPatent](../api/profile-post-patents.md)|[itemPatent](../resources/itempatent.md)|Crie um novo objeto itemPatent.|
|[Obter itemPatent](../api/itempatent-get.md)|[itemPatent](../resources/itempatent.md)|Leia as propriedades e as relações de um [objeto itemPatent.](../resources/itempatent.md)|
|[Atualizar itemPatent](../api/itempatent-update.md)|[itemPatent](../resources/itempatent.md)|Atualize as propriedades de um [objeto itemPatent.](../resources/itempatent.md)|
|[Excluir itemPatent](../api/itempatent-delete.md)|Nenhum|Exclui um [objeto itemPatent.](../resources/itempatent.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|Cadeia de caracteres|As audiências que são capazes de ver os valores contidos na entidade. Herdado [do itemFacet](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado [do itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|description|Cadeia de caracteres|Descpription of the patent or filing. |
|displayName|String|Título da patente ou arquivamento. |
|id|Cadeia de caracteres|Identificador usado para endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|inferência|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado [do itemFacet](../resources/itemfacet.md).|
|isPending        |Booliano     |Indica que a patente está pendente.        |
|issuedDate       |Data        |A data em que a patente foi concedida.   |
|issuingAuthority |Cadeia de Caracteres      |Autoridade que concedeu a patente.     |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado [do itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|number           |String      |O número da patente.                      |
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores se originaram se sincronizados de outro serviço. Herdado [do itemFacet](../resources/itemfacet.md).|
|webUrl           |String      |URL fazendo referência à patente ou ao arquivamento. |


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemPatent",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemPatent",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "description": "String",
  "displayName": "String",
  "isPending": "Boolean",
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "number": "String",
  "webUrl": "String"
}
```


