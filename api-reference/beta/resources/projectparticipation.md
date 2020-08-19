---
title: tipo de recurso projectParticipation
description: tipo de recurso projectParticipation
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 535564d3b35bbccb47c54a78fe4b508a6d6a2963
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812019"
---
# <a name="projectparticipation-resource-type"></a>tipo de recurso projectParticipation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre os projetos associados a um usuário.

Herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar projetos](../api/profile-list-projects.md)|coleção [projectParticipation](../resources/projectparticipation.md)|Obtenha os recursos projectParticipation da propriedade de navegação Projects.|
|[Criar projectParticipation](../api/profile-post-projects.md)|[projectParticipation](../resources/projectparticipation.md)|Criar um novo objeto projectParticipation.|
|[Obter projectParticipation](../api/projectparticipation-get.md)|[projectParticipation](../resources/projectparticipation.md)|Leia as propriedades e os relacionamentos de um objeto [projectParticipation](../resources/projectparticipation.md) .|
|[Atualizar projectParticipation](../api/projectparticipation-update.md)|[projectParticipation](../resources/projectparticipation.md)|Atualiza as propriedades de um objeto [projectParticipation](../resources/projectparticipation.md) .|
|[Excluir projectParticipation](../api/projectparticipation-delete.md)|Nenhum|Exclui um objeto [projectParticipation](../resources/projectparticipation.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Coleção de cadeias de caracteres|Contém categorias que um usuário associou ao projeto (por exemplo, transformação digital, Rig óleo). |
|clientes|[companyDetail](../resources/companydetail.md)|Contém informações detalhadas sobre o cliente para o qual o projeto foi. |
|collaborationTags|Coleção de cadeia de caracteres|Contém marcas de cenário de experiência que um usuário associou aos juros. Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` , `wantsToImprove` .|
|conhecidos|coleção [relatedPerson](../resources/relatedperson.md)|Lista as pessoas que também trabalharam no projeto. |
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|detalhada|[positionDetail](../resources/positiondetail.md)|Contém detalhes sobre a função do usuário no projeto.|
|displayName|String|Contém um nome amigável para o projeto.|
|id|String|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|responsáveis|coleção [relatedPerson](../resources/relatedperson.md)|A pessoa ou as pessoas que patrocinaram o projeto.    |
## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.projectParticipation",
  "baseType": ""
}-->

```json
{
  "@odata.type": "#microsoft.graph.projectParticipation",
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
  "client": {
    "@odata.type": "microsoft.graph.companyDetail"
  },
  "displayName": "String",
  "detail": {
    "@odata.type": "microsoft.graph.positionDetail"
  },
  "colleagues": [
    {
      "@odata.type": "microsoft.graph.relatedPerson"
    }
  ],
  "sponsors": [
    {
      "@odata.type": "microsoft.graph.relatedPerson"
    }
  ],
  "collaborationTags": [
    "String"
  ]
}
```
