---
title: Tipo de recurso projectParticipation
description: Tipo de recurso projectParticipation
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1d349b33dc3325451e97d055c178082676b48de3
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156361"
---
# <a name="projectparticipation-resource-type"></a>Tipo de recurso projectParticipation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre projetos associados a um usuário.

Herda de [itemFacet](itemfacet.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar projetos](../api/profile-list-projects.md)|[coleção projectParticipation](../resources/projectparticipation.md)|Obter os recursos projectParticipation da propriedade de navegação de projetos.|
|[Criar projectParticipation](../api/profile-post-projects.md)|[projectParticipation](../resources/projectparticipation.md)|Criar um novo objeto projectParticipation.|
|[Obter projectParticipation](../api/projectparticipation-get.md)|[projectParticipation](../resources/projectparticipation.md)|Leia as propriedades e os relacionamentos de um [objeto projectParticipation.](../resources/projectparticipation.md)|
|[Atualizar projectParticipation](../api/projectparticipation-update.md)|[projectParticipation](../resources/projectparticipation.md)|Atualizar as propriedades de um [objeto projectParticipation.](../resources/projectparticipation.md)|
|[Excluir projectParticipation](../api/projectparticipation-delete.md)|Nenhum(a)|Exclui um [objeto projectParticipation.](../resources/projectparticipation.md)|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [itemFacet](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Coleção de cadeias de caracteres|Contém categorias que um usuário associou ao projeto (por exemplo, transformação digital, equipamento de petróleo). |
|client|[companyDetail](../resources/companydetail.md)|Contém informações detalhadas sobre o cliente do projeto. |
|collaborationTags|Coleção de cadeias de caracteres|Contém marcas de cenário de experiência que um usuário associou ao interesse. Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` `wantsToImprove` .|
|colleagues|[coleção relatedPerson](../resources/relatedperson.md)|Lista as pessoas que também trabalharam no projeto. |
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece a dateTimeOffset para quando a entidade foi criada. Herdado de [itemFacet](../resources/itemfacet.md).|
|detalhe|[positionDetail](../resources/positiondetail.md)|Contém detalhes sobre a função do usuário no projeto.|
|displayName|String|Contém um nome amigável para o projeto.|
|id|String|Identificador usado para endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|inferência|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pela criação ou modificação do aplicativo. Herdado de [itemFacet](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece a dateTimeOffset para quando a entidade foi criada. Herdado de [itemFacet](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores se originaram se sincronizados de outro serviço. Herdado de [itemFacet](../resources/itemfacet.md).|
|patrocinadores|[coleção relatedPerson](../resources/relatedperson.md)|A pessoa ou as pessoas que patrocinaram o projeto.    |
## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.projectParticipation"
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


