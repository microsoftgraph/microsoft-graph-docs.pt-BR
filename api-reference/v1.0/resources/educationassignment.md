---
title: Tipo de recurso educationAssignment
description: O **recurso educationAssignment** representa uma tarefa ou unidade de trabalho atribuída a um aluno ou membro da equipe em uma classe como parte de seu estudo.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 932a11e32514b8ee8a3ab6a7c3f2280f61b530a5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021719"
---
# <a name="educationassignment-resource-type"></a>Tipo de recurso educationAssignment

Namespace: microsoft.graph

O **recurso educationAssignment** representa uma tarefa ou unidade de trabalho atribuída a um aluno ou membro da equipe em uma classe como parte de seu estudo. 

Somente professores ou proprietários de equipe podem criar atribuições. As atribuições contêm atribuições e tarefas nas que o professor deseja que o aluno trabalhe. Cada atribuição de aluno tem um [envio associado](educationsubmissionresource.md) que contém qualquer trabalho que o professor solicitou para ser entregue. Um professor pode adicionar pontuações e comentários ao envio entregue pelo aluno.

Quando uma atribuição é criada, ela está em um estado rascunho. Os alunos não podem ver a atribuição e os envios não serão criados. Você pode alterar o status de uma atribuição usando a [ação publicar.](../api/educationassignment-publish.md) Não é possível usar uma solicitação PATCH para alterar o status da atribuição.

As APIs de atribuição são expostas no namespace de classe.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar recurso de tarefa](../api/educationassignment-post-resource.md) |[educationAssignmentResource](educationassignmentresource.md)| Crie uma nova **educationAssignmentResource** postando na coleção resources.|
|[Obter a tarefa](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |Ler propriedades e relações de um **objeto educationAssignment.**|
|[Atualizar](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |Atualize **um objeto educationAssignment.** |
|[Delete](../api/educationassignment-delete.md) | None |**Exclua um objeto educationAssignment.** |
|[Publish](../api/educationassignment-publish.md)|[educationAssignment](educationassignment.md)|Altere o estado de um **objeto educationAssignment** de rascunho para publicado.|
|[Configurar pasta de recursos de atribuição](../api/educationassignment-setupresourcesfolder.md)| cadeia de caracteres| Criar uma SharePoint (em local pré-definido) para carregar arquivos como recursos de atribuição|
|[Listar recursos](../api/educationassignment-list-resources.md) |[Coleção educationAssignmentResource](educationassignmentresource.md)| Obter uma **coleção de objetos educationAssignmentResource.**|
|[Listar envios](../api/educationassignment-list-submissions.md) |[Coleção educationSubmission](educationsubmission.md)| Obter uma **coleção de objetos educationSubmission.**|
|[Listar categorias](../api/educationassignment-list-categories.md) |[Coleção educationCategory](educationcategory.md)| Obter uma **coleção de objetos educationCategory.**|
|[Adicionar categorias](../api/educationassignment-post-categories.md) |[educationCategory](educationcategory.md) | Atribua **uma educationCategory** pertencente à classe a essa atribuição.|
|[Remover categoria](../api/educationassignment-remove-category.md) |None| Remova uma **educationCategory** pertencente à classe desta atribuição.|
|[Anexar rubric](../api/educationassignment-put-rubric.md)|None|Anexe um **educationRubric** existente a essa atribuição.|
|[Remover rubric](../api/educationassignment-delete-rubric.md)|None|Desconectar **educationRubric** desta atribuição.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura.|
|addedStudentAction|Cadeia de caracteres|Campo opcional para controlar o comportamento de atribuição para alunos que são adicionados após a publicação da atribuição. Se não for especificado, o valor será `none` padrão. Atualmente, suporta apenas dois valores: `none` ou `assignIfOpen` .|
|allowLateSubmissions|Booliano| Identifica se os alunos podem enviar após a data de vencimento. Se essa propriedade não for especificada durante a criação, ela será padrão como true. |
|allowStudentsToAddResourcesToSubmission|Boolean| Identifica se os alunos podem adicionar seus próprios recursos a um envio ou se eles só podem modificar os recursos adicionados pelo professor. |
|assignDateTime|DateTimeOffset|A data em que a atribuição deve ficar ativa.  Se, no futuro, a atribuição não for mostrada ao aluno até essa data.  O **tipo Timestamp** representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| Quais usuários ou classe inteira devem receber um objeto de envio depois que a atribuição for publicada. |
|assignedDateTime|DateTimeOffset|O momento em que a atribuição foi publicada para os alunos e a atribuição aparece na linha do tempo dos alunos.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|classId|Cadeia de caracteres| Classe a qual essa atribuição pertence. |
|closeDateTime|DateTimeOffset| Data em que a atribuição será fechada para envios. Este é um campo opcional que pode ser nulo se a atribuição não permitirLateSubmissions ou quando closeDateTime for igual ao dueDateTime. Mas, se especificado, o closeDateTime deve ser maior ou igual ao dueDateTime. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|createdBy|[identitySet](identityset.md)| Who a atribuição. |
|createdDateTime|DateTimeOffset|Momento em que a atribuição foi criada.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|displayName|Cadeia de caracteres|Nome da atribuição.|
|dueDateTime|DateTimeOffset|Data em que a atribuição dos alunos é final.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|grading|[educationAssignmentGradeType](educationassignmentgradetype.md)|Como a atribuição será gradeada. |
|instructions|[itemBody](itembody.md)| Instruções para a atribuição.  Isso junto com o nome de exibição diz ao aluno o que fazer. |
|lastModifiedBy|[identitySet](identityset.md)| Who última modificação da atribuição. |
|lastModifiedDateTime|DateTimeOffset|Momento em que a atribuição foi modificada pela última vez.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|notificationChannelUrl|String|Campo opcional para especificar a URL do [canal para](channel.md) postar a notificação de publicação de atribuição. Se não for especificado ou nulo, o padrão será o `General` canal. Este campo só se aplica a atribuições em que o **valor assignTo** é [educationAssignmentClassRecipient](educationassignmentclassrecipient.md). A atualização da **notificaçãoChannelUrl** não é permitida após a publicação da atribuição.|
|status|cadeia de caracteres| Status da **atribuição**.  Não é possível corrigir esse valor.  Os valores possíveis são: `draft`, `scheduled`, `published`, `assigned`.|
|webUrl|cadeia de caracteres| A URL de link profundo para a atribuição determinada.|
|resourcesFolderUrl|cadeia de caracteres| URL da pasta onde todos os recursos de arquivo para essa atribuição são armazenados.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recursos|[Coleção educationAssignmentResource](educationassignmentresource.md)| Learning objetos associados a essa atribuição.  Somente os professores podem modificar essa lista. Anulável.|
|envios|[Coleção educationSubmission](educationsubmission.md)| Depois de publicado, há um objeto de envio para cada aluno que representa seu trabalho e nota.  Somente leitura. Anulável.|
|categories|[Coleção educationCategory](educationcategory.md)| Quando definido, permite que os usuários encontrem facilmente atribuições de um determinado tipo.  Somente leitura. Anulável.|
|rubric|[educationRubric](educationrubric.md)|Quando definido, a rubrica de classificação anexada a essa atribuição.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "addedStudentAction": "none",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "String (timestamp)",
  "classId": "String",
  "closeDateTime": "String (timestamp)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "dueDateTime": "String (timestamp)",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "instructions": {"@odata.type": "microsoft.graph.itemBody"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "notificationChannelUrl": "string",
  "status": "string",
  "webUrl": "string",
  "resourcesFolderUrl": "string"
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
  "suppressions": []
}
-->
