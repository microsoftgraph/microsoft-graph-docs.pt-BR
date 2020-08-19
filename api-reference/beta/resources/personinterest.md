---
title: tipo de recurso personInterest
description: tipo de recurso personInterest
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: beecb5fa65609196fd4514d097d97b6f64fcdb4c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812040"
---
# <a name="personinterest-resource-type"></a>tipo de recurso personInterest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece informações detalhadas sobre os interesses que o usuário tenha associado a si mesmos em vários serviços.

Herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos

| Método                                                    | Tipo de retorno                         | Descrição                                                           |
|:----------------------------------------------------------|:------------------------------------|:----------------------------------------------------------------------|
|[Listar interesses](../api/profile-list-interests.md)|coleção [personInterest](../resources/personinterest.md)|Obtenha os recursos personInterest da propriedade de navegação interesses.|
|[Criar personInterest](../api/profile-post-interests.md)|[personInterest](../resources/personinterest.md)|Criar um novo objeto personInterest.|
|[Obter personInterest](../api/personinterest-get.md)|[personInterest](../resources/personinterest.md)|Leia as propriedades e os relacionamentos de um objeto [personInterest](../resources/personinterest.md) .|
|[Atualizar personInterest](../api/personinterest-update.md)|[personInterest](../resources/personinterest.md)|Atualiza as propriedades de um objeto [personInterest](../resources/personinterest.md) .|
|[Excluir personInterest](../api/personinterest-delete.md)|Nenhum|Exclui um objeto [personInterest](../resources/personinterest.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Coleção de cadeias de caracteres|Contém categorias que um usuário associou aos juros (por exemplo, pessoal, recipies). |
|collaborationTags|Coleção de cadeia de caracteres|Contém marcas de cenário de experiência que um usuário associou aos juros. Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` , `wantsToImprove` .|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|description|String|Contém uma descrição dos juros.|
|displayName|String|Contém um nome amigável para os juros.  |
|id|String|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|webUrl|String|Contém um link para uma página da Web ou recurso sobre os juros. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personInterest",
  "baseType": ""
}-->

```json
{
  "@odata.type": "#microsoft.graph.personInterest",
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
  "description": "String",
  "displayName": "String",
  "webUrl": "String",
  "collaborationTags": [
    "String"
  ]
}
```
