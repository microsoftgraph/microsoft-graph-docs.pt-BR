---
title: tipo de recurso businessFlowTemplate
description: No recurso de revisões do Azure AD Access, `businesFlowTemplate` o representa um modelo de fluxo de negócios do Azure AD. O identificador de um modelo, como a análise de membros convidados de um grupo, é fornecido pelo chamador durante a criação de uma revisão do Access.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: markwahl-msft
ms.openlocfilehash: 461fe34e0d572f910f15df9521d54660f0568ad1
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703788"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="6c0b3-104">tipo de recurso businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="6c0b3-104">businessFlowTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c0b3-105">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , `businesFlowTemplate` o representa um modelo de fluxo de negócios do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="6c0b3-106">O identificador de um modelo, como a análise de membros convidados de um grupo, é fornecido pelo chamador durante a criação de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-106">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="6c0b3-107">Os objetos do modelo de fluxo de negócios são gerados automaticamente quando o administrador global embuti o locatário para usar o recurso de revisões do Access.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-107">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="6c0b3-108">Os modelos de fluxo de negócios incluem revisões de acesso de atribuições para um aplicativo, associações de um grupo, associações de uma função do Azure AD, associações de usuários convidados de um grupo e atribuições de usuários convidados a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-108">The business flow templates include access reviews of assignments to an application, memberships of a group, memberships of an Azure AD role, guest user memberships of a group, and guest user assignments to an application.</span></span> <span data-ttu-id="6c0b3-109">Nenhum modelo de fluxo de negócios adicional pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-109">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="6c0b3-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="6c0b3-110">Methods</span></span>

| <span data-ttu-id="6c0b3-111">Método</span><span class="sxs-lookup"><span data-stu-id="6c0b3-111">Method</span></span>           | <span data-ttu-id="6c0b3-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6c0b3-112">Return Type</span></span>    |<span data-ttu-id="6c0b3-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c0b3-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c0b3-114">Listar businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="6c0b3-114">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="6c0b3-115">coleção [businessFlowTemplate](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="6c0b3-115">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="6c0b3-116">Obtenha os modelos de fluxo de negócios apropriados para as revisões do Access.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-116">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c0b3-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c0b3-117">Properties</span></span>
| <span data-ttu-id="6c0b3-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c0b3-118">Property</span></span>     | <span data-ttu-id="6c0b3-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c0b3-119">Type</span></span>   |<span data-ttu-id="6c0b3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c0b3-120">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="6c0b3-121">O identificador atribuído ao recurso do modelo de fluxo de negócios.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-121">The feature-assigned identifier of the business flow template.</span></span> <span data-ttu-id="6c0b3-122">Esses valores diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-122">These values are case sensitive.</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="6c0b3-123">O nome do modelo de fluxo de negócios</span><span class="sxs-lookup"><span data-stu-id="6c0b3-123">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="6c0b3-124">Relações</span><span class="sxs-lookup"><span data-stu-id="6c0b3-124">Relationships</span></span>

<span data-ttu-id="6c0b3-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c0b3-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="6c0b3-126">Ver também</span><span class="sxs-lookup"><span data-stu-id="6c0b3-126">See also</span></span>

| <span data-ttu-id="6c0b3-127">Método</span><span class="sxs-lookup"><span data-stu-id="6c0b3-127">Method</span></span>           | <span data-ttu-id="6c0b3-128">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6c0b3-128">Return Type</span></span>    |<span data-ttu-id="6c0b3-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c0b3-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c0b3-130">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="6c0b3-130">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="6c0b3-131">accessReview</span><span class="sxs-lookup"><span data-stu-id="6c0b3-131">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="6c0b3-132">Criar um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-132">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="6c0b3-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c0b3-133">JSON representation</span></span>

<span data-ttu-id="6c0b3-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-134">Here is a JSON representation of the resource.</span></span>

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
