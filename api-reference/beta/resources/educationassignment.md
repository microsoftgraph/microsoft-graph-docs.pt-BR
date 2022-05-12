---
title: tipo de recurso educationAssignment
description: As atribuições são tarefas ou unidades de trabalho atribuídas a um aluno ou membro da equipe em uma classe como parte do estudo.
ms.localizationpriority: medium
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ca08c26283b84d3a0bdc45fbfed6efd782d71c6f
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366174"
---
# <a name="educationassignment-resource-type"></a>tipo de recurso educationAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As atribuições são tarefas ou unidades de trabalho atribuídas a um aluno ou membro da equipe em uma classe como parte do estudo. 

Somente professores ou proprietários de equipe podem **criar tarefas**. **As tarefas** contêm folhetos e tarefas nas qual o professor deseja que o aluno trabalhe. Cada tarefa **de** aluno tem um [envio associado](educationsubmissionresource.md) que contém qualquer trabalho que seu professor pediu para ser entregue. Um professor pode adicionar pontuações e comentários ao **envio** entregue pelo aluno.

Quando uma **atribuição** é criada, ela está em um estado de Rascunho. Os alunos não podem ver **a tarefa** e **os envios** não serão criados. Você pode alterar o status de uma **atribuição** usando a [ação de](../api/educationassignment-publish.md) publicação. Você não pode usar uma solicitação PATCH para alterar o status **da atribuição** .

**As** APIs de atribuição são expostas no namespace de classe.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar recurso de tarefa](../api/educationassignment-post-resources.md) |[educationAssignmentResource](educationassignmentresource.md)| Crie um novo **educationAssignmentResource** postando na coleção de recursos.|
|[Obter a tarefa](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |Ler propriedades e relações de um **objeto educationAssignment** .|
|[Atualizar](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |Atualize **um objeto educationAssignment** . |
|[Excluir](../api/educationassignment-delete.md) | Nenhuma |**Exclua um objeto educationAssignment**. |
|[Publish](../api/educationassignment-publish.md)|[educationAssignment](educationassignment.md)|Altere o estado de **um objeto educationAssignment** de rascunho para publicado.|
|[Configurar a pasta de recursos de atribuição](../api/educationassignment-setupresourcesfolder.md)| string| Crie uma SharePoint (em local predefinido) para carregar arquivos como recursos de atribuição.|
|[Listar recursos](../api/educationassignment-list-resources.md) |[coleção educationAssignmentResource](educationassignmentresource.md)| Obtenha uma **coleção de objetos educationAssignmentResource** .|
|[Listar envios](../api/educationassignment-list-submissions.md) |[coleção educationSubmission](educationsubmission.md)| Obtenha uma **coleção de objetos educationSubmission** .|
|[Listar categorias](../api/educationassignment-list-categories.md) |[coleção educationCategory](educationcategory.md)| Obtenha uma **coleção de objetos educationCategory** .|
|[Adicionar categorias](../api/educationassignment-post-categories.md) |[educationCategory](educationcategory.md) | Atribua **uma educationCategory** que pertence à classe a esta tarefa.|
|[Remover categoria](../api/educationassignment-remove-category.md) |Nenhuma| Remova uma **educationCategory que** pertence à classe desta **tarefa**.|
|[Anexar rubric](../api/educationassignment-put-rubric.md)|Nenhum|Anexe um **educationRubric existente** a essa **tarefa**.|
|[Remover rubrica](../api/educationassignment-delete-rubric.md)|Nenhuma|**Desanexe o educationRubric** desta **tarefa**.|
|[Obter delta](../api/educationassignment-delta.md)|[coleção educationAssignment](../resources/educationassignment.md)|Obtenha uma lista de atribuições recém-criadas ou **atualizadas** sem precisar executar uma leitura completa da coleção.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura.|
|addedStudentAction|Cadeia de caracteres|Campo opcional para controlar o comportamento **da tarefa** para alunos que são adicionados após **a publicação** da tarefa. Se não for especificado, o valor será padrão `none` . Atualmente, dá suporte a apenas dois valores: `none` ou `assignIfOpen`.|
|addToCalendarAction| educationAddToCalendarOptions|Campo opcional para controlar o comportamento **da** tarefa para adicionar **tarefas aos calendários** dos alunos e professores quando a **tarefa** é publicada. Os valores possíveis são: `none`, `studentsAndPublisher`, `studentsAndTeamOwners`, `unknownFutureValue`e `studentsOnly`. Observe que você deve usar o `Prefer: include-unknown-enum-members` cabeçalho da solicitação para obter os seguintes valores nesta [enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `studentsOnly`. O valor padrão é `none`.|
|allowLateSubmissions|Booliano| Identifica se os alunos podem enviar após a data de conclusão. Se essa propriedade não for especificada durante a criação, o padrão será true. |
|allowStudentsToAddResourcesToSubmission|Booliano| Identifica se os alunos podem adicionar seus próprios recursos a um **envio** ou se eles só podem modificar os recursos adicionados pelo professor. |
|assignDateTime|DateTimeOffset|A data em que a **atribuição** deve ficar ativa.  Se, no futuro, **a tarefa** não for mostrada ao aluno até essa data.  O **tipo de carimbo de data** /hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| Quais usuários ou classe inteira devem receber um objeto **de envio** depois que a **atribuição** for publicada. |
|assignedDateTime|DateTimeOffset|O momento em que a **tarefa** foi publicada para os alunos e **a tarefa** aparece na linha do tempo dos alunos.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|classId|Cadeia de caracteres| Classe à qual esta **tarefa** pertence. |
|closeDateTime|DateTimeOffset| Data em que **a atribuição** será fechada para **envios**. Este é um campo opcional que pode ser nulo se  a atribuição não permitirLateSubmissions ou quando closeDateTime for igual ao dueDateTime. Mas, se especificado, closeDateTime deve ser maior ou igual ao dueDateTime. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|createdBy|[identitySet](identityset.md)| Who criou a **atribuição**. |
|createdDateTime|DateTimeOffset|Momento em que **a atribuição** foi criada.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|displayName|Cadeia de caracteres|Nome da **atribuição**.|
|dueDateTime|DateTimeOffset|Data de **conclusão da tarefa** dos alunos.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|Classificação|[educationAssignmentGradeType](educationassignmentgradetype.md)|Como **a tarefa** será classificada. |
|Instruções|[itemBody](itembody.md)| Instruções para a **atribuição**.  Isso junto com o nome de exibição informa ao aluno o que fazer. |
|lastModifiedBy|[identitySet](identityset.md)| Who última modificação da **atribuição**. |
|lastModifiedDateTime|DateTimeOffset|Momento em que **a atribuição** foi modificada pela última vez.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|notificationChannelUrl|Cadeia de caracteres|Campo opcional para especificar a URL do [canal para](channel.md) postar a **notificação de publicação de atribuição** . Se não for especificado ou nulo, o padrão será o `General` canal. Esse campo só se aplica a **atribuições em** que o valor **assignTo** é [educationAssignmentClassRecipient](educationassignmentclassrecipient.md). A atualização do **notificationChannelUrl** não é permitida após **a publicação** da atribuição.|
|status|cadeia de caracteres| Status da **atribuição**.  Você não pode APLICAR PATCH a esse valor.  Os valores possíveis são: `draft`, `scheduled`, `published`, `assigned`.|
|webUrl|cadeia de caracteres| A URL de link profundo para a **atribuição fornecida**.|
|resourcesFolderUrl|string| URL da pasta em que todos os recursos de arquivo para essa **atribuição** são armazenados.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recursos|[coleção educationAssignmentResource](educationassignmentresource.md)| Learning objetos associados a essa **atribuição**.  Somente professores podem modificar essa lista. Anulável.|
|Submissões|[coleção educationSubmission](educationsubmission.md)| Depois de publicado, há um objeto **de envio** para cada aluno que representa seu trabalho e nota.  Somente leitura. Anulável.|
|categories|[coleção educationCategory](educationcategory.md)| Quando definido, permite que os usuários localizem **facilmente atribuições** de um determinado tipo.  Somente leitura. Anulável.|
|Rubrica|[educationRubric](educationrubric.md)|Quando definido, a rubrica de classificação anexada a essa **atribuição**.|

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
  "addToCalendarAction": "string",
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
