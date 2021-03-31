---
title: Tipo de recurso principalResourceMembershipsScope
description: Permite que os escopos de seleção revisem o acesso das entidades selecionadas aos recursos selecionados.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2ac3dd53223b9260c3f51c3c872d36b044e698d5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469725"
---
# <a name="principalresourcemembershipsscope-resource-type"></a>Tipo de recurso principalResourceMembershipsScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

O principalResourceMembershipsScope é um tipo de [accessReviewScope](accessreviewscope.md) que permite selecionar uma coleção de escopos principais e uma coleção de escopos de recursos e revisar o acesso de entidades selecionadas aos recursos selecionados. Consulte as consultas com suporte para ver o que pode ser selecionado. Ele é usado como a `scope` propriedade de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).

Herda de [accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|principalScopes|[Coleção accessReviewScope](../resources/accessreviewscope.md)|Define os escopos das entidades a serem incluídas em uma revisão de acesso.|
|resourceScopes|[Coleção accessReviewScope](../resources/accessreviewscope.md)|Define os escopos dos recursos para os quais o acesso será revisado.|

## <a name="relationships"></a>Relações
Nenhum

### <a name="supported-queries-for-resourcescope"></a>Consultas com suporte para resourceScope
As consultas são suportadas como a `resourceScope` propriedade. Eles determinam o conjunto de recursos para o qual o acesso está sendo revisado. 

|Cenário| consulta resourceScope | 
|--|--|
| Revisão do acesso de principalScopes a uma entidade de serviço | /servicePrincipals/{ID da entidade de serviço} |
| Revisão do acesso de principalScopes a uma função de diretório do Azure AD | /roleManagement/directory/roleDefinitions/{role ID} |
| Revisão do acesso de principalScopes a todas as funções de diretório do Azure AD | /roleManagement/directory/roleDefinitions |

### <a name="supported-queries-for-principalscope"></a>Consultas com suporte para o principalScope
As consultas são suportadas como a `principalScope` propriedade. Eles determinam o conjunto de entidades cujo acesso ao resourceScope associado será revisado. O tipo de principalScope associado lista os tipos de consulta de odata aceitos como o principalScope.

|Cenário| consulta principalScope | Tipo de consulta OData | Comentários adicionais |
|--|--|-- | --|
| Revisar o acesso de todos os usuários ao resourceScope | /users |[accessReviewQueryScope](accessreviewqueryscope.md)||
| Revisar o acesso de usuários convidados ao resourceScope | /users?$filter=(userType eq 'Guest') |[accessReviewQueryScope](accessreviewqueryscope.md)||
| Revisar o acesso de todos os usuários inativos ao resourceScope | /users |[accessReviewInactiveUsersQueryScope](accessreviewinactiveusersqueryscope.md)| Deve incluir `instanceDuration` a propriedade|
| Revisar o acesso de usuários inativos convidados ao resourceScope | /users?$filter=(userType eq 'Guest') |[accessReviewInactiveUsersQueryScope](accessreviewinactiveusersqueryscope.md)| Deve incluir `instanceDuration` a propriedade|




## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.principalResourceMembershipsScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
  "principalScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
  "resourceScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ]
}
```
