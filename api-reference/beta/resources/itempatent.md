---
title: Tipo de recurso itemPatent
description: Tipo de recurso itemPatent
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 424d3e047af36307be8d2589e2ab1dddcadf87785e4f58fa020fb9eae085a1b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54248324"
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
|displayName|Cadeia de caracteres|Título da patente ou arquivamento. |
|id|Cadeia de caracteres|Identificador usado para endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|inferência|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado [do itemFacet](../resources/itemfacet.md).|
|isPending        |Boolean     |Indica que a patente está pendente.        |
|issuedDate       |Data        |A data em que a patente foi concedida.   |
|issuingAuthority |Cadeia de caracteres      |Autoridade que concedeu a patente.     |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado [do itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|number           |Cadeia de caracteres      |O número da patente.                      |
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


