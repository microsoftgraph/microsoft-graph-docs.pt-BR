---
title: Tipo de recurso subjectRightsRequest
description: Representa as propriedades de uma solicitação de direitos de entidade.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f59c1306bea22b0da7e59024600017e73dfa8eff
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461433"
---
# <a name="subjectrightsrequest-resource-type"></a>Tipo de recurso subjectRightsRequest

Namespace: microsoft.graph

Representa as propriedades de uma solicitação de direitos de entidade, que é uma solicitação formal de um titular dos dados a um controlador para executar uma ação em seus dados pessoais. 

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar subjectRightsRequests](../api/subjectRightsRequest-list.md)|[coleção subjectRightsRequest](../resources/subjectRightsRequest.md)|Obtenha uma lista dos [objetos subjectRightsRequest](../resources/subjectRightsRequest.md) e suas propriedades.|
|[Criar subjectRightsRequest](../api/subjectRightsRequest-post.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|Crie um novo [objeto subjectRightsRequest](../resources/subjectRightsRequest.md) .|
|[Obter subjectRightsRequest](../api/subjectRightsRequest-get.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|Leia as propriedades e as relações de um [objeto subjectRightsRequest](../resources/subjectRightsRequest.md) .|
|[Atualizar subjectRightsRequest](../api/subjectRightsRequest-update.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|Atualize as propriedades de um [objeto subjectRightsRequest](../resources/subjectRightsRequest.md) .|
|[getFinalAttachment](../api/subjectRightsRequest-getfinalattachment.md)|Stream|Obtenha o anexo final da solicitação. O anexo é um arquivo zip que contém todos os arquivos incluídos pelo administrador de privacidade.|
|[getFinalReport](../api/subjectRightsRequest-getfinalreport.md)|Stream|Obtenha o relatório final para a solicitação. O relatório é um arquivo de texto que contém informações sobre os arquivos incluídos pelo administrador de privacidade.|
|[Listar anotações](../api/subjectRightsRequest-list-notes.md)|[coleção authoredNote](../resources/authorednote.md)|Obtenha os recursos authoredNote da propriedade de navegação de anotações.|
|[Criar authoredNote](../api/subjectRightsRequest-post-notes.md)|[authoredNote](../resources/authorednote.md)|Crie um novo objeto authoredNote.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignedTo|[identity](../resources/identity.md)|Identidade à qual a solicitação é atribuída.|
|closedDateTime|DateTimeOffset|A data e a hora em que a solicitação foi fechada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|createdBy|[identitySet](../resources/identityset.md)|Informações de identidade para a entidade que criou a solicitação.|
|createdDateTime|DateTimeOffset|A data e a hora em que a solicitação foi criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
|dataSubject|[dataSubject](../resources/datasubject.md)|Informações sobre o titular dos dados.|
|dataSubjectType|dataSubjectType|O tipo do titular dos dados. Os valores possíveis são: `customer`, `currentEmployee`, `formerEmployee`, `prospectiveEmployee`, `student`, `teacher`, `faculty`, `other`, `unknownFutureValue`.|
|description|String|Descrição da solicitação.|
|displayName|String|O nome da solicitação.|
|História|[coleção subjectRightsRequestHistory](../resources/subjectRightsRequesthistory.md)|Coleção de eventos de alteração de histórico.|
|insight|[subjectRightsRequestDetail](../resources/subjectRightsRequestdetail.md)|Insight sobre a solicitação.|
|internalDueDateTime|DateTimeOffset|A data e a hora em que a solicitação é concluída internamente. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Informações de identidade para a entidade que modificou a solicitação pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a solicitação foi modificada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|Regulamentos|Coleção String|Lista de regulamentos que essa solicitação atenderá.|
|Estágios|[coleção subjectRightsRequestStageDetail](../resources/subjectRightsRequeststagedetail.md)|Informações sobre os diferentes estágios da solicitação.|
|status|subjectRightsRequestStatus|O status da solicitação.. Os valores possíveis são: `active`, `closed`, `unknownFutureValue`.|
|type|subjectRightsRequestType|O tipo da solicitação. Os valores possíveis são: `export`, `delete`,  `access`, `tagForAction`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|notes|[coleção authoredNote](../resources/authorednote.md)|Lista de anotações associadas à solicitação.|
|team|[equipe](../resources/team.md)|Informações sobre a Microsoft Teams que foi criada para a solicitação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subjectRightsRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequest",
    "type": "access",
    "dataSubjectType": "customer",
    "regulations": [
        "String"
    ],
    "displayName": "String",
    "description": "String",
    "status": "active",
    "internalDueDateTime": "String (timestamp)",
    "closedDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)",
    "id": "String (identifier)",
    "createdDateTime": "String (timestamp)",
    "stages": [
        {
            "stage": "contentRetrieval",
            "status": "completed",
            "error": 
            {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "contentReview",
            "status": "current",
            "error": 
            {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "generateReport",
            "status": "notStarted",
            "error": 
            {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "caseResolved",
            "status": "notStarted",
            "error": 
            {
                "@odata.type": "microsoft.graph.publicError"
            }
        }
    ],
    "insight": {
        "@odata.type": "microsoft.graph.subjectRightsRequestDetail"
    },
    "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "dataSubject": {
        "@odata.type": "microsoft.graph.dataSubject",
    },
    "team": {
        "@odata.type": "microsoft.graph.team"
    }
}
```

