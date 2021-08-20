---
title: tipo de recurso itemPublication
description: tipo de recurso itemPublication
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 5cdc4a741205be696e584100d1ce6900052a951354481cc0dceffb7d1e19464b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54248283"
---
# <a name="itempublication-resource-type"></a>tipo de recurso itemPublication

Namespace: microsoft.graph

Representa uma publicação ou artigo que foi associado ao perfil de um [usuário.](../resources/profile.md)

Herda do [itemFacet](../resources/itemfacet.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar publicações](../api/profile-list-publications.md)|[coleção itemPublication](../resources/itempublication.md)|Obter os recursos itemPublication da propriedade de navegação de publicações.|
|[Criar itemPublication](../api/profile-post-publications.md)|[itemPublication](../resources/itempublication.md)|Crie um novo objeto itemPublication.|
|[Obter itemPublication](../api/itempublication-get.md)|[itemPublication](../resources/itempublication.md)|Leia as propriedades e as relações de um [objeto itemPublication.](../resources/itempublication.md)|
|[Atualizar itemPublication](../api/itempublication-update.md)|[itemPublication](../resources/itempublication.md)|Atualize as propriedades de um [objeto itemPublication.](../resources/itempublication.md)|
|[Excluir itemPublication](../api/itempublication-delete.md)|Nenhum|Exclui um [objeto itemPublication.](../resources/itempublication.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|Cadeia de caracteres|As audiências que são capazes de ver os valores contidos na entidade. Herdado [do itemFacet](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado [do itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|description    |Cadeia de caracteres      |Descrição da publicação.                   |
|displayName    |Cadeia de caracteres      |Título da publicação.                         |
|id|Cadeia de caracteres|Identificador usado para endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|inferência|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado [do itemFacet](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado [do itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|publishedDate  |Data        |A data em que a publicação foi publicada.      |
|publicador      |String      |Publicação ou editor para a publicação.     |
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores se originaram se sincronizados de outro serviço. Herdado [do itemFacet](../resources/itemfacet.md).|
|thumbnailUrl   |Cadeia de caracteres      |URL fazendo referência a uma miniatura da publicação.   |
|webUrl         |String      |URL fazendo referência à publicação.                  |

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


