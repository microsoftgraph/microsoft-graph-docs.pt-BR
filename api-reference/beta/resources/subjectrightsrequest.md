---
title: Tipo de recurso subjectRightsRequest
description: Representa as propriedades de uma solicitação de direitos de entidade.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: b601530b71f8af9b84e1bf94b19b3b3332b12f21
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461230"
---
# <a name="subjectrightsrequest-resource-type"></a>Tipo de recurso subjectRightsRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| contentQuery         | String | KQL consulta de conteúdo baseada em conteúdo que deve ser usada para pesquisa. Essa propriedade é definida somente para APIs acessadas usando `\security` o caminho de consulta e não o `\privacy` caminho da consulta.|
|createdBy|[identitySet](../resources/identityset.md)|Informações de identidade para a entidade que criou a solicitação.|
|createdDateTime|DateTimeOffset|A data e a hora em que a solicitação foi criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
|dataSubject|[dataSubject](../resources/datasubject.md)|Informações sobre o titular dos dados.|
|dataSubjectType|dataSubjectType|O tipo do titular dos dados. Os valores possíveis são: `customer`, `currentEmployee`, `formerEmployee`, `prospectiveEmployee`, `student`, `teacher`, `faculty`, `other`, `unknownFutureValue`.|
|description|String|Descrição da solicitação.|
|displayName|String|O nome da solicitação.|
| externalId           | Cadeia de caracteres| A ID externa da solicitação que é imutável após a criação e é usada para acompanhar a solicitação para o sistema externo. Essa propriedade é definida somente para APIs acessadas usando `\security` o caminho de consulta e não o `\privacy` caminho da consulta.|
|História|[coleção subjectRightsRequestHistory](../resources/subjectrightsrequesthistory.md)|Coleção de eventos de alteração de histórico.|
| includeAllVersions   | Booliano | Inclua todas as versões dos documentos. Por padrão, as cópias atuais dos documentos serão retornadas. Se SharePoint sites tiverem o controle de versão habilitado, incluir todas as versões incluirá as cópias históricas dos documentos. Essa propriedade é definida somente para APIs acessadas usando `\security` o caminho de consulta e não o `\privacy` caminho da consulta.|
| includeAuthoredContent| Booliano | Inclua o conteúdo criado pelo titular dos dados. Essa propriedade é definida somente para APIs acessadas usando `\security` o caminho de consulta e não o `\privacy` caminho da consulta.|
|insight|[subjectRightsRequestDetail](../resources/subjectrightsrequestdetail.md)|Insight sobre a solicitação.|
|internalDueDateTime|DateTimeOffset|A data e a hora em que a solicitação é concluída internamente. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Informações de identidade para a entidade que modificou a solicitação pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a solicitação foi modificada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
| mailboxLocations     | [subjectRightsRequestMailboxLocation](../resources/subjectrightsrequestmailboxlocation.md)|Os locais de caixa de correio que devem ser pesquisados. Essa propriedade é definida somente para APIs acessadas usando `\security` o caminho de consulta e não o `\privacy` caminho da consulta.|
| pauseAfterEstimate   | Booliano| Pause a solicitação após a conclusão da estimativa. Por padrão, a estimativa de dados será executada e pausada, permitindo que você visualize os resultados e selecione a opção para recuperar dados na interface do usuário. Você pode definir essa propriedade como `false` se quiser que ela execute a estimativa e comece automaticamente com a recuperação do conteúdo. Essa propriedade é definida somente para APIs acessadas usando `\security` o caminho de consulta e não o `\privacy` caminho da consulta.|
|Regulamentos|Coleção de cadeias de caracteres|Lista de regulamentos que essa solicitação atenderá.|
| siteLocations| [subjectRightsRequestSiteLocation](../resources/subjectrightsrequestsitelocation.md)| Os SharePoint e OneDrive locais do site que devem ser pesquisados. Essa propriedade é definida somente para APIs acessadas usando `\security` o caminho de consulta e não o `\privacy` caminho da consulta.|
|Estágios|[coleção subjectRightsRequestStageDetail](../resources/subjectrightsrequeststagedetail.md)|Informações sobre os diferentes estágios da solicitação.|
|status|subjectRightsRequestStatus|O status da solicitação. Os valores possíveis são: `active`, `closed`, `unknownFutureValue`.|
|type|subjectRightsRequestType|O tipo da solicitação. Os valores possíveis são: `export`, `delete`, `access`, `tagForAction`, `unknownFutureValue`.|

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
    "contentQuery": "String",
    "closedDateTime": "String (timestamp)",
    "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "createdDateTime": "String (timestamp)",
    "dataSubject": {
        "@odata.type": "microsoft.graph.dataSubject"
    },
    "dataSubjectType": "customer",
    "description": "String",
    "displayName": "String",
    "externalId": "String",
    "id": "String (identifier)",
    "includeAllVersions": "Boolean",
    "includeAuthoredContent": "Boolean",
    "insight": {
        "@odata.type": "microsoft.graph.subjectRightsRequestDetail"
    },
    "internalDueDateTime": "String (timestamp)",
    "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "mailboxLocations": {
        "@odata.type": "microsoft.graph.subjectRightsRequestMailboxLocation"
    },
    "pauseAfterDownload": "Boolean",
    "regulations": [
        "String"
    ],
    "stages": [
        {
            "stage": "contentRetrieval",
            "status": "completed",
            "error": {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "contentReview",
            "status": "current",
            "error": {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "generateReport",
            "status": "notStarted",
            "error": {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "caseResolved",
            "status": "notStarted",
            "error": {
                "@odata.type": "microsoft.graph.publicError"
            }
        }
    ],
    "siteLocations": {
        "@odata.type": "microsoft.graph.subjectRightsRequestSiteLocation"
    },
    "status": "active",
    "team": {
        "@odata.type": "microsoft.graph.team"
    },
    "type": "access"
}
```

