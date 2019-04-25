---
title: tipo de recurso educationSubmission
description: Os envios são propriedade de uma atribuição. Um envio representa os recursos que um indivíduo (ou grupo) liga para uma atribuição e a grade/comentários que é retornado.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: aeeb1355da2ffcb0ebf561af2ecd15ac93221e26
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542887"
---
# <a name="educationsubmission-resource-type"></a>tipo de recurso educationSubmission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os envios são propriedade de uma atribuição. Um envio representa os recursos que um indivíduo (ou grupo) liga para uma atribuição e a grade/comentários que é retornado.
Os envios são criados automaticamente quando uma atribuição é publicada. O envio possui duas listas de recursos. Os recursos representam a área de trabalho usuários/grupos enquanto os recursos enviados representam os recursos que foram ativamente ativados pelos alunos.  

>**Observação:** O status é somente leitura e o objeto é movido através do fluxo de trabalho via ações. 

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter educationSubmission](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |Ler propriedades e relações de um objeto **educationSubmission** .|
|[Listar recursos](../api/educationsubmission-list-resources.md) |coleção [educationSubmissionResource](educationsubmissionresource.md)| Obtenha uma coleção de objetos **educationSubmissionResource** .|
|[Listar submittedResources](../api/educationsubmission-list-submittedresources.md) |coleção [educationSubmissionResource](educationsubmissionresource.md)| Obtenha uma coleção de objetos **educationSubmissionResource** .|
|[Update](../api/educationsubmission-update.md) | [educationSubmission](educationsubmission.md) |Atualize um objeto **educationSubmission** . |
|[Enter](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|Um professor usa Return para indicar que os notas/comentários podem ser mostrados para o aluno.|
|[Enviar](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|Um aluno usa Submit para ativar a atribuição. Isso copiará os recursos na pasta **submittedResources** para a gradação e atualizará o status.|
|[Não enviar](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|Um aluno usa o não enviar para mover o estado do envio de enviado de volta para o trabalho. Isso copiará os recursos na pasta **workingResources** para a gradação e atualizará o status.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|comentários|[educationFeedback](educationfeedback.md)|Retém a propriedade feedback que armazena as notas do professor de volta para os alunos.|
|grade|[educationAssignmentGrade](educationassignmentgrade.md)|Contém as informações de nota que um professor atribui a esse envio.|
|id|String| Somente leitura.|
|destinatário|[educationSubmissionRecipient](educationsubmissionrecipient.md)|A quem esse envio é atribuído.|
|releasedBy|[identitySet](identityset.md)|Usuário que moveu o status desse envio para liberado.|
|releasedDateTime|DateTimeOffset|Momento no momento em que o envio foi lançado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|returnedBy|[identitySet](identityset.md)|Usuário que moveu o status desse envio para o retornado.|
|returnedDateTime|DateTimeOffset|Momento no momento em que o envio foi retornado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|resourcesFolderUrl|String|Pasta onde todos os recursos de arquivo para esse envio precisam ser armazenados.|
|status|cadeia de caracteres| Somente Leitura. Os valores possíveis são: `working`, `submitted`, `released`, `returned`.|
|submittedBy|[identitySet](identityset.md)|Usuário que moveu o recurso para o estado enviado.|
|submittedDateTime|DateTimeOffset|Momento no momento em que o envio foi movido para o estado enviado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|unsubmittedBy|[identitySet](identityset.md)|Usuário que moveu o recurso de enviado para o estado de trabalho.|
|unsubmittedDateTime|DateTimeOffset|Momento no momento em que o envio foi movido de enviado para o estado de trabalho. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recursos|coleção [educationSubmissionResource](educationsubmissionresource.md)| Anulável.|
|submittedResources|coleção [educationSubmissionResource](educationsubmissionresource.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "grade": {"@odata.type": "microsoft.graph.educationAssignmentGrade"},
  "id": "String (identifier)",
  "recipient": {"@odata.type": "microsoft.graph.educationSubmissionRecipient"},
  "returnedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "returnedDateTime": "String (timestamp)",
  "resourcesFolderUrl": "String",
  "status": "string",
  "submittedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "submittedDateTime": "String (timestamp)",
  "unsubmittedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "unsubmittedDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
