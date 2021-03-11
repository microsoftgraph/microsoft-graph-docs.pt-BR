---
title: Tipo de recurso educationSubmission
description: Os envios pertencem a uma atribuição. Um envio representa os recursos que um indivíduo (ou grupo) entrega para uma atribuição e a nota/feedback que é retornada.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: fccb8c691d5398bd95cc3ebc7eca1fc3028443a5
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722154"
---
# <a name="educationsubmission-resource-type"></a>Tipo de recurso educationSubmission

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os envios pertencem a uma atribuição. Um envio representa os recursos que um indivíduo (ou grupo) entrega para uma atribuição e os resultados (como notas ou comentários) associados ao envio.
Os envios são criados automaticamente quando uma atribuição é publicada. O envio possui duas listas de recursos. Os recursos representam a área de trabalho usuário/grupos enquanto os recursos enviados representam os recursos que foram ativamente entregues pelos alunos.  

>**Observação:** O status é somente leitura e o objeto é movido pelo fluxo de trabalho por meio de ações. 

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter educationSubmission](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |Leia propriedades e relações de um **objeto educationSubmission.**|
|[Listar recursos](../api/educationsubmission-list-resources.md) |[Coleção educationSubmissionResource](educationsubmissionresource.md)| Obter uma **coleção de objetos educationSubmissionResource.**|
|[Listar submittedResources](../api/educationsubmission-list-submittedresources.md) |[Coleção educationSubmissionResource](educationsubmissionresource.md)| Obter uma **coleção de objetos educationSubmissionResource.**|
|[Listar resultados](../api/educationsubmission-list-outcomes.md) |[Coleção educationOutcome](educationoutcome.md)| Obter uma **coleção de objetos educationOutcome.**|
|[Retornar](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|Um professor usa o retorno para indicar que as notas/comentários podem ser mostradas ao aluno.|
|[Enviar](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|Um aluno usa enviar para entregar a atribuição. Isso copiará os recursos para a **pasta submittedResources** para a classificação e atualiza o status.|
|[Unsubmit](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|Um aluno usa o cancelamento para mover o estado do envio do envio de volta ao trabalho. Isso copiará os recursos para a **pasta workingResources** para a classificação e atualiza o status.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|destinatário|[educationSubmissionRecipient](educationsubmissionrecipient.md)|A quem esse envio é atribuído.|
|releasedBy|[identitySet](identityset.md)|Usuário que moveu o status desse envio para liberado.|
|releasedDateTime|DateTimeOffset|Momento no tempo em que o envio foi lançado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|returnedBy|[identitySet](identityset.md)|Usuário que moveu o status desse envio para retornado.|
|returnedDateTime|DateTimeOffset|Momento no tempo em que o envio foi retornado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|resourcesFolderUrl|Cadeia de caracteres|Pasta onde todos os recursos de arquivo para esse envio precisam ser armazenados.|
|status|cadeia de caracteres| Somente Leitura. Os valores possíveis são: `working`, `submitted`, `released`, `returned`.|
|submittedBy|[identitySet](identityset.md)|Usuário que moveu o recurso para o estado enviado.|
|submittedDateTime|DateTimeOffset|Momento no tempo em que o envio foi movido para o estado enviado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|unsubmittedBy|[identitySet](identityset.md)|Usuário que moveu o recurso de enviado para o estado de trabalho.|
|unsubmittedDateTime|DateTimeOffset|Momento no tempo em que o envio foi movido do envio para o estado de trabalho. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recursos|[Coleção educationSubmissionResource](educationsubmissionresource.md)| Anulável.|
|submittedResources|[Coleção educationSubmissionResource](educationsubmissionresource.md)| Somente leitura. Anulável.|
|outcomes|[Coleção educationOutcome.](educationOutcome.md) Contém notas, comentários e/ou informações rubricas que o professor atribui a esse envio|Leitura-Gravação. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
    "id":"String (identifier)",
    "recipient":{"@odata.type":"microsoft.graph.educationSubmissionRecipient"},
    "returnedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "returnedDateTime":"String (timestamp)",
    "resourcesFolderUrl":"String",
    "status":"string",
    "submittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "submittedDateTime":"String (timestamp)",
    "unsubmittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "unsubmittedDateTime":"String (timestamp)",
    "releasedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "releasedDateTime":"String (timestamp)"
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
  "suppressions": []
}
-->


