---
title: Tipo de recurso accessReviewScheduleDefinition
description: Representa o agendamento de uma revisão Azure AD acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 11711828cf658fd91b326404201c881ecd252e84
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697705"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>Tipo de recurso accessReviewScheduleDefinition

Namespace: microsoft.graph

Representa o agendamento de uma revisão Azure AD [acesso.](accessreviewsv2-overview.md)

Um accessReviewScheduleDefinition contém uma lista de [objetos accessReviewInstance](accessreviewinstance.md) . Cada recorrência da definição de agendamento cria uma instância. As instâncias também representam cada recurso exclusivo que está sendo revisado. Se uma definição de agenda examinar vários recursos, cada recurso terá uma instância exclusiva para cada recorrência. No caso de uma revisão única, apenas uma instância é criada por recurso.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessReviewScheduleDefinitions](../api/accessreviewset-list-definitions.md) | [coleção accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Lista todos os accessReviewScheduleDefinition. Não inclui objetos accessReviewInstance associados nos resultados. |
|[Obter accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obtenha um accessReviewScheduleDefinition com uma **ID especificada**. Não inclui objetos accessReviewInstance associados nos resultados. |
|[Criar accessReviewScheduleDefinition](../api/accessreviewset-post-definitions.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Crie um novo accessReviewScheduleDefinition. |
|[Excluir accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Nenhum. | Exclua um accessReviewScheduleDefinition com uma **ID especificada**. |
|[Atualizar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Nenhum. | Atualize as propriedades de um accessReviewScheduleDefinition com uma **ID especificada**. |
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Recupera todas as definições para as quais o usuário chamador é um revisores em uma ou mais instâncias.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| additionalNotificationRecipients   |[coleção accessReviewNotificationRecipientItem](../resources/accessReviewNotificationRecipientItem.md)| Define a lista de usuários adicionais ou membros do grupo a serem notificados sobre o progresso da revisão de acesso. |
| createdBy  |[userIdentity](../resources/useridentity.md)  | Usuário que criou essa revisão. Somente leitura. |
| createdDateTime  |DateTimeOffset  | Carimbo de data/hora quando a série de revisão de acesso foi criada. Oferece suporte para `$select` e `$orderBy`. Somente leitura. |
| descriptionForAdmins  | Cadeia de Caracteres  |  Descrição fornecida pelos criadores de revisão para fornecer mais contexto da revisão aos administradores. Oferece suporte para `$select`. |
| descriptionForReviewers | Cadeia de Caracteres | Descrição fornecida pelos criadores de revisão para fornecer mais contexto da revisão aos revisores. Os revisores verão essa descrição no email enviado a eles solicitando sua revisão. As notificações por email dão suporte a até 256 caracteres. Oferece suporte para `$select`. |
| displayName | Cadeia de caracteres   | Nome da série de revisão de acesso. Oferece suporte para `$select` e `$orderBy`. Obrigatório durante a criação. |
| fallbackReviewers   |[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de revisores é usada para definir a lista de revisores de fallback. Esses revisores de fallback serão notificados para tomar medidas se nenhum usuário for encontrado na lista de revisores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe. Consulte [accessReviewReviewerScope](accessreviewreviewerscope.md). Substitui **backupReviewers**. Oferece suporte para `$select`. |
| id | Cadeia de caracteres | O identificador exclusivo atribuído ao recurso de uma revisão de acesso. Oferece suporte para `$select`. Somente leitura.|
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | Essa propriedade é necessária ao definir o escopo de uma revisão para o acesso dos usuários convidados em todos os grupos do Microsoft 365 e determina quais grupos do Microsoft 365 são revisados. Cada grupo se tornará um **accessReviewInstance exclusivo da** série de revisão de acesso.  Para obter escopos com suporte, consulte [accessReviewScope](accessreviewscope.md). Oferece suporte para `$select`. Para obter exemplos de opções para configurar instanceEnumerationScope, consulte Configurar o escopo de sua definição de revisão de acesso usando o [Microsoft API do Graph](/graph/accessreviews-scope-concept). | 
| lastModifiedDateTime | DateTimeOffset   | Carimbo de data/hora quando a série de revisão de acesso foi modificada pela última vez. Oferece suporte para `$select`. Somente leitura.|
| Revisores   |[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de revisão de acesso é usada para definir quem são os revisores. A propriedade de revisores só poderá ser atualizada se usuários individuais forem atribuídos como revisores. Obrigatório durante a criação. Oferece suporte para `$select`. Para obter exemplos de opções para atribuir revisores, consulte Atribuir revisores à sua definição de revisão de acesso [usando o Microsoft API do Graph](/graph/accessreviews-reviewers-concept). |
| scope  |[accessReviewScope](../resources/accessreviewscope.md)  |  Define as entidades cujo acesso é revisado.  Para obter escopos com suporte, consulte [accessReviewScope](accessreviewscope.md). Obrigatório durante a criação. Dá `$select` suporte e `$filter` (`contains` somente). Para obter exemplos de opções para configurar o escopo, consulte Configurar o escopo de sua definição de revisão de acesso [usando o Microsoft API do Graph](/graph/accessreviews-scope-concept). |
| configurações  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| As configurações de uma série de revisão de acesso, consulte a definição de tipo abaixo. Oferece suporte para `$select`. Obrigatório durante a criação. |
| status  |Cadeia de caracteres   | Esse campo somente leitura especifica o status de uma revisão de acesso. Os estados típicos incluem `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`e `AutoReviewed`.  <br>Dá `$select`suporte `$orderby`a , e `$filter` (`eq` somente). Somente leitura. |
| backupReviewers (preterido) |[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de revisores é usada para definir a lista de revisores de fallback. Esses revisores de fallback serão notificados para tomar medidas se nenhum usuário for encontrado na lista de revisores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe.  Oferece suporte para `$select`. <br>**Nota:** Essa propriedade foi substituída por **fallbackReviewers**. No entanto, especificar **backupReviewers** ou **fallbackReviewers** preenche automaticamente os mesmos valores para a outra propriedade. |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
| instances|[coleção accessReviewInstance](accessreviewinstance.md) | Se **accessReviewScheduleDefinition** for uma revisão de acesso recorrente, as instâncias representarão cada recorrência. Uma revisão que não se repetir terá exatamente uma instância. As instâncias também representam cada recurso exclusivo sob revisão no **accessReviewScheduleDefinition**. Se uma revisão tiver vários recursos e várias instâncias, cada recurso terá uma instância exclusiva para cada recorrência. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "descriptionForAdmins": "String",
  "descriptionForReviewers": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "fallbackReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "instanceEnumerationScope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
  },
  "additionalNotificationRecipients": [
    {
        "@odata.type": "microsoft.graph.accessReviewNotificationRecipientItem"
    }
  ]
}
```
