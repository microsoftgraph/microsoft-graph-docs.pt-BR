---
title: Tipo de recurso accessReviewScheduleDefinition
description: Representa o agendamento de uma revisão de acesso do Azure AD.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 23b13daba0ea86d2330bd8b6c7f59e27af967aec
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084696"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>Tipo de recurso accessReviewScheduleDefinition

Namespace: microsoft.graph

Representa o agendamento de uma revisão de acesso do Azure [AD.](accessreviewsv2-root.md)

Um accessReviewScheduleDefinition contém uma lista de [objetos accessReviewInstance.](accessreviewinstance.md) Cada recorrência da definição de agenda cria uma instância. As instâncias também representam cada recurso exclusivo que está sendo revisado. Se uma definição de agenda analisar vários recursos, cada recurso terá uma instância exclusiva por cada recorrência. No caso de uma revisão única, apenas uma instância é criada por recurso.

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | [Coleção accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Lista todos os accessReviewScheduleDefinition. Não inclui objetos accessReviewInstance associados nos resultados. |
|[Obter accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obter um accessReviewScheduleDefinition com uma **id especificada**. Não inclui objetos accessReviewInstance associados nos resultados. |
|[Criar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-post.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Crie um novo accessReviewScheduleDefinition. |
|[Excluir accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Nenhum. | Excluir um accessReviewScheduleDefinition com uma **id especificada**. |
|[Atualizar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Nenhum. | Atualizar propriedades de um accessReviewScheduleDefinition com uma **id especificada**. |
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[Coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Recupera todas as definições para as quais o usuário de chamada é um revistor em uma ou mais instâncias.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| id | String | O identificador exclusivo atribuído ao recurso de uma revisão de acesso. Oferece suporte para `$select`. Somente leitura.|
| displayName | Cadeia de caracteres   | Nome da série de revisão de acesso. Oferece suporte para `$select` e `$orderBy`. Obrigatório durante a criação. |
| createdDateTime  |DateTimeOffset  | Timestamp quando a série de revisão de acesso foi criada. Oferece suporte para `$select` e `$orderBy`. Somente leitura. |
| lastModifiedDateTime | DateTimeOffset   | Timestamp quando a série de revisão de acesso foi modificada pela última vez. Oferece suporte para `$select`. Somente leitura.|
| status  |String   | Este campo somente leitura especifica o status de uma revisão de acesso. Os estados típicos `Initializing` `NotStarted` incluem , `Starting` , , , , , e `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` .  <br>Suporta `$select` `$orderby` , e ( `$filter` `eq` somente). Somente leitura. |
| descriptionForAdmins  | Cadeia de caracteres  |  Descrição fornecida pelos criadores de revisão para fornecer mais contexto da revisão aos administradores. Suporta o `$select`. |
| descriptionForReviewers | Cadeia de caracteres | Descrição fornecida pelos criadores de revisão para fornecer mais contexto da revisão aos revisadores. Os revisadores verão essa descrição no email enviado a eles solicitando sua revisão. As notificações por email suportam até 256 caracteres. Suporta o `$select`. |
| createdBy  |[userIdentity](../resources/useridentity.md)  | Usuário que criou essa revisão. Somente leitura. |
| escopo  |[accessReviewScope](../resources/accessreviewscope.md)  |  Define as entidades cujo acesso é revisado.  Para escopos com suporte, consulte [accessReviewScope](accessreviewscope.md). Obrigatório durante a criação. Suporta `$select` e `$filter` ( `contains` somente). Para exemplos de opções para configurar escopo, consulte [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept). |
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | Essa propriedade é necessária ao analisar o acesso dos usuários convidados em todos os grupos Microsoft 365 e determina quais grupos Microsoft 365 são revisados. Cada grupo se tornará um **accessReviewInstance exclusivo** da série de revisão de acesso.  Para escopos com suporte, consulte [accessReviewScope](accessreviewscope.md). Suporta o `$select`. Para exemplos de opções para configurar instanceEnumerationScope, consulte Configure the scope of your [access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept). | 
| settings  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| As configurações de uma série de revisão de acesso, consulte a definição de tipo abaixo. Suporta o `$select`. Obrigatório durante a criação. |
| revisadores   |[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de revisão de acesso é usada para definir quem são os revistores. A propriedade reviewers só será atualizável se usuários individuais são atribuídos como revistores. Obrigatório durante a criação. Suporta o `$select`. Para exemplos de opções para atribuir revisadores, consulte Atribuir revisadores à sua definição de revisão de acesso [usando a API do Microsoft Graph](/graph/accessreviews-reviewers-concept). |
| fallbackReviewers   |[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos do revistor é usada para definir a lista de revisadores de fallback. Esses revisadores de fallback serão notificados para tomar medidas se nenhum usuário for encontrado na lista de revisadores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como o revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe. Consulte [accessReviewReviewerScope](accessreviewreviewerscope.md). Substitui **backupReviewers**. Suporta o `$select`. |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
| instances|[Coleção accessReviewInstance](accessreviewinstance.md) | Se **accessReviewScheduleDefinition** for uma revisão de acesso recorrente, as instâncias representarão cada recorrência. Uma revisão que não se recorre terá exatamente uma instância. As instâncias também representam cada recurso exclusivo sob revisão no **accessReviewScheduleDefinition**. Se uma revisão tiver vários recursos e várias instâncias, cada recurso terá uma instância exclusiva para cada recorrência. |

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
  }
}
```
