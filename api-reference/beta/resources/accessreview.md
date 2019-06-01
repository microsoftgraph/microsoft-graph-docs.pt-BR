---
title: tipo de recurso accessReview
description: 'No recurso de revisões do Azure AD Access, `accessReview` o representa uma revisão do Access.  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b1801a7f7cbd52375e4fbbfb42847b29539a2dde
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657732"
---
# <a name="accessreview-resource-type"></a>tipo de recurso accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões do Azure AD [Access](accessreviews-root.md) , `accessReview` o representa uma revisão do Access.  


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Obtenha uma revisão do Access com uma ID específica. |
|[Criar accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Criar um novo accessReview. |
|[Excluir accessReview](../api/accessreview-delete.md) | Nenhum.   | Excluir um accessReview. |
|[Atualizar accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Atualizar um accessReview. |
|[Listar revisores do accessReview](../api/accessreview-listreviewers.md) |      [](useridentity.md) coleção UserIdentity| Obter os revisores de um accessReview. |
|[Adicionar revisor accessReview](../api/accessreview-addreviewer.md) |      Nenhum.   |   Adicionar um revisor a um accessReview. |
|[Remover revisor accessReview](../api/accessreview-removereviewer.md) | Nenhum.  |   Remover um revisor de um accessReview. |
|[Listar decisões accessReview](../api/accessreview-listdecisions.md) |      coleção [accessReviewDecision](accessreviewdecision.md)| Obtenha as decisões de um accessReview.|
|[Listar minhas decisões do accessReview](../api/accessreview-listmydecisions.md) |     coleção [accessReviewDecision](accessreviewdecision.md)| Como revisor, obtenha as minhas decisões de um accessReview.|
|[Enviar lembrete accessReview](../api/accessreview-sendreminder.md) |        Nenhum.   |   Envie um lembrete para os revisores de um accessReview. |
|[Parar accessReview](../api/accessreview-stop.md) |     Nenhum.   |   Parar um accessReview. |
|[Redefinir decisões do accessReview](../api/accessreview-reset.md) |     Nenhum.   |   Redefina as decisões em um accessReview em andamento.|
|[Aplicar decisões accessReview](../api/accessreview-apply.md) |     Nenhum.   |   Aplique as decisões de um accessReview concluído.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | O identificador exclusivo atribuído a um recurso de uma revisão do Access. |
| `displayName`             |`String`                                                        | O nome de revisão do acesso. Obrigatório ao criar. |
| `startDateTime`           |`DateTimeOffset`                                                | O DateTime quando a revisão está agendada para ser iniciada.  Isso pode ser uma data no futuro.  Obrigatório ao criar. |
| `endDateTime`             |`DateTimeOffset`                                                | O DateTime quando a revisão é agendada para terminar. Este deve ser pelo menos um dia depois da data de início.  Obrigatório ao criar. |
| `status`                  |`String`                                                        | Este campo somente leitura especifica o status de um accessReview. Os Estados típicos `Initializing`incluem `NotStarted`, `Starting``InProgress` `Completing` `Completed` `AutoReviewing`,,,,, e `AutoReviewed`. |
| `description`             |`String`                                                        | A descrição fornecida pelo criador de revisão de acesso, para mostrar aos revisores. |
| `businessFlowTemplateId`  |`String`                                                        | O identificador do modelo de fluxo de negócios. Obrigatório ao criar. |
| `reviewerType`            |`String`                                                        | O tipo de relação de revisor para o objeto de destino, um `self` `delegated` ou `entityOwners`. Obrigatório ao criar. | 
| `createdBy`               |[userIdentity](useridentity.md)                                 | O usuário que criou essa revisão. |
| `reviewedEntity`          |[identity](identity.md)                                      | O objeto para o qual as revisões de acesso está examinando as atribuições de direitos de acesso. Isso pode ser o grupo para a revisão de associações de usuários em um grupo ou o aplicativo para uma revisão das atribuições de usuários a um aplicativo. Obrigatório ao criar. | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | As configurações de um accessReview, confira definição de tipo abaixo. |



## <a name="relationships"></a>Relações




| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `reviewers`               |[](useridentity.md) coleção UserIdentity                     | A coleção de revisores para uma revisão do Access, se o Access revisar revisualizador `delegate`é do tipo. |
| `decisions`               |coleção [accessReviewDecision](accessreviewdecision.md) | O conjunto de decisões para esta revisão do Access. |
| `myDecisions`             |coleção [accessReviewDecision](accessreviewdecision.md) | O conjunto de decisões para o chamador, se o chamador for um revisor. |
| `instances`               |coleção [accessReview](accessreview.md)         | O conjunto de instâncias do Access revês passado, presente e futuro, se esse objeto for uma revisão de acesso recorrente. |

Se essas relações estão presentes em um objeto, depende se o objeto é uma revisão de acesso único, a série de uma revisão de acesso recorrente ou uma instância de uma revisão de acesso recorrente.

| Cenário | Tem revisores? | Tem decisões e mydecisions? | Tem instâncias? |
|:---------|:---------------|:---------------|:---------------|
|Revisão de acesso de uso único|Sim | Sim, depois de iniciado | Não |
| Análise de acesso recorrente | Sim | Não | Sim |
| Instância de uma análise de acesso recorrente | Sim | Sim, depois de iniciado | Não |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReview"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
 "description": "string",
 "businessFlowTemplateId": "string (identifier)",
 "reviewerType": "string",
 "createdBy": "microsoft.graph.userIdentity",
 "reviewedEntity": "microsoft.graph.identity",
 "settings": "microsoft.graph.accessReviewSettings",
 "reviewers": "Collection(microsoft.graph.userIdentity)"
}

```

## <a name="the-accessreviewsettings-type"></a>O tipo accessReviewSettings

O `accessReviewSettings` fornece configurações adicionais ao criar uma revisão do Access, para controlar o comportamento do recurso ao iniciar uma revisão do Access.  Este tipo tem as seguintes propriedades: 

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | Sinalizador para indicar se o envio de emails para revisores e o criador de revisão está habilitado.                |
| `remindersEnabled`|`Boolean`       | Sinalizador para indicar se o envio de emails de lembrete aos revisores está habilitado.       |
| `justificationRequiredOnApproval`|`Boolean` | Sinalizador para indicar se os revisores são necessários para fornecer uma justificativa ao revisar o acesso.|
| `activityDurationInDays`|`Int64` | O número de dias de atividades do usuário para mostrar aos revisores. |
| `autoReviewEnabled`|`Boolean` | Sinalizador para indicar se o recurso deve definir uma decisão se o revisor não fornecer um, para uso com a aplicação automática, está habilitado. |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | Configurações detalhadas de como o recurso deve definir a decisão de revisão, para uso com a aplicação automática, descrita abaixo. |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | Configurações detalhadas de recorrência, descritas abaixo. |
| `autoApplyReviewResultsEnabled`|`Boolean` | Sinalizador para indicar se a capacidade de aplicação automática, para alterar automaticamente o recurso de acesso ao objeto de destino, está habilitada.  Se não habilitado, um usuário deve, após a conclusão da revisão, aplicar a revisão do Access. |
| `accessRecommendationsEnabled`|`Boolean` | Sinalizador para indicar se a exibição de recomendações para revisores está habilitada. |

## <a name="the-autoreviewsettings-type"></a>O tipo autoReviewSettings

O `autoReviewSettings` é inserido nas configurações de análise do Access e especifica o comportamento do recurso quando uma revisão do Access é concluída.  O tipo tem uma propriedade, `notReviewedResult`.

| Propriedade                     | Tipo     | Descrição                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | Deve ser `Approve`, `Deny` ou `Recommendation`. |


## <a name="the-accessreviewrecurrencesettings-type"></a>O tipo accessReviewRecurrenceSettings

O `accessReviewRecurrenceSettings` está incorporado nas configurações de revisão do Access e especifica que a revisão do acesso se repete em intervalos regulares.  Este tipo tem as seguintes propriedades:

| Propriedade                     | Tipo                                                                                                          | Descrição |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | O intervalo de recorrência, que deve ser `onetime`um `weekly`de `monthly`, `quarterly`,, `annual`ou.                                                                   |
| `recurrenceEndType`|`String` | Como a recorrência termina. Se for `Never`, não haverá uma extremidade explícita da série de recorrência. Se for `endBy`, a recorrência terminará em uma determinada data. Se for `occurrences`, a série terminará após `recurrentCount` a conclusão das instâncias da revisão. |
| `durationInDays`|`Int32`     | A duração em dias da recorrência.                                                                              |
| `recurrenceCount`|`Int32`    | A contagem de recorrências, se o valor `recurrenceEndType` for `occurrences`ou 0 caso contrário.                                                        |


<!--
{
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
