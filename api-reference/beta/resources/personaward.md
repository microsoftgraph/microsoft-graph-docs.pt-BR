---
title: Tipo de recurso personAward
description: Tipo de recurso personAward
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 4af72499276b6eb4e90333243462e94f0cfa02b92aa014cbcdc59e1a111d1afa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251047"
---
# <a name="personaward-resource-type"></a>Tipo de recurso personAward

Namespace: microsoft.graph

Representa um prêmio associado ao perfil de um [usuário.](../resources/profile.md)

Herda do [itemFacet](../resources/itemfacet.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List awards](../api/profile-list-awards.md)|[Coleção personAward](../resources/personaward.md)|Obter os recursos personAward da propriedade de navegação de prêmio.|
|[Criar personAward](../api/profile-post-awards.md)|[personAward](../resources/personaward.md)|Crie um novo objeto personAward.|
|[Obter personAward](../api/personaward-get.md)|[personAward](../resources/personaward.md)|Leia as propriedades e as relações de um [objeto personAward.](../resources/personaward.md)|
|[Atualizar personAward](../api/personaward-update.md)|[personAward](../resources/personaward.md)|Atualize as propriedades de [um objeto personAward.](../resources/personaward.md)|
|[Excluir personAward](../api/personaward-delete.md)|Nenhum|Exclui um [objeto personAward.](../resources/personaward.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|Cadeia de caracteres|As audiências que são capazes de ver os valores contidos na entidade. Herdado [do itemFacet](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado [do itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|description|Cadeia de caracteres|Descpription of the award or honor. |
|displayName|Cadeia de caracteres|Nome do prêmio ou da honra. |
|id|Cadeia de caracteres|Identificador usado para endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|inferência|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado [do itemFacet](../resources/itemfacet.md).|
|issuedDate|Data|A data em que o prêmio ou a honra foi concedido. |
|issuingAuthority|Cadeia de caracteres|Autoridade que concedeu o prêmio ou a honra.  |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado [do itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores se originaram se sincronizados de outro serviço. Herdado [do itemFacet](../resources/itemfacet.md).|
|thumbnailUrl|Cadeia de caracteres|URL fazendo referência a uma miniatura do prêmio ou da honra.  |
|webUrl|String|URL referenciando o prêmio ou a honra. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personAward",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAward",
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
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "thumbnailUrl": "String",
  "webUrl": "String"
}
```


