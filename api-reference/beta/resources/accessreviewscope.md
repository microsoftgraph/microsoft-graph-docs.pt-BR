---
title: Tipo de recurso accessReviewScope
description: 'No recurso de revisões de acesso do Azure AD, as entidades serão revisadas em `accessReviewScope` uma revisão de acesso.  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8739ff822ffc6b0f2989b80a150c7d968880f532
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133431"
---
# <a name="accessreviewscope-resource-type"></a>Tipo de recurso accessReviewScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **accessReviewScope** define quais entidades serão revisadas em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md). Isso é expresso como uma consulta odata. O tipo de consulta também deve ser expresso para que os cenários possam ter suporte para revisar entidades fora do MicrosoftGraph, como ARM.

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo  | Descrição |
| :-------------------------| :---------- | :---------- |
| consulta |String  | A consulta especificando o que será revisado. Consulte a tabela para ver exemplos. |
|queryType  |String | O tipo de consulta. Exemplos incluem MicrosoftGraph e ARM. |

### <a name="supported-queries-for-accessreviewscope-as-scope"></a>Consultas com suporte para accessReviewScope como escopo
A seguir estão consultas com suporte como a `scope` propriedade em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md)

|Cenário| Consulta | Comentários adicionais |
|--|--|-- |
| Revisão de todos os usuários atribuídos a um grupo | /groups/{group id}/transitiveMembers ||
| Revisão de usuários convidados atribuídos a um grupo | /groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest') ||
| Revisão de usuários convidados atribuídos a todos os grupos | ./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest') | Observe que a instanceEnumerationScope correspondente também deve ser passada para accessReviewScheduleDefinition. Consulte a tabela abaixo para consultar instanceEnumerationScope. |
| Avaliações de asigment do pacote de acesso ao gerenciamento de direitos | /identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' e assignmentPolicyId eq '{id}')| Observe que somente READ é suportado para Revisões de Atribuição de Pacote do Access|

### <a name="supported-queries-for-accessreviewscope-as-instanceenumerationscope"></a>Consultas com suporte para accessReviewScope como instanceEnumerationScope
A seguir estão consultas com suporte como a `instanceEnumerationScope` propriedade em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md)

|Cenário| Consulta | Comentários adicionais |
|--|--|--|
| Revisão de usuários convidados atribuídos a todos os grupos, excluindo grupos especificados | /groups?$filter=(groupTypes/any(c:c+eq+'Unified') and id ne '{group id}' and id ne '{group id}' and id ne '{group id}')&$count=true | Observe que o escopo correspondente também deve ser passado para accessReviewScheduleDefinition. Consulte "Revisão de usuários convidados atribuídos a todos os grupos" na tabela de propriedades de escopo acima para a consulta de escopo. |

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
