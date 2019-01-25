---
title: tipo de recurso de accessReview
description: 'No Windows Azure AD access analisa o recurso, o `accessReview` representa uma revisão de acesso.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2cb5d32a8dcc6b12330aca6e831a8ab2083759df
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523516"
---
# <a name="accessreview-resource-type"></a>tipo de recurso de accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de [acesso analisa](accessreviews-root.md) Azure AD, o `accessReview` representa uma revisão de acesso.  


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Obtenha uma revisão do access com uma id específica. |
|[Criar accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Crie um novo accessReview. |
|[Excluir accessReview](../api/accessreview-delete.md) | Nenhum.   | Exclua um accessReview. |
|[Atualizar accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Atualize um accessReview. |
|[Listar accessReview revisores](../api/accessreview-listreviewers.md) |      coleção [userIdentity](useridentity.md)| Obtenha os revisores de um accessReview. |
|[Adicionar Revisor accessReview](../api/accessreview-addreviewer.md) |      Nenhum.   |   Adicione um revisor a um accessReview. |
|[Remover accessReview revisor](../api/accessreview-removereviewer.md) | Nenhum.  |   Remova um revisor de um accessReview. |
|[Lista accessReview decisões](../api/accessreview-listdecisions.md) |      coleção [accessReviewDecision](accessreviewdecision.md)| Obtenha as decisões de um accessReview.|
|[Listar meus decisões accessReview](../api/accessreview-listmydecisions.md) |     coleção [accessReviewDecision](accessreviewdecision.md)| Como um revisor, obtenha Minhas decisões de um accessReview.|
|[Enviar accessReview lembrete](../api/accessreview-sendreminder.md) |        Nenhum.   |   Envie um lembrete para os revisores de um accessReview. |
|[Parar accessReview](../api/accessreview-stop.md) |     Nenhum.   |   Pare uma accessReview. |
|[Redefinir accessReview decisões](../api/accessreview-reset.md) |     Nenhum.   |   Redefina as decisões em um accessReview em andamento.|
|[Aplicar accessReview decisões](../api/accessreview-apply.md) |     Nenhum.   |   Aplique as decisões de um accessReview concluída.|

## <a name="permissions"></a>Permissões

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.Read.All, AccessReview.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | O identificador exclusivo atribuído pelo recurso de uma revisão de acesso. |
| `displayName`             |`String`                                                        | O nome de revisão de acesso. Necessários na criação. |
| `startDateTime`           |`DateTimeOffset`                                                | DateTime quando a revisão está agendada para ser iniciar.  Isso poderia ser uma data no futuro.  Necessários na criação. |
| `endDateTime`             |`DateTimeOffset`                                                | DateTime quando a revisão está agendada para terminar. Isto deve ser de pelo menos um dia mais recente do que a data de início.  Necessários na criação. |
| `status`                  |`String`                                                        | Este campo somente leitura Especifica o status de um accessReview. Os estados típicos incluem `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, e `AutoReviewed`. |
| `description`             |`String`                                                        | A descrição fornecida pelo criador de revisão do access, para mostrar aos revisores. |
| `businessFlowTemplateId`  |`String`                                                        | O identificador de modelo de fluxo de negócios. Necessários na criação. |
| `reviewerType`            |`String`                                                        | O tipo de relacionamento de revisor ao objeto de destino, uma das `self`, `delegated` ou `entityOwners`. Necessários na criação. | 
| `createdBy`               |[userIdentity](useridentity.md)                                 | O usuário que criou este examinar. |
| `reviewedEntity`          |`microsoft.graph.identity`                                      | O objeto para o qual o access analisa é revisar as atribuições de direitos de acesso. Isso pode ser o grupo para a revisão de associações de usuários em um grupo, ou o aplicativo para uma análise das atribuições de usuários para um aplicativo. Necessários na criação. | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | As configurações de um accessReview, consulte a definição de tipo abaixo. |



## <a name="relationships"></a>Relacionamento




| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `reviewers`               |coleção [userIdentity](useridentity.md)                     | A coleção de revisores para uma revisão de acesso, se reviewerType de revisão de acesso é do tipo `delegate`. |
| `decisions`               |coleção [accessReviewDecision](accessreviewdecision.md) | A coleção de decisões para essa revisão de acesso. |
| `myDecisions`             |coleção [accessReviewDecision](accessreviewdecision.md) | A coleção de decisões para o chamador, se o chamador é um revisor. |
| `instances`               |coleção [accessReview](accessreview.md)         | A coleção de avaliações de acesso instâncias passado, presente e futuro, se esse objeto é uma análise mais acesso recorrente. |

Se essas relações estão presentes em um objeto, depende se o objeto for uma revisão de acesso de uma única vez, a série de uma análise mais acesso recorrentes, ou uma instância de uma análise mais acesso recorrente.

| Cenário | Possui revisores? | Tem decisões e myDecisions? | Possui instâncias? |
|:---------|:---------------|:---------------|:---------------|
|Revisão de acesso de uma única vez|Sim | Sim, uma vez iniciado | Não |
| Revisão de acesso recorrente | Sim | Não | Sim |
| Instância de uma análise mais acesso recorrente | Sim | Sim, uma vez iniciado | Não |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
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

## <a name="the-accessreviewsettings-type"></a>O tipo de accessReviewSettings

O `accessReviewSettings` fornece configurações adicionais ao criar uma revisão de acesso, para controlar o comportamento de recurso ao iniciar uma revisão de acesso.  Esse tipo tem as seguintes propriedades: 

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | Sinalizador para indicar se o envio de emails para revisores e o criador de revisão está habilitado.                |
| `remindersEnabled`|`Boolean`       | Sinalizador para indicar se o envio de emails de lembrete aos revisores estão habilitadas.       |
| `justificationRequiredOnApproval`|`Boolean` | Sinalizador para indicar se revisores são necessários para fornecer uma justificativa durante a revisão de acesso.|
| `activityDurationInDays`|`Int64` | O número de dias de atividades do usuário para mostrar aos revisores. |
| `autoReviewEnabled`|`Boolean` | Sinalizador para indicar se o recurso deve definir uma decisão se o revisor não fornecer um, para uso com auto-apply, está habilitado. |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | As configurações detalhadas sobre como o recurso deve definir a decisão de revisão, para uso com auto-apply, descrito abaixo. |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | Configurações detalhadas para recorrência, descrito abaixo. |
| `autoApplyReviewResultsEnabled`|`Boolean` | Sinalizador para indicar se aplicar automaticamente o recurso, para alterar automaticamente o recurso de acesso do objeto de destino, está habilitado.  Se não estiver habilitado, um usuário deve, após a conclusão da revisão, se aplicam a revisão de acesso. |
| `accessRecommendationsEnabled`|`Boolean` | Sinalizador para indicar se mostrar as recomendações para revisores está habilitado. |



## <a name="the-autoreviewsettings-type"></a>O tipo de autoReviewSettings

O `autoReviewSettings` é incorporado dentro as configurações de revisão de acesso e especifica o comportamento para o recurso quando terminar de revisar um acesso.  O tipo tem uma propriedade, `notReviewedResult`.

| Propriedade                     | Tipo     | Descrição                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | Deve ser `Approve`, `Deny` ou `Recommendation`. |


## <a name="the-accessreviewrecurrencesettings-type"></a>O tipo de accessReviewRecurrenceSettings

O `accessReviewRecurrenceSettings` é incorporado dentro as configurações de revisão de acesso e especifica que a revisão do access recorrente em intervalos regulares.  Esse tipo tem as seguintes propriedades:

| Propriedade                     | Tipo                                                                                                          | Descrição |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | O intervalo de recorrência, que deve ser um dos `onetime`, `weekly`, `monthly`, `quarterly`, ou `annual`.                                                                   |
| `recurrenceEndType`|`String` | Como a recorrência terminará. Se for `Never`, e em seguida, não há nenhum fim explícito da série recorrência. Se for `endBy`, em seguida, a recorrência terminará em uma determinada data. Se for `occurrences`, em seguida, a série terminará após `recurrentCount` concluíram instâncias da revisão. |
| `durationInDays`|`Int32`     | A duração em dias para recorrência.                                                                              |
| `recurrenceCount`|`Int32`    | A contagem de recorrências, se o valor da `recurrenceEndType` é `occurrences`, ou caso contrário, 0.                                                        |



<!--
{
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
