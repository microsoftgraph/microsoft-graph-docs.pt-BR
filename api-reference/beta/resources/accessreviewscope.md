---
title: tipo de recurso accessReviewScope
description: 'No recurso de revisões do Azure AD Access, o `accessReviewScope` representa quais entidades serão revisadas em uma revisão do Access.  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: af5a9bde0763f8aea9e28dc74832586c9e0d2e82
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000767"
---
# <a name="accessreviewscope-resource-type"></a>tipo de recurso accessReviewScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **accessReviewScope** define quais entidades serão revisadas em um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md). Isso é expresso como uma consulta OData. O tipo de consulta também deve ser expresso para que os cenários possam ter suporte para revisar entidades fora do MicrosoftGraph, como ARM.

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo  | Descrição |
| :-------------------------| :---------- | :---------- |
| consulta |Cadeia de caracteres  | A consulta que especifica o que será revisado. Consulte a tabela para obter exemplos. |
|queryType  |Cadeia de caracteres | O tipo de consulta. Os exemplos incluem MicrosoftGraph e ARM. |

### <a name="supported-queries-for-accessreviewscope-as-scope"></a>Consultas com suporte para o accessReviewScope como escopo
As consultas a seguir são suportadas como a `scope` propriedade em um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)

|Cenário| Consulta | Comentários adicionais |
|--|--|-- |
| Revisão de todos os usuários atribuídos a um grupo | /groups/{Group ID}/transitiveMembers ||
| Revisão de usuários convidados atribuídos a um grupo | /groups/{Group ID}/Microsoft.Graph.User/? $count = true&$filter = (UserType EQ ' Guest ') ||
| Revisão de usuários convidados atribuídos a todos os grupos | ./Members/Microsoft.Graph.User/? $count = true&$filter = (UserType EQ ' Guest ') | Observe que o instanceEnumerationScope correspondente também deve ser passado para o accessReviewScheduleDefinition. Consulte a tabela abaixo para ver instanceEnumerationScope consulta. |
| Revisões de Assigment do pacote de acesso de gerenciamento de direitos | /identityGovernance/entitlementManagement/accessPackageAssignments? $filter = (accessPackageId EQ ' {Package ID} ' e assignmentPolicyId EQ ' {ID} ')| Observe que somente leitura tem suporte para revisões de atribuição de pacote do Access|

### <a name="supported-queries-for-accessreviewscope-as-instanceenumerationscope"></a>Consultas com suporte para o accessReviewScope como instanceEnumerationScope
As consultas a seguir são suportadas como a `instanceEnumerationScope` propriedade em um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)

|Cenário| Consulta | Comentários adicionais |
|--|--|--|
| Revisão de usuários convidados atribuídos a todos os grupos, excluindo grupos especificados | /groups? $filter = (groupTypes/Any (c:c + EQ + ' Unified ') e ID ne ' {ID de grupo} ' e ID ne ' {ID de grupo} ' e ID ne ' {Group ID} ') &$count = true | Observe que o escopo correspondente deve também ser passado para o accessReviewScheduleDefinition. Consulte "análise de usuários convidados atribuídos a todos os grupos" na tabela de propriedades de escopo acima para a consulta de escopo. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScope",
  "query": "String",
  "queryType": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
