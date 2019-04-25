---
title: tipo de recurso educationAssignment
description: O recurso **educationAssignment** representa uma tarefa ou unidade de trabalho atribuída a um membro de aluno ou de equipe em uma classe como parte de seu estudo. Somente professores ou proprietários de equipe podem criar atribuições. As atribuições contêm folhetos e tarefas que o professor deseja que o aluno trabalhe. Cada atribuição de aluno tem um envio associado que contém qualquer trabalho que seus professores pediram para ser ativado. Um professor pode adicionar resultados e comentários ao envio que foi ativado pelo aluno.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 03612cd65dbefac4e31f1a4d06085ba635fe1eab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543039"
---
# <a name="educationassignment-resource-type"></a>tipo de recurso educationAssignment

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **educationAssignment** representa uma tarefa ou unidade de trabalho atribuída a um membro de aluno ou de equipe em uma classe como parte de seu estudo. Somente professores ou proprietários de equipe podem criar atribuições. As atribuições contêm folhetos e tarefas que o professor deseja que o aluno trabalhe. Cada atribuição de aluno tem um [envio](educationsubmissionresource.md) associado que contém qualquer trabalho que seus professores pediram para ser ativado. Um professor pode adicionar resultados e comentários ao envio que foi ativado pelo aluno.

Quando uma atribuição é criada, ela está em um estado de rascunho. Os alunos não podem ver a atribuição e os envios não serão criados. Você pode alterar o status de uma atribuição usando a ação [publicar](../api/educationassignment-publish.md) . Você não pode usar uma solicitação PATCH para alterar o status da atribuição.

As APIs de atribuição são expostas no namespace da classe.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter tarefa](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |Ler propriedades e relações de um objeto **educationAssignment** .|
|[Criar recurso de tarefa](../api/educationassignment-post-resources.md) |[educationAssignmentResource](educationassignmentresource.md)| Crie um novo **educationAssignmentResource** postando na coleção Resources.|
|[Listar recursos](../api/educationassignment-list-resources.md) |coleção [educationAssignmentResource](educationassignmentresource.md)| Obtenha uma coleção de objetos **educationAssignmentResource** .|
|[Envios de lista](../api/educationassignment-list-submissions.md) |coleção [educationSubmission](educationsubmission.md)| Obtenha uma coleção de objetos **educationSubmission** .|
|[Listar categorias](../api/educationassignment-list-categories.md) |coleção [educationCategory](educationcategory.md)| Obtenha uma coleção de objetos **educationCategory** .|
|[Adicionar categorias](../api/educationassignment-add-categories.md) |[educationCategory](educationcategory.md) | Atribua um **educationCategory** pertencente à classe a essa atribuição.|
|[Remover categoria](../api/educationassignment-remove-category.md) |Nenhum| Remover um **educationCategory** pertencente à classe dessa atribuição.|
|[Update](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |Atualize um objeto **educationAssignment** . |
|[Excluir](../api/educationassignment-delete.md) | Nenhum |Excluir um objeto **educationAssignment** . |
|[Publish](../api/educationassignment-publish.md)|[educationAssignment](educationassignment.md)|Alterar o estado de um objeto **educationAssignment** de rascunho para publicado.|
|[Obter URL da pasta do recurso](../api/educationassignment-getresourcesfolderurl.md)| string| A pasta do OneDrive em que os recursos baseados em arquivo devem ser colocados para fazer parte de um recurso de atribuição. Os arquivos devem estar localizados nessa pasta para serem adicionados como um recurso.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura.|
|allowLateSubmissions|Booliano| Identifica se os alunos podem enviar após a data de conclusão. Se essa propriedade não for especificada durante a criação, o padrão será true. |
|allowStudentsToAddResourcesToSubmission|Booliano| Identifica se os alunos podem adicionar seus próprios recursos a um envio ou se eles só podem modificar recursos adicionados pelo professor. |
|assignDateTime|DateTimeOffset|A data em que a atribuição deve se tornar ativa.  Se no futuro, a atribuição não será mostrada ao aluno até esta data.  O tipo **timestamp** representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|atribuir|[educationAssignmentRecipient](educationassignmentrecipient.md)| Quais usuários ou classes inteira devem receber um objeto de envio depois que a atribuição for publicada. |
|assignedDateTime|DateTimeOffset|O momento em que a atribuição foi publicada para estudantes e a atribuição aparece na linha do tempo dos alunos.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|classId|String| Classe à qual essa atribuição pertence. |
|createdBy|[identitySet](identityset.md)| Quem criou a atribuição. |
|createdDateTime|DateTimeOffset|Momento em que a atribuição foi criada.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|displayName|String|Nome da atribuição.|
|dueDateTime|DateTimeOffset|Data de vencimento da atribuição de alunos.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|notas|[educationAssignmentGradeType](educationassignmentgradetype.md)|Como a atribuição será classificada. |
|contida|[itemBody](itembody.md)| Instruções para a atribuição.  Isso, juntamente com o nome para exibição, diga ao aluno o que fazer. |
|lastModifiedBy|[identitySet](identityset.md)| Quem modificou a atribuição pela última vez. |
|lastModifiedDateTime|DateTimeOffset|Momento em que a atribuição foi modificada pela última vez.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|status|cadeia de caracteres| Status da **atribuição**.  Você não pode corrigir esse valor.  Os valores possíveis são: `draft`, `published`, `assigned`.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recursos|coleção [educationAssignmentResource](educationassignmentresource.md)| Objetos de aprendizado associados a essa atribuição.  Somente os professores podem modificar essa lista. Anulável.|
|envios|coleção [educationSubmission](educationsubmission.md)| Depois de publicado, há um objeto de envio para cada aluno representando seu trabalho e classificação.  Somente leitura. Anulável.|
|categories|coleção [educationCategory](educationcategory.md)| Quando definido, permite que os usuários encontrem facilmente as atribuições de um determinado tipo.  Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "String (timestamp)",
  "classId": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "dueDateTime": "String (timestamp)",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "instructions": {"@odata.type": "microsoft.graph.itemBody"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "status": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
