---
title: tipo de recurso businessFlowTemplate
description: No recurso de revisões do Azure AD Access, `businesFlowTemplate` o representa um modelo de fluxo de negócios do Azure AD. O identificador de um modelo, como a análise de membros convidados de um grupo, é fornecido pelo chamador durante a criação de uma revisão do Access.
localization_priority: Normal
ms.openlocfilehash: 0cca72bc8ccd372cdaf9952b385bc63f81b0631d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338794"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="688cd-104">tipo de recurso businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="688cd-104">businessFlowTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="688cd-105">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , `businesFlowTemplate` o representa um modelo de fluxo de negócios do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="688cd-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="688cd-106">O identificador de um modelo, como a análise de membros convidados de um grupo, é fornecido pelo chamador durante a criação de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="688cd-106">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="688cd-107">Os objetos do modelo de fluxo de negócios são gerados automaticamente quando o administrador global embuti o locatário para usar o recurso de revisões do Access.</span><span class="sxs-lookup"><span data-stu-id="688cd-107">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="688cd-108">Nenhum modelo de fluxo de negócios adicional pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="688cd-108">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="688cd-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="688cd-109">Methods</span></span>

| <span data-ttu-id="688cd-110">Método</span><span class="sxs-lookup"><span data-stu-id="688cd-110">Method</span></span>           | <span data-ttu-id="688cd-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="688cd-111">Return Type</span></span>    |<span data-ttu-id="688cd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="688cd-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="688cd-113">Listar businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="688cd-113">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="688cd-114">coleção [businessFlowTemplate](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="688cd-114">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="688cd-115">Obtenha os modelos de fluxo de negócios apropriados para as revisões do Access.</span><span class="sxs-lookup"><span data-stu-id="688cd-115">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="688cd-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="688cd-116">Properties</span></span>
| <span data-ttu-id="688cd-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="688cd-117">Property</span></span>     | <span data-ttu-id="688cd-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="688cd-118">Type</span></span>   |<span data-ttu-id="688cd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="688cd-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="688cd-120">O identificador atribuído ao recurso do modelo de fluxo de negócios</span><span class="sxs-lookup"><span data-stu-id="688cd-120">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="688cd-121">O nome do modelo de fluxo de negócios</span><span class="sxs-lookup"><span data-stu-id="688cd-121">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="688cd-122">Relações</span><span class="sxs-lookup"><span data-stu-id="688cd-122">Relationships</span></span>

<span data-ttu-id="688cd-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="688cd-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="688cd-124">Ver também</span><span class="sxs-lookup"><span data-stu-id="688cd-124">See also</span></span>

| <span data-ttu-id="688cd-125">Método</span><span class="sxs-lookup"><span data-stu-id="688cd-125">Method</span></span>           | <span data-ttu-id="688cd-126">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="688cd-126">Return Type</span></span>    |<span data-ttu-id="688cd-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="688cd-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="688cd-128">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="688cd-128">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="688cd-129">accessReview</span><span class="sxs-lookup"><span data-stu-id="688cd-129">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="688cd-130">Criar um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="688cd-130">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="688cd-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="688cd-131">JSON representation</span></span>

<span data-ttu-id="688cd-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="688cd-132">Here is a JSON representation of the resource.</span></span>

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
