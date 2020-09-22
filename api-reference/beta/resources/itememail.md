---
title: tipo de recurso de email
description: tipo de recurso de email
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2dbf1f3f2c90cf7562d034e32f8fa03d1590ee42
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021480"
---
# <a name="itememail-resource-type"></a>tipo de recurso de email

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre endereços de email associados ao usuário.

Herda de [Myfacet](../resources/itemfacet.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar emails](../api/profile-list-emails.md)|coleção [email](../resources/itememail.md)|Obtenha os recursos de email da propriedade de navegação emails.|
|[Criar email](../api/profile-post-emails.md)|[Email](../resources/itememail.md)|Criar um novo objeto de email.|
|[Obter email](../api/itememail-get.md)|[Email](../resources/itememail.md)|Leia as propriedades e os relacionamentos de um objeto item de [email](../resources/itememail.md) .|
|[Atualizar email](../api/itememail-update.md)|[Email](../resources/itememail.md)|Atualiza as propriedades de um objeto item de [email](../resources/itememail.md) .|
|[Excluir email](../api/itememail-delete.md)|Nenhum|Exclui um objeto [MyEmail](../resources/itememail.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|address|Cadeia de caracteres|O próprio endereço de email.|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|displayName|String|O nome ou rótulo que um usuário associou a um endereço de email específico.|
|id|String|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|tipo|emailtype|O tipo de endereço de email. Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemEmail",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemEmail",
  "id": "0f30bf5d-bf5d-0f30-5dbf-300f5dbf300f",
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
  "address": "String",
  "displayName": "String",
  "type": "String"
}
```


