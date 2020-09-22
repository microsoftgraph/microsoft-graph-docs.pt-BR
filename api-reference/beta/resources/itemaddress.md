---
title: tipo de recurso de endereço
description: tipo de recurso de endereço
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ca6848b6b5ac60d419e56914a59e2470d5970ed9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075634"
---
# <a name="itemaddress-resource-type"></a>tipo de recurso de endereço

Namespace: microsoft.graph

Representa um endereço físico e detalhes do local onde o endereço é encontrado.

Herda de [Myfacet](../resources/itemfacet.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar endereços](../api/profile-list-addresses.md)|coleção [myAddress](../resources/itemaddress.md)|Obtenha os recursos de endereço da propriedade de navegação addresses.|
|[Criar endereço](../api/profile-post-addresses.md)|[Endereço do destinatário](../resources/itemaddress.md)|Criar um novo objeto de endereço.|
|[Get endereço](../api/itemaddress-get.md)|[Endereço do destinatário](../resources/itemaddress.md)|Leia as propriedades e os relacionamentos de [um objeto](../resources/itemaddress.md) item.|
|[Atualizar endereço](../api/itemaddress-update.md)|[Endereço do destinatário](../resources/itemaddress.md)|Atualizar as propriedades [de um objeto](../resources/itemaddress.md) item.|
|[Excluir endereço](../api/itemaddress-delete.md)|Nenhum|Exclui um objeto [myAddress](../resources/itemaddress.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|Cadeia de caracteres|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|detalhada|[physicalAddress](../resources/physicaladdress.md)|Detalhes sobre o próprio endereço.|
|displayName|Cadeia de caracteres|Nome amigável que o usuário atribuiu a este endereço. |
|geoCoordinates|[geoCoordinates](../resources/geocoordinates.md)|As geocoordenas do endereço.|
|id|Cadeia de caracteres|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|

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


