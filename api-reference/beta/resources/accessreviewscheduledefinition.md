---
title: Tipo de recurso accessReviewScheduleDefinition
description: Representa uma série de revisão de acesso ou revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5a4d904ce0e15e12002def67714b275babc00917
ms.sourcegitcommit: 1e9a53e7b8e67349288f5cfbabe8355de83817b0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2021
ms.locfileid: "58367293"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>Tipo de recurso accessReviewScheduleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa o agendamento de uma revisão de acesso do Azure [AD.](accessreviewsv2-root.md) 

Um accessReviewScheduleDefinition contém uma lista de [objetos accessReviewInstance.](accessreviewinstance.md) Cada recorrência da definição de agenda cria uma instância. As instâncias também representam cada recurso exclusivo que está sendo revisado. Se uma definição de agenda analisar vários recursos (incluindo vários grupos), cada recurso terá uma instância exclusiva por cada recorrência. No caso de uma revisão única, apenas uma instância é criada por recurso.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | [Coleção accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Lista todos os accessReviewScheduleDefinition. Não inclui objetos accessReviewInstance associados nos resultados. |
|[Obter accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obter um accessReviewScheduleDefinition com uma **id especificada**. Não inclui objetos accessReviewInstance associados nos resultados. |
|[Criar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-post.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Crie um novo accessReviewScheduleDefinition. |
|[Excluir accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Nenhum. | Excluir um accessReviewScheduleDefinition com uma **id especificada**. |
|[Atualizar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Nenhum. | Atualizar propriedades de um accessReviewScheduleDefinition com uma **id especificada**. |
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[Coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Recupera todas as definições para as quais o usuário de chamada é um revistor em uma ou mais instâncias.|

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :------------------| :-------------- | :---------- |
| id | Cadeia de caracteres | O identificador exclusivo atribuído ao recurso de uma revisão de acesso. Oferece suporte para `$select`. Somente leitura.|
| displayName | Cadeia de caracteres   | Nome da série de revisão de acesso. Oferece suporte para `$select` e `$orderBy`. Obrigatório ao criar. |
| createdDateTime  |DateTimeOffset  | Timestamp quando a série de revisão de acesso foi criada. Oferece suporte para `$select`. Somente leitura. |
| lastModifiedDateTime | DateTimeOffset   | Timestamp quando a série de revisão de acesso foi modificada pela última vez. Oferece suporte para `$select`. Somente leitura.|
| status  |Cadeia de caracteres   | Este campo somente leitura especifica o status de uma revisão de acesso. Os estados típicos `Initializing` `NotStarted` incluem , `Starting` , , , , , e `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` .  <br>Suporta `$select` `$orderby` , e ( `$filter` `eq` somente). Somente leitura. |
| descriptionForAdmins  |cadeia de caracteres  |  Descrição fornecida pelos criadores de revisão para fornecer mais contexto da revisão aos administradores. Suporta `$select`. |
| descriptionForReviewers |cadeia de caracteres | Descrição fornecida pelos criadores de revisão para fornecer mais contexto da revisão aos revisadores. Os revisadores verão essa descrição no email enviado a eles solicitando sua revisão. Suporta `$select`. |
| createdBy  |[userIdentity](../resources/useridentity.md)  | Usuário que criou essa revisão. Somente leitura. |
| escopo  |[accessReviewScope](../resources/accessreviewscope.md)  | Define as entidades cujo acesso é revisado. Para escopos com suporte, consulte [accessReviewScope](accessreviewscope.md). Obrigatório durante a criação. Suporta `$select` e `$filter` ( `contains` somente). Para exemplos de opções para configurar escopo, consulte [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept). |
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | Essa propriedade é necessária ao analisar o acesso dos usuários convidados em todos os grupos Microsoft 365 e determina quais grupos Microsoft 365 são revisados. Cada grupo se tornará um **accessReviewInstance exclusivo** da série de revisão de acesso.  Para escopos com suporte, consulte [accessReviewScope](accessreviewscope.md). Suporta o `$select`. Para exemplos de opções para configurar instanceEnumerationScope, consulte Configure the scope of your [access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept). | 
| configurações  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| As configurações de uma série de revisão de acesso, consulte a definição de tipo abaixo. Suporta `$select`. Obrigatório durante a criação. |
| revisadores   |[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de revisão de acesso é usada para definir quem são os revistores. A propriedade reviewers só será atualizável se usuários individuais são atribuídos como revistores. Obrigatório durante a criação. Suporta o `$select`. Para exemplos de opções para atribuir revisadores, consulte Atribuir revisadores à sua definição de revisão de acesso [usando a API do Microsoft Graph](/graph/accessreviews-reviewers-concept). |
| fallbackReviewers   |[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos do revistor é usada para definir a lista de revisadores de fallback. Esses revisadores de fallback serão notificados para tomar medidas se nenhum usuário for encontrado na lista de revisadores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como o revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe. Consulte [accessReviewReviewerScope](accessreviewreviewerscope.md). Substitui backupReviewers. Suporta o `$select`. |
| instances |[Coleção accessReviewInstance](../resources/accessreviewinstance.md)|  Conjunto de instâncias de críticas de acesso para esta série de revisão de acesso. As avaliações do Access que não se recorrem terão apenas uma instância; caso contrário, há uma instância para cada recorrência. |
| backupReviewers (preterido) |[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos do revistor é usada para definir a lista de revisadores de fallback. Esses revisadores de fallback serão notificados para tomar medidas se nenhum usuário for encontrado na lista de revisadores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como o revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe.  Suporta o `$select`. <br>**Observação:** Essa propriedade foi substituída por **fallbackReviewers**. No entanto, especificar **backupReviewers** ou **fallbackReviewers** preenche automaticamente os mesmos valores para a outra propriedade. |
| additionalNotificationRecipients   |[Coleção accessReviewNotificationRecipientItem](../resources/accessReviewNotificationRecipientItem.md)| Define a lista de usuários adicionais ou membros do grupo a serem notificados sobre o progresso da revisão de acesso. |

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `instances`               |[Coleção accessReviewInstance](accessreviewinstance.md)         | Se for `accessReviewScheduleDefinition` uma revisão de acesso recorrente, as instâncias representarão cada recorrência. Uma revisão que não se recorre terá exatamente uma instância. As instâncias também representam cada recurso exclusivo sob revisão no `accessReviewScheduleDefinition` . Se uma revisão tiver vários recursos e várias instâncias, cada recurso terá uma instância exclusiva para cada recorrência. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
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
  "backupReviewers": [
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
