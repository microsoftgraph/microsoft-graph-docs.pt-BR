---
title: tipo de recurso skillProficiency
description: tipo de recurso skillProficiency
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: d01c9fe6c4171c16d96e5b81eb8537ea0cbeb1a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997673"
---
# <a name="skillproficiency-resource-type"></a>tipo de recurso skillProficiency

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre as habilidades associadas a um usuário em vários serviços.

Herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Methods
 
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar qualificações](../api/profile-list-skills.md)|coleção [skillProficiency](../resources/skillproficiency.md)|Obtenha os recursos skillProficiency da propriedade de navegação de habilidades.|
|[Criar skillProficiency ](../api/profile-post-skills.md)|[skillProficiency](../resources/skillproficiency.md)|Criar um novo objeto skillProficiency.|
|[Obter skillProficiency](../api/skillproficiency-get.md)|[skillProficiency](../resources/skillproficiency.md)|Leia as propriedades e os relacionamentos de um objeto [skillProficiency](../resources/skillproficiency.md) .|
|[Atualizar skillProficiency](../api/skillproficiency-update.md)|[skillProficiency](../resources/skillproficiency.md)|Atualiza as propriedades de um objeto [skillProficiency](../resources/skillproficiency.md) .|
|[Excluir skillProficiency](../api/skillproficiency-delete.md)|Nenhum|Exclui um objeto [skillProficiency](../resources/skillproficiency.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|Categorias|Coleção de cadeias de caracteres|Contém categorias que um usuário associou à habilidade (por exemplo, pessoal, profissional, hobby). |
|collaborationTags|Coleção de cadeias de caracteres|Contém marcas de cenário de experiência que um usuário associou aos juros. Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` , `wantsToImprove` .|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|displayName|String|Contém um nome amigável para a habilidade. |
|id|String|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|proficiência|skillProficiencyLevel|Detalhes da proficiência dos usuários com esta habilidade. Os possíveis valores são: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|webUrl|String|Contém um link para uma fonte de informações sobre a habilidade. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skillProficiency",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skillProficiency",
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
  "categories": [
    "String"
  ],
  "displayName": "String",
  "proficiency": "String",
  "webUrl": "String",
  "collaborationTags": [
    "String"
  ]
}
```

