---
title: tipo de recurso de educationSubmission
description: Envios pertencentes a uma atribuição. Um envio representa os recursos que um turn individual (ou de grupo) para uma atribuição e o nível/feedback que é retornado.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9cbfaa46d979e3796ae9128e212bfaa1f6bf8453
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920874"
---
# <a name="educationsubmission-resource-type"></a>tipo de recurso de educationSubmission

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Envios pertencentes a uma atribuição. Um envio representa os recursos que um turn individual (ou de grupo) para uma atribuição e o nível/feedback que é retornado.
Envios são criados automaticamente quando uma atribuição é publicada. O envio possui duas listas de recursos. Recursos representam os grupos de usuários/trabalhando área enquanto os recursos enviados representam os recursos que ativamente foram ativados por alunos.  

>**Observação:** O status é somente leitura e o objeto é movido por meio do fluxo de trabalho por meio de ações. 

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter educationSubmission](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |Leia as propriedades e os relacionamentos de um objeto **educationSubmission** .|
|[Lista de recursos](../api/educationsubmission-list-resources.md) |coleção [educationSubmissionResource](educationsubmissionresource.md)| Obtenha uma coleção de objetos **educationSubmissionResource** .|
|[Lista submittedResources](../api/educationsubmission-list-submittedresources.md) |coleção [educationSubmissionResource](educationsubmissionresource.md)| Obtenha uma coleção de objetos **educationSubmissionResource** .|
|[Update](../api/educationsubmission-update.md) | [educationSubmission](educationsubmission.md) |Atualize um objeto **educationSubmission** . |
|[Retornar](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|Professor usa o retorno para indicar que as notas/comentários podem ser exibidos a student.|
|[Enviar](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|Um estudante usa Enviar para ativar na atribuição. Isso irá copiar os recursos para a pasta **submittedResources** para classificação e atualiza o status.|
|[Unsubmit](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|Um estudante usa o unsubmit para mover o estado do envio do back enviado para o trabalho. Isso irá copiar os recursos para a pasta **workingResources** para classificação e atualiza o status.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|comentários|[educationFeedback](educationfeedback.md)|Contém a propriedade de comentários que armazena as notas do professor volta aos alunos.|
|grade|[educationAssignmentGrade](educationassignmentgrade.md)|Contém as informações de nível que um professor atribui a esse envio.|
|id|Cadeia de caracteres| Somente leitura.|
|destinatário|[educationSubmissionRecipient](educationsubmissionrecipient.md)|Este envio é atribuído à.|
|releasedBy|[identitySet](identityset.md)|Usuário que migraram o status de envio esta liberada.|
|releasedDateTime|DateTimeOffset|Momento específico quando o envio foi lançado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|returnedBy|[identitySet](identityset.md)|Usuário que migraram o status deste envio a ser retornado.|
|returnedDateTime|DateTimeOffset|Momento específico quando o envio foi retornado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|resourcesFolderUrl|Cadeia de caracteres|Pasta onde todos os recursos de arquivo para o envio precisam ser armazenados.|
|status|string| Somente Leitura. Os valores possíveis são: `working`, `submitted`, `released`, `returned`.|
|submittedBy|[identitySet](identityset.md)|Usuário que o recurso são movidas para o estado enviado.|
|submittedDateTime|DateTimeOffset|Momento específico quando o envio foi movido para o estado enviado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|unsubmittedBy|[identitySet](identityset.md)|Usuários que migraram do recurso de enviados para o estado de trabalho.|
|unsubmittedDateTime|DateTimeOffset|Momento específico quando o envio foi movido de enviados para o estado de trabalho. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
