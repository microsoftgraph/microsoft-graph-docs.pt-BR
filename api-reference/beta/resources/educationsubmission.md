---
title: Tipo de recurso educationSubmission
description: Representa os recursos que um indivíduo (ou grupo) envia para uma tarefa e os resultados (como notas ou comentários) associados ao envio.
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 12618b5a852755f9c478896b6088aa1d6836a549
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685058"
---
# <a name="educationsubmission-resource-type"></a>Tipo de recurso educationSubmission

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os recursos que um indivíduo (ou grupo) entregará para uma [](educationassignment.md) tarefa e os resultados (como notas ou comentários) associados ao **envio**.

Os envios são de propriedade de uma **atribuição**. Os envios são criados automaticamente quando uma **atribuição** é publicada. O **envio** possui duas listas de recursos. Os recursos representam a área de trabalho de usuários/grupos, enquanto os recursos enviados representam os recursos que foram entregues ativamente pelos alunos.  

A **propriedade de status** é somente leitura e o objeto é movido pelo fluxo de trabalho por meio de ações. 

Se [setUpResourcesFolder](../api/educationsubmission-setupResourcesFolder.md) não tiver sido chamado em um recurso **educationSubmission** , a propriedade **resourcesFolderUrl** será `null`.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter educationSubmission](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |Ler propriedades e relações de um **objeto educationSubmission** .|
|[Listar recursos](../api/educationsubmission-list-resources.md) |[coleção educationSubmissionResource](educationsubmissionresource.md)| Obtenha uma **coleção de objetos educationSubmissionResource** .|
|[Listar submittedResources](../api/educationsubmission-list-submittedresources.md) |[coleção educationSubmissionResource](educationsubmissionresource.md)| Obtenha uma **coleção de objetos educationSubmissionResource** .|
|[Listar resultados](../api/educationsubmission-list-outcomes.md) |[coleção educationOutcome](educationoutcome.md)| Obtenha uma **coleção de objetos educationOutcome** .|
|[Retorno](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|Um professor usa o retorno para indicar que as notas/comentários podem ser mostrados ao aluno.|
|[Reatribuir](../api/educationsubmission-reassign.md)|[educationSubmission](educationsubmission.md)|Reatribua o envio ao aluno com comentários para revisão.|
|[Configurar a pasta de recursos específicos de envio](../api/educationsubmission-setupResourcesFolder.md) |[educationSubmission](educationsubmission.md) | Crie uma SharePoint (em local predefinido) para carregar arquivos como recursos de envio. |
|[Enviar](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|Um aluno usa enviar para entregar a **tarefa**. Isso copiará os recursos para **a pasta submittedResources** para a classificação e atualizará o status.|
|[cancelar](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|Um aluno usa o cancelamento para mover o estado do envio do envio de volta para o trabalho. Isso copiará os recursos para a **pasta workingResources** para a classificação e atualizará o status.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|Identificador exclusivo para o envio.|
|destinatário|[educationSubmissionRecipient](educationsubmissionrecipient.md)|Who esse envio é atribuído.|
|returnedBy|[identitySet](identityset.md)|Usuário que moveu o status deste envio para retornado.|
|returnedDateTime|DateTimeOffset|Momento no tempo em que o envio foi retornado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|resourcesFolderUrl|String|Pasta em que todos os recursos de arquivo para esse envio precisam ser armazenados.|
|status|educationSubmissionStatus| Somente leitura. Os valores possíveis são: `working`, `submitted`, `released`, `returned`e `unknownFutureValue` `reassigned`. Observe que você deve usar o `Prefer: include-unknown-enum-members` cabeçalho da solicitação para obter os seguintes valores nesta [enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `reassigned`.|
|submittedBy|[identitySet](identityset.md)|Usuário que moveu o recurso para o estado enviado.|
|submittedDateTime|DateTimeOffset|Momento no tempo em que o envio foi movido para o estado enviado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|unsubmittedBy|[identitySet](identityset.md)|Usuário que moveu o recurso de enviado para o estado de trabalho.|
|unsubmittedDateTime|DateTimeOffset|Momento no tempo em que o envio foi movido do envio para o estado de trabalho. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|reassignedBy|[identitySet](identityset.md)|Usuário que moveu o status deste envio para reatribuido.|
|reassignedDateTime|DateTimeOffset|Momento no tempo em que o envio foi reatribuido. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recursos|[coleção educationSubmissionResource](educationsubmissionresource.md)| Anulável.|
|submittedResources|[coleção educationSubmissionResource](educationsubmissionresource.md)| Somente leitura. Anulável.|
|Resultados|[coleção educationOutcome](educationOutcome.md) . Contém notas, comentários e/ou informações de rubricas que o professor atribui a este envio|Leitura/gravação. Anulável.|

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
    "reassignedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "reassignedDateTime":"String (timestamp)"
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


