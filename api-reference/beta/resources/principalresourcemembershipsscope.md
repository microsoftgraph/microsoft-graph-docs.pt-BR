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
# <a name="principalresourcemembershipsscope-resource-type"></a><span data-ttu-id="598d4-103">Tipo de recurso principalResourceMembershipsScope</span><span class="sxs-lookup"><span data-stu-id="598d4-103">principalResourceMembershipsScope resource type</span></span>

<span data-ttu-id="598d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="598d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="598d4-105">O principalResourceMembershipsScope é um tipo de [accessReviewScope](accessreviewscope.md) que permite selecionar uma coleção de escopos principais e uma coleção de escopos de recursos e revisar o acesso de entidades selecionadas aos recursos selecionados.</span><span class="sxs-lookup"><span data-stu-id="598d4-105">The principalResourceMembershipsScope is a type of [accessReviewScope](accessreviewscope.md) which allows you to select a collection of principal scopes and a collection of resource scopes and review access of selected principals to selected resources.</span></span> <span data-ttu-id="598d4-106">Consulte as consultas com suporte para ver o que pode ser selecionado.</span><span class="sxs-lookup"><span data-stu-id="598d4-106">See the supported queries to see what can be selected.</span></span> <span data-ttu-id="598d4-107">Ele é usado como a `scope` propriedade de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="598d4-107">It is used as the `scope` property of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span>

<span data-ttu-id="598d4-108">Herda de [accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="598d4-108">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="598d4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="598d4-109">Properties</span></span>
|<span data-ttu-id="598d4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="598d4-110">Property</span></span>|<span data-ttu-id="598d4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="598d4-111">Type</span></span>|<span data-ttu-id="598d4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="598d4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="598d4-113">principalScopes</span><span class="sxs-lookup"><span data-stu-id="598d4-113">principalScopes</span></span>|<span data-ttu-id="598d4-114">[Coleção accessReviewScope](../resources/accessreviewscope.md)</span><span class="sxs-lookup"><span data-stu-id="598d4-114">[accessReviewScope](../resources/accessreviewscope.md) collection</span></span>|<span data-ttu-id="598d4-115">Define os escopos das entidades a serem incluídas em uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="598d4-115">Defines the scopes of the principals to be included in an access review.</span></span>|
|<span data-ttu-id="598d4-116">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="598d4-116">resourceScopes</span></span>|<span data-ttu-id="598d4-117">[Coleção accessReviewScope](../resources/accessreviewscope.md)</span><span class="sxs-lookup"><span data-stu-id="598d4-117">[accessReviewScope](../resources/accessreviewscope.md) collection</span></span>|<span data-ttu-id="598d4-118">Define os escopos dos recursos para os quais o acesso será revisado.</span><span class="sxs-lookup"><span data-stu-id="598d4-118">Defines the scopes of the resources for which access will be reviewed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="598d4-119">Relações</span><span class="sxs-lookup"><span data-stu-id="598d4-119">Relationships</span></span>
<span data-ttu-id="598d4-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="598d4-120">None.</span></span>

### <a name="supported-queries-for-resourcescope"></a><span data-ttu-id="598d4-121">Consultas com suporte para resourceScope</span><span class="sxs-lookup"><span data-stu-id="598d4-121">Supported queries for resourceScope</span></span>
<span data-ttu-id="598d4-122">As consultas são suportadas como a `resourceScope` propriedade.</span><span class="sxs-lookup"><span data-stu-id="598d4-122">The queries are supported as the `resourceScope` property.</span></span> <span data-ttu-id="598d4-123">Eles determinam o conjunto de recursos para o qual o acesso está sendo revisado.</span><span class="sxs-lookup"><span data-stu-id="598d4-123">They determine the set of resources access is being reviewed to.</span></span> 

|<span data-ttu-id="598d4-124">Cenário</span><span class="sxs-lookup"><span data-stu-id="598d4-124">Scenario</span></span>| <span data-ttu-id="598d4-125">consulta resourceScope</span><span class="sxs-lookup"><span data-stu-id="598d4-125">resourceScope Query</span></span> | 
|--|--|
| <span data-ttu-id="598d4-126">Revisão do acesso de principalScopes a uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="598d4-126">Reviewing access of principalScopes to a service principal</span></span> | <span data-ttu-id="598d4-127">/servicePrincipals/{ID da entidade de serviço}</span><span class="sxs-lookup"><span data-stu-id="598d4-127">/servicePrincipals/{service principal ID}</span></span> |
| <span data-ttu-id="598d4-128">Revisão do acesso de principalScopes a uma função de diretório do Azure AD</span><span class="sxs-lookup"><span data-stu-id="598d4-128">Reviewing access of principalScopes to an Azure AD directory role</span></span> | <span data-ttu-id="598d4-129">/roleManagement/directory/roleDefinitions/{role ID}</span><span class="sxs-lookup"><span data-stu-id="598d4-129">/roleManagement/directory/roleDefinitions/{role ID}</span></span> |
| <span data-ttu-id="598d4-130">Revisão do acesso de principalScopes a todas as funções de diretório do Azure AD</span><span class="sxs-lookup"><span data-stu-id="598d4-130">Reviewing access of principalScopes to all Azure AD directory roles</span></span> | <span data-ttu-id="598d4-131">/roleManagement/directory/roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="598d4-131">/roleManagement/directory/roleDefinitions</span></span> |

### <a name="supported-queries-for-principalscope"></a><span data-ttu-id="598d4-132">Consultas com suporte para o principalScope</span><span class="sxs-lookup"><span data-stu-id="598d4-132">Supported queries for principalScope</span></span>
<span data-ttu-id="598d4-133">As consultas são suportadas como a `principalScope` propriedade.</span><span class="sxs-lookup"><span data-stu-id="598d4-133">The queries are supported as the `principalScope` property.</span></span> <span data-ttu-id="598d4-134">Eles determinam o conjunto de entidades cujo acesso ao resourceScope associado será revisado.</span><span class="sxs-lookup"><span data-stu-id="598d4-134">They determine the set of principals whose access to the associated resourceScope will be reviewed.</span></span> <span data-ttu-id="598d4-135">O tipo de principalScope associado lista os tipos de consulta de odata aceitos como o principalScope.</span><span class="sxs-lookup"><span data-stu-id="598d4-135">The associated principalScope Type lists the odata query types accepted as the principalScope.</span></span>

|<span data-ttu-id="598d4-136">Cenário</span><span class="sxs-lookup"><span data-stu-id="598d4-136">Scenario</span></span>| <span data-ttu-id="598d4-137">consulta principalScope</span><span class="sxs-lookup"><span data-stu-id="598d4-137">principalScope Query</span></span> | <span data-ttu-id="598d4-138">Tipo de consulta OData</span><span class="sxs-lookup"><span data-stu-id="598d4-138">OData Query Type</span></span> | <span data-ttu-id="598d4-139">Comentários adicionais</span><span class="sxs-lookup"><span data-stu-id="598d4-139">Additional Comments</span></span> |
|--|--|-- | --|
| <span data-ttu-id="598d4-140">Revisar o acesso de todos os usuários ao resourceScope</span><span class="sxs-lookup"><span data-stu-id="598d4-140">Review access of all users to the resourceScope</span></span> | <span data-ttu-id="598d4-141">/users</span><span class="sxs-lookup"><span data-stu-id="598d4-141">/users</span></span> |[<span data-ttu-id="598d4-142">accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="598d4-142">accessReviewQueryScope</span></span>](accessreviewqueryscope.md)||
| <span data-ttu-id="598d4-143">Revisar o acesso de usuários convidados ao resourceScope</span><span class="sxs-lookup"><span data-stu-id="598d4-143">Review access of  guest users to the resourceScope</span></span> | <span data-ttu-id="598d4-144">/users?$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="598d4-144">/users?$filter=(userType eq 'Guest')</span></span> |[<span data-ttu-id="598d4-145">accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="598d4-145">accessReviewQueryScope</span></span>](accessreviewqueryscope.md)||
| <span data-ttu-id="598d4-146">Revisar o acesso de todos os usuários inativos ao resourceScope</span><span class="sxs-lookup"><span data-stu-id="598d4-146">Review access of all inactive users to the resourceScope</span></span> | <span data-ttu-id="598d4-147">/users</span><span class="sxs-lookup"><span data-stu-id="598d4-147">/users</span></span> |[<span data-ttu-id="598d4-148">accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="598d4-148">accessReviewInactiveUsersQueryScope</span></span>](accessreviewinactiveusersqueryscope.md)| <span data-ttu-id="598d4-149">Deve incluir `instanceDuration` a propriedade</span><span class="sxs-lookup"><span data-stu-id="598d4-149">Must include `instanceDuration` property</span></span>|
| <span data-ttu-id="598d4-150">Revisar o acesso de usuários inativos convidados ao resourceScope</span><span class="sxs-lookup"><span data-stu-id="598d4-150">Review access of guest inactive users to the resourceScope</span></span> | <span data-ttu-id="598d4-151">/users?$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="598d4-151">/users?$filter=(userType eq 'Guest')</span></span> |[<span data-ttu-id="598d4-152">accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="598d4-152">accessReviewInactiveUsersQueryScope</span></span>](accessreviewinactiveusersqueryscope.md)| <span data-ttu-id="598d4-153">Deve incluir `instanceDuration` a propriedade</span><span class="sxs-lookup"><span data-stu-id="598d4-153">Must include `instanceDuration` property</span></span>|




## <a name="json-representation"></a><span data-ttu-id="598d4-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="598d4-154">JSON representation</span></span>
<span data-ttu-id="598d4-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="598d4-155">The following is a JSON representation of the resource.</span></span>
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
