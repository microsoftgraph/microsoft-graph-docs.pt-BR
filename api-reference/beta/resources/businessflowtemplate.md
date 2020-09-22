---
title: tipo de recurso businessFlowTemplate
description: No recurso de revisões do Azure AD Access, o `businesFlowTemplate` representa um modelo de fluxo de negócios do Azure AD. O identificador de um modelo, como a análise de membros convidados de um grupo, é fornecido pelo chamador durante a criação de uma revisão do Access.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 81185c1773c24c3f51190b8f222427034db4097c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071625"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="f9e6c-104">tipo de recurso businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="f9e6c-104">businessFlowTemplate resource type</span></span>

<span data-ttu-id="f9e6c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9e6c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9e6c-106">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , o `businesFlowTemplate` representa um modelo de fluxo de negócios do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f9e6c-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="f9e6c-107">O identificador de um modelo, como a análise de membros convidados de um grupo, é fornecido pelo chamador durante a criação de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="f9e6c-107">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="f9e6c-108">Os objetos do modelo de fluxo de negócios são gerados automaticamente quando o administrador global embuti o locatário para usar o recurso de revisões do Access.</span><span class="sxs-lookup"><span data-stu-id="f9e6c-108">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="f9e6c-109">Os modelos de fluxo de negócios incluem revisões de acesso de atribuições para um aplicativo, associações de um grupo, associações de uma função do Azure AD, associações de usuários convidados de um grupo e atribuições de usuários convidados a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f9e6c-109">The business flow templates include access reviews of assignments to an application, memberships of a group, memberships of an Azure AD role, guest user memberships of a group, and guest user assignments to an application.</span></span> <span data-ttu-id="f9e6c-110">Nenhum modelo de fluxo de negócios adicional pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="f9e6c-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="f9e6c-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="f9e6c-111">Methods</span></span>

| <span data-ttu-id="f9e6c-112">Método</span><span class="sxs-lookup"><span data-stu-id="f9e6c-112">Method</span></span>           | <span data-ttu-id="f9e6c-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f9e6c-113">Return Type</span></span>    |<span data-ttu-id="f9e6c-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9e6c-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f9e6c-115">Listar businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="f9e6c-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="f9e6c-116">coleção [businessFlowTemplate](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="f9e6c-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="f9e6c-117">Obtenha os modelos de fluxo de negócios apropriados para as revisões do Access.</span><span class="sxs-lookup"><span data-stu-id="f9e6c-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="f9e6c-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9e6c-118">Properties</span></span>
| <span data-ttu-id="f9e6c-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9e6c-119">Property</span></span>     | <span data-ttu-id="f9e6c-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9e6c-120">Type</span></span>   |<span data-ttu-id="f9e6c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9e6c-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="f9e6c-122">O identificador atribuído ao recurso do modelo de fluxo de negócios.</span><span class="sxs-lookup"><span data-stu-id="f9e6c-122">The feature-assigned identifier of the business flow template.</span></span> <span data-ttu-id="f9e6c-123">Esses valores diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="f9e6c-123">These values are case sensitive.</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="f9e6c-124">O nome do modelo de fluxo de negócios</span><span class="sxs-lookup"><span data-stu-id="f9e6c-124">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="f9e6c-125">Relações</span><span class="sxs-lookup"><span data-stu-id="f9e6c-125">Relationships</span></span>

<span data-ttu-id="f9e6c-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f9e6c-126">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="f9e6c-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="f9e6c-127">See also</span></span>

| <span data-ttu-id="f9e6c-128">Método</span><span class="sxs-lookup"><span data-stu-id="f9e6c-128">Method</span></span>           | <span data-ttu-id="f9e6c-129">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f9e6c-129">Return Type</span></span>    |<span data-ttu-id="f9e6c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9e6c-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f9e6c-131">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="f9e6c-131">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="f9e6c-132">accessReview</span><span class="sxs-lookup"><span data-stu-id="f9e6c-132">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="f9e6c-133">Criar um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="f9e6c-133">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f9e6c-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9e6c-134">JSON representation</span></span>

<span data-ttu-id="f9e6c-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9e6c-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.businessFlowTemplate"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


