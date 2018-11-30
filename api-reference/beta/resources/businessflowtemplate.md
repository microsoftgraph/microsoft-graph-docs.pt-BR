---
title: tipo de recurso de businessFlowTemplate
description: No Windows Azure AD access analisa o recurso, o `businesFlowTemplate` representa um modelo de fluxo de negócios do Azure AD. O identificador de um modelo, por exemplo, para revisar os membros de convidado de um grupo, é fornecido pelo chamador ao criar uma revisão de acesso.
ms.openlocfilehash: 8faf1a1381f5cdcf4bfaab78adc7a6554479b427
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039876"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="9a039-104">tipo de recurso de businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="9a039-104">businessFlowTemplate resource type</span></span>

> <span data-ttu-id="9a039-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9a039-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a039-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9a039-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a039-107">No recurso de [acesso analisa](accessreviews-root.md) Azure AD, o `businesFlowTemplate` representa um modelo de fluxo de negócios do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9a039-107">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="9a039-108">O identificador de um modelo, por exemplo, para revisar os membros de convidado de um grupo, é fornecido pelo chamador ao criar uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="9a039-108">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="9a039-109">Os objetos de modelo de fluxo de negócios são gerados automaticamente quando o onboards administrador global locatário para usar o access revisa o recurso.</span><span class="sxs-lookup"><span data-stu-id="9a039-109">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="9a039-110">Nenhum modelo de fluxo de negócios adicionais pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="9a039-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="9a039-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="9a039-111">Methods</span></span>

| <span data-ttu-id="9a039-112">Método</span><span class="sxs-lookup"><span data-stu-id="9a039-112">Method</span></span>           | <span data-ttu-id="9a039-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9a039-113">Return Type</span></span>    |<span data-ttu-id="9a039-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a039-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9a039-115">Lista businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="9a039-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="9a039-116">coleção [businessFlowTemplate](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="9a039-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="9a039-117">Obtenha os modelos de fluxo de negócios apropriado para acessar as revisões.</span><span class="sxs-lookup"><span data-stu-id="9a039-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="9a039-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a039-118">Properties</span></span>
| <span data-ttu-id="9a039-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a039-119">Property</span></span>     | <span data-ttu-id="9a039-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a039-120">Type</span></span>   |<span data-ttu-id="9a039-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a039-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="9a039-122">O identificador atribuído pelo recurso de modelo de fluxo de negócio</span><span class="sxs-lookup"><span data-stu-id="9a039-122">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="9a039-123">O nome do modelo de fluxo de negócio</span><span class="sxs-lookup"><span data-stu-id="9a039-123">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="9a039-124">Relações</span><span class="sxs-lookup"><span data-stu-id="9a039-124">Relationships</span></span>

<span data-ttu-id="9a039-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9a039-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="9a039-126">Ver também</span><span class="sxs-lookup"><span data-stu-id="9a039-126">See also</span></span>

| <span data-ttu-id="9a039-127">Método</span><span class="sxs-lookup"><span data-stu-id="9a039-127">Method</span></span>           | <span data-ttu-id="9a039-128">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9a039-128">Return Type</span></span>    |<span data-ttu-id="9a039-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a039-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9a039-130">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="9a039-130">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="9a039-131">accessReview</span><span class="sxs-lookup"><span data-stu-id="9a039-131">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="9a039-132">Crie um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="9a039-132">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9a039-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a039-133">JSON representation</span></span>

<span data-ttu-id="9a039-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a039-134">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
