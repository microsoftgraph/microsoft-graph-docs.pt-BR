---
title: Tipo de recurso accessReviewQueryScope
description: Define o que será revisado em uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 976a856755b6bb638719bec6006c3d8d0587c42a
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469731"
---
# <a name="accessreviewqueryscope-resource-type"></a>Tipo de recurso accessReviewQueryScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Um objeto accessReviewQueryScope define o que será revisado em [um accessReview](../resources/accessreviewsv2-root.md). Consulte as consultas com suporte para ver as opções de seleção. Para analisar o escopo de uma revisão de acesso a usuários inativos, consulte [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md). 

Herda de [accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|consulta|String|A consulta que representa o que será revisado em uma revisão de acesso. Exemplos disso incluem /groups/{id}/members?$filter=...|
|queryRoot|String|No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta. Essa propriedade só será necessária se uma consulta relativa for especificada. Por exemplo, `./manager`.|
|queryType|String|Indica o tipo de consulta. Os tipos incluem MicrosoftGraph e ARM.|

### <a name="supported-queries-for-accessreviewqueryscope-as-scope"></a>Consultas com suporte para accessReviewQueryScope como escopo
As consultas são suportadas como a `scope` propriedade em [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)

|Cenário| Consulta | Comentários adicionais |
|--|--|-- |
| Revisão de todos os usuários atribuídos a um grupo | /groups/{group id}/transitiveMembers ||
| Revisão de usuários convidados atribuídos a um grupo | /groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest') ||
| Revisão de usuários convidados atribuídos a todos os grupos do Microsoft 365 | ./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest') | Observe que a instância correspondenteEnumerationScope também deve ser passada para accessReviewScheduleDefinition. Consulte a tabela abaixo para consulta instanceEnumerationScope. |
| Avaliações de atribuição de pacote de acesso ao gerenciamento de direitos | /identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')| Observe que somente READ é suportado para Avaliações de Atribuição de Pacote do Access|
| Revisão das Entidades de Serviço atribuídas a funções privilegiadas | /beta/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') e roleDefinitionId eq '{role ID}') | |

### <a name="supported-queries-for-instanceenumerationscope"></a>Consultas com suporte para instanceEnumerationScope 
As consultas são suportadas como a `instanceEnumerationScope` propriedade em [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)

|Cenário| Consulta | Comentários adicionais |
|--|--|--|
|  Revisão de usuários convidados atribuídos a todos os grupos do Microsoft 365| /v1.0/groups? \$ filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true | Observe que o escopo correspondente também deve ser passado junto com isso|
| Revisão de usuários convidados atribuídos a todas as equipes | /v1.0/groups? \$ filter=(groupTypes/any(c:c+eq+'Unified') e resourceProvisioningOptions/Any(x:x eq 'Team'))&$count=true | Observe que o escopo correspondente também deve ser passado junto com isso|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
