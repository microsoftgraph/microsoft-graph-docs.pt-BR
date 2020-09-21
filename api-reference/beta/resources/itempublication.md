---
title: tipo de recurso de multipúblico
description: tipo de recurso de multipúblico
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 59b30c08e78db52af9e10c6aac2550dc02c11e62
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083999"
---
# <a name="itempublication-resource-type"></a>tipo de recurso de multipúblico

Namespace: microsoft.graph

Representa uma publicação ou um artigo que tenha sido associado ao [perfil](../resources/profile.md)de um usuário.

Herda de [Myfacet](../resources/itemfacet.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar publicações](../api/profile-list-publications.md)|coleção de [Multipúblico](../resources/itempublication.md)|Obtenha os recursos de publicação da propriedade de navegação publicações.|
|[Criar a multipúblico](../api/profile-post-publications.md)|[multipúblico](../resources/itempublication.md)|Criar um novo objeto dopublication.|
|[Obter o multipúblico](../api/itempublication-get.md)|[multipúblico](../resources/itempublication.md)|Leia as propriedades e os relacionamentos de um objeto de [Ispublication](../resources/itempublication.md) .|
|[Atualizar a multipública](../api/itempublication-update.md)|[multipúblico](../resources/itempublication.md)|Atualizar as propriedades de um objeto de [multipúblico](../resources/itempublication.md) .|
|[Excluir a multipúblico](../api/itempublication-delete.md)|Nenhum|Exclui um objeto [Dopublication](../resources/itempublication.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|Cadeia de caracteres|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|description    |Cadeia de caracteres      |Descrição da publicação.                   |
|displayName    |Cadeia de caracteres      |Título da publicação.                         |
|id|Cadeia de caracteres|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|publishedDate  |Data        |A data em que a publicação foi publicada.      |
|publicador      |String      |Publicação ou editor para a publicação.     |
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|thumbnailUrl   |Cadeia de caracteres      |URL que faz referência a uma miniatura da publicação.   |
|webUrl         |String      |URL que faz referência à publicação.                  |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemPublication",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemPublication",
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
  "publishedDate": "Date",
  "publisher": "String",
  "thumbnailUrl": "String",
  "webUrl": "String"
}
```


