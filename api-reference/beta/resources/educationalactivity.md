---
title: tipo de recurso educationalActivity
description: tipo de recurso educationalActivity
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 5f920b2afbb319af923212563aac6e8ea163c9de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055677"
---
# <a name="educationalactivity-resource-type"></a>tipo de recurso educationalActivity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os dados que um usuário forneceu relacionados ao Undergraduate, graduado, dograduação ou outras atividades educacionais.

Herda as propriedades de metadados de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar educationalActivities](../api/profile-list-educationalactivities.md)|coleção [educationalActivity](../resources/educationalactivity.md)|Obtenha os recursos educationalActivity da propriedade de navegação educationalActivities.|
|[Criar educationalActivity ](../api/profile-post-educationalactivities.md)|[educationalActivity](../resources/educationalactivity.md)|Criar um novo objeto educationalActivity.|
|[Obter educationalActivity](../api/educationalactivity-get.md)|[educationalActivity](../resources/educationalactivity.md)|Leia as propriedades e os relacionamentos de um objeto [educationalActivity](../resources/educationalactivity.md) .|
|[Atualizar educationalActivity](../api/educationalactivity-update.md)|[educationalActivity](../resources/educationalactivity.md)|Atualiza as propriedades de um objeto [educationalActivity](../resources/educationalactivity.md) .|
|[Excluir educationalActivity](../api/educationalactivity-delete.md)|Nenhum|Exclui um objeto [educationalActivity](../resources/educationalactivity.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|Cadeia de caracteres|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|completionMonthYear|Data|O mês e o ano em que o usuário formou ou concluiu a atividade. |
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|endMonthYear|Data|O mês e o ano em que o usuário concluiu a atividade educacional referenciada.|
|id|Cadeia de caracteres|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|instituição|[institutionData](../resources/institutiondata.md)|Contém detalhes da instituição estudada em. |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|programa|[educationalActivityDetail](../resources/educationalactivitydetail.md)|Contém informações estendidas sobre o programa ou o curso.|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|startMonthYear|Data|O mês e o ano em que o usuário tiver iniciado a atividade referenciada.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationalActivity",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationalActivity",
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
  "completionMonthYear": "Date",
  "endMonthYear": "Date",
  "institution": {
    "@odata.type": "microsoft.graph.institutionData"
  },
  "program": {
    "@odata.type": "microsoft.graph.educationalActivityDetail"
  },
  "startMonthYear": "Date"
}
```

