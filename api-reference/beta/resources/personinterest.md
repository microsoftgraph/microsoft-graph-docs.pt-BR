---
title: Tipo de recurso personInterest
description: Tipo de recurso personInterest
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0b635ab19f4cda9985de05e317316579ad60f7b1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161394"
---
# <a name="personinterest-resource-type"></a>Tipo de recurso personInterest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece informações detalhadas sobre os interesses que o usuário associou a si mesmo em vários serviços.

Herda de [itemFacet](itemfacet.md).

## <a name="methods"></a>Métodos

| Método                                                    | Tipo de retorno                         | Descrição                                                           |
|:----------------------------------------------------------|:------------------------------------|:----------------------------------------------------------------------|
|[Listar interesses](../api/profile-list-interests.md)|[Coleção personInterest](../resources/personinterest.md)|Obter os recursos personInterest da propriedade de navegação de interesses.|
|[Criar personInterest](../api/profile-post-interests.md)|[personInterest](../resources/personinterest.md)|Crie um novo objeto personInterest.|
|[Obter personInterest](../api/personinterest-get.md)|[personInterest](../resources/personinterest.md)|Leia as propriedades e os relacionamentos de um [objeto personInterest.](../resources/personinterest.md)|
|[Atualizar personInterest](../api/personinterest-update.md)|[personInterest](../resources/personinterest.md)|Atualizar as propriedades de um [objeto personInterest.](../resources/personinterest.md)|
|[Excluir personInterest](../api/personinterest-delete.md)|Nenhum(a)|Exclui um [objeto personInterest.](../resources/personinterest.md)|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [itemFacet](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Coleção de cadeias de caracteres|Contém categorias que um usuário associou ao interesse (por exemplo, pessoais, recipies). |
|collaborationTags|Coleção de cadeias de caracteres|Contém marcas de cenário de experiência que um usuário associou ao interesse. Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` `wantsToImprove` .|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece a dateTimeOffset para quando a entidade foi criada. Herdado de [itemFacet](../resources/itemfacet.md).|
|description|String|Contém uma descrição do interesse.|
|displayName|String|Contém um nome amigável para o interesse.  |
|id|String|Identificador usado para endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|inferência|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pela criação ou modificação do aplicativo. Herdado de [itemFacet](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece a dateTimeOffset para quando a entidade foi criada. Herdado de [itemFacet](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores se originaram se sincronizados de outro serviço. Herdado de [itemFacet](../resources/itemfacet.md).|
|webUrl|String|Contém um link para uma página da Web ou um recurso sobre o interesse. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personInterest"
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


