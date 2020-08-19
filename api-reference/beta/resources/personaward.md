---
title: tipo de recurso personAward
description: tipo de recurso personAward
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 3031994e3b19fdd3962118c21d86a334c63781ea
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812895"
---
# <a name="personaward-resource-type"></a>tipo de recurso personAward

Namespace: microsoft.graph

Representa um prêmio que foi associado ao [perfil](../resources/profile.md)de um usuário.

Herda de [Myfacet](../resources/itemfacet.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar prêmios](../api/profile-list-awards.md)|coleção [personAward](../resources/personaward.md)|Obtenha os recursos personAward da propriedade de navegação Awards.|
|[Criar personAward](../api/profile-post-awards.md)|[personAward](../resources/personaward.md)|Criar um novo objeto personAward.|
|[Obter personAward](../api/personaward-get.md)|[personAward](../resources/personaward.md)|Leia as propriedades e os relacionamentos de um objeto [personAward](../resources/personaward.md) .|
|[Atualizar personAward](../api/personaward-update.md)|[personAward](../resources/personaward.md)|Atualiza as propriedades de um objeto [personAward](../resources/personaward.md) .|
|[Excluir personAward](../api/personaward-delete.md)|Nenhum|Exclui um objeto [personAward](../resources/personaward.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|description|String|Descpription do prêmio ou honra. |
|displayName|String|Nome do prêmio ou honra. |
|id|String|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|issuedDate|Data|A data em que o prêmio ou honra foi concedido. |
|issuingAuthority|String|Autoridade que concedeu o prêmio ou honra.  |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|thumbnailUrl|String|URL que faz referência a uma miniatura do prêmio ou honra.  |
|webUrl|String|URL que faz referência ao prêmio ou honra. |

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
