---
title: tipo de recurso businessFlowTemplate
description: No recurso de revisões do Azure AD Access, `businesFlowTemplate` o representa um modelo de fluxo de negócios do Azure AD. O identificador de um modelo, como a análise de membros convidados de um grupo, é fornecido pelo chamador durante a criação de uma revisão do Access.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6890ed724c1a71c69a881ce0e2e70675b3537520
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973481"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="e2875-104">tipo de recurso businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="e2875-104">businessFlowTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2875-105">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , `businesFlowTemplate` o representa um modelo de fluxo de negócios do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e2875-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="e2875-106">O identificador de um modelo, como a análise de membros convidados de um grupo, é fornecido pelo chamador durante a criação de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="e2875-106">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="e2875-107">Os objetos do modelo de fluxo de negócios são gerados automaticamente quando o administrador global embuti o locatário para usar o recurso de revisões do Access.</span><span class="sxs-lookup"><span data-stu-id="e2875-107">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="e2875-108">Nenhum modelo de fluxo de negócios adicional pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="e2875-108">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="e2875-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="e2875-109">Methods</span></span>

| <span data-ttu-id="e2875-110">Método</span><span class="sxs-lookup"><span data-stu-id="e2875-110">Method</span></span>           | <span data-ttu-id="e2875-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e2875-111">Return Type</span></span>    |<span data-ttu-id="e2875-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2875-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e2875-113">Listar businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="e2875-113">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="e2875-114">coleção [businessFlowTemplate](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e2875-114">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="e2875-115">Obtenha os modelos de fluxo de negócios apropriados para as revisões do Access.</span><span class="sxs-lookup"><span data-stu-id="e2875-115">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="e2875-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2875-116">Properties</span></span>
| <span data-ttu-id="e2875-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2875-117">Property</span></span>     | <span data-ttu-id="e2875-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2875-118">Type</span></span>   |<span data-ttu-id="e2875-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2875-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="e2875-120">O identificador atribuído ao recurso do modelo de fluxo de negócios</span><span class="sxs-lookup"><span data-stu-id="e2875-120">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="e2875-121">O nome do modelo de fluxo de negócios</span><span class="sxs-lookup"><span data-stu-id="e2875-121">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="e2875-122">Relações</span><span class="sxs-lookup"><span data-stu-id="e2875-122">Relationships</span></span>

<span data-ttu-id="e2875-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2875-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="e2875-124">Ver também</span><span class="sxs-lookup"><span data-stu-id="e2875-124">See also</span></span>

| <span data-ttu-id="e2875-125">Método</span><span class="sxs-lookup"><span data-stu-id="e2875-125">Method</span></span>           | <span data-ttu-id="e2875-126">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e2875-126">Return Type</span></span>    |<span data-ttu-id="e2875-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2875-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e2875-128">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="e2875-128">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="e2875-129">accessReview</span><span class="sxs-lookup"><span data-stu-id="e2875-129">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="e2875-130">Criar um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="e2875-130">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e2875-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2875-131">JSON representation</span></span>

<span data-ttu-id="e2875-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2875-132">Here is a JSON representation of the resource.</span></span>

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
