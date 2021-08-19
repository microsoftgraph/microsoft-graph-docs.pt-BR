---
title: tipo de recurso itemAddress
description: tipo de recurso itemAddress
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7e11ab6a69e377144a53c298e1c8ad99d496557769be5d799dd0afa2beb38ea7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54167881"
---
# <a name="itemaddress-resource-type"></a>tipo de recurso itemAddress

Namespace: microsoft.graph

Representa um endereço físico e detalhes do local onde o endereço é encontrado.

Herda do [itemFacet](../resources/itemfacet.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar endereços](../api/profile-list-addresses.md)|[coleção itemAddress](../resources/itemaddress.md)|Obter os recursos itemAddress da propriedade de navegação de endereços.|
|[Criar itemAddress](../api/profile-post-addresses.md)|[itemAddress](../resources/itemaddress.md)|Crie um novo objeto itemAddress.|
|[Obter itemAddress](../api/itemaddress-get.md)|[itemAddress](../resources/itemaddress.md)|Leia as propriedades e as relações de um [objeto itemAddress.](../resources/itemaddress.md)|
|[Atualizar itemAddress](../api/itemaddress-update.md)|[itemAddress](../resources/itemaddress.md)|Atualize as propriedades de um [objeto itemAddress.](../resources/itemaddress.md)|
|[Excluir itemAddress](../api/itemaddress-delete.md)|Nenhum|Exclui um [objeto itemAddress.](../resources/itemaddress.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|Cadeia de caracteres|As audiências que são capazes de ver os valores contidos na entidade. Herdado [do itemFacet](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado [do itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|detail|[physicalAddress](../resources/physicaladdress.md)|Detalhes sobre o endereço em si.|
|displayName|Cadeia de caracteres|Nome amigável que o usuário atribuiu a esse endereço. |
|geoCoordinates|[geoCoordinates](../resources/geocoordinates.md)|As geocoordinações do endereço.|
|id|Cadeia de caracteres|Identificador usado para endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|inferência|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado [do itemFacet](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado [do itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores se originaram se sincronizados de outro serviço. Herdado [do itemFacet](../resources/itemfacet.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemAddress",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemAddress",
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
  "displayName": "String",
  "detail": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.geoCoordinates"
  }
}
```


