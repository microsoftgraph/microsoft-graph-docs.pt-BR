---
title: tipo de recurso de educationAssignment
description: O recurso de **educationAssignment** representa uma tarefa ou a unidade de trabalho atribuído a um estudante ou membro da equipe em uma classe como parte de sua estudo. Apenas professores ou proprietários de equipe podem criar atribuições. Atribuições contêm folhetos e que deseja que seja o professor student para trabalhar em tarefas. Cada atribuição de student tem um envio associado que contém qualquer trabalho que seu professor solicitado a ser ativado. Um professor pode adicionar comentários e pontuações para o envio ativado pelo aluno.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: e96b2a27d24f0dc38595e5aea931045199eb6d10
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982257"
---
# <a name="educationassignment-resource-type"></a>tipo de recurso de educationAssignment

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso de **educationAssignment** representa uma tarefa ou a unidade de trabalho atribuído a um estudante ou membro da equipe em uma classe como parte de sua estudo. Apenas professores ou proprietários de equipe podem criar atribuições. Atribuições contêm folhetos e que deseja que seja o professor student para trabalhar em tarefas. Cada atribuição de student tem um [envio](educationsubmissionresource.md) associado que contém qualquer trabalho que seu professor solicitado a ser ativado. Um professor pode adicionar comentários e pontuações para o envio ativado pelo aluno.

Quando uma atribuição é criada, ele é em um estado de rascunho. Alunos não podem ver a atribuição e envios não serão criados. Você pode alterar o status de uma atribuição usando a ação [Publicar](../api/educationassignment-publish.md) . Você não pode usar uma solicitação de PATCH para alterar o status da atribuição.

A atribuição de APIs são expostas no namespace.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Fazer a atribuição](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |Leia as propriedades e os relacionamentos de um objeto **educationAssignment** .|
|[Criar o recurso de atribuição](../api/educationassignment-post-resources.md) |[educationAssignmentResource](educationassignmentresource.md)| Crie um novo **educationAssignmentResource** pelo lançamento à coleção de recursos.|
|[Lista de recursos](../api/educationassignment-list-resources.md) |coleção [educationAssignmentResource](educationassignmentresource.md)| Obtenha uma coleção de objetos **educationAssignmentResource** .|
|[Envios de lista](../api/educationassignment-list-submissions.md) |coleção [educationSubmission](educationsubmission.md)| Obtenha uma coleção de objetos **educationSubmission** .|
|[Update](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |Atualize um objeto **educationAssignment** . |
|[Delete](../api/educationassignment-delete.md) | Nenhum |Exclua um objeto **educationAssignment** . |
|[Publish](../api/educationassignment-publish.md)|[educationAssignment](educationassignment.md)|Altere o estado de um objeto **educationAssignment** de rascunho publicadas.|
|[Obtenha a URL da pasta de recursos](../api/educationassignment-getresourcesfolderurl.md)| string| A pasta de OneDrive em que os recursos baseados no arquivo devem ser colocados para fazer parte de um recurso de atribuição. Arquivos devem estar localizados nesta pasta a ser adicionado como um recurso.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura.|
|allowLateSubmissions|Booliano| Identifica se alunos podem enviar após a data de vencimento. Se essa propriedade não for especificada durante a criação, padrão será true. |
|allowStudentsToAddResourcesToSubmission|Booliano| Identifica se alunos podem adicionar seus próprios recursos para um envio ou se eles só podem modificar recursos adicionados com o professor. |
|assignDateTime|DateTimeOffset|A data quando a atribuição deve se tornar ativa.  Se no futuro, a atribuição não será mostrada ao aluno até esta data.  O tipo de **carimbo de hora** representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| Quais usuários ou classe todo deve receber um objeto de envio depois que a atribuição é publicada. |
|assignedDateTime|DateTimeOffset|No momento em que a atribuição foi publicada para alunos e a atribuição é mostrada na linha do tempo de alunos.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|classId|String| Classe que essa atribuição pertence. |
|createdBy|[identitySet](identityset.md)| Quem criou a atribuição. |
|createdDateTime|DateTimeOffset|Momento em que a atribuição foi criada.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|displayName|String|Nome da atribuição.|
|dueDateTime|DateTimeOffset|Data quando a atribuição de alunos é vencimento.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|classificação|[educationAssignmentGradeType](educationassignmentgradetype.md)|Como a atribuição vai ser Graduada. |
|instruções|[itemBody](itembody.md)| Instruções para a atribuição.  Isso também saberá o nome de exibição dizem student o que fazer. |
|lastModifiedBy|[identitySet](identityset.md)| Quem da última modificação da atribuição. |
|lastModifiedDateTime|DateTimeOffset|Momento da última modificação a atribuição.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|status|string| Status da **atribuição**.  Você não pode corrigir esse valor.  Os valores possíveis são: `draft`, `published`, `assigned`.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recursos|coleção [educationAssignmentResource](educationassignmentresource.md)| Objetos de aprendizado que estão associados essa atribuição.  Professores só podem modificar esta lista. Anulável.|
|envios|coleção [educationSubmission](educationsubmission.md)| Depois de publicado, não há um objeto de envio para cada aluno representando seus trabalhos e um nível.  Somente leitura. Anulável.|

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
