---
title: Tipo de recurso businessFlowTemplate
description: No recurso de revisões de acesso do Azure AD, o representa um modelo de fluxo de negócios do `businesFlowTemplate` Azure AD. O identificador de um modelo, como para revisar membros convidados de um grupo, é fornecido pelo chamador ao criar uma revisão de acesso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 95a2723ee20777989ed1576d02c69adc649555ed
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433142"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="d6d83-104">Tipo de recurso businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="d6d83-104">businessFlowTemplate resource type</span></span>

<span data-ttu-id="d6d83-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6d83-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6d83-106">No recurso de revisões de acesso do Azure [AD,](accessreviews-root.md) o representa um modelo de fluxo de negócios do `businesFlowTemplate` Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d6d83-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="d6d83-107">O identificador de um modelo, como para revisar membros convidados de um grupo, é fornecido pelo chamador ao criar uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="d6d83-107">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="d6d83-108">Os objetos do modelo de fluxo de negócios são gerados automaticamente quando o administrador global integra o locatário para usar o recurso de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="d6d83-108">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="d6d83-109">Os modelos de fluxo de negócios incluem revisões de acesso de atribuições a um aplicativo, associações de um grupo, associações de uma função do Azure AD, associações de usuários convidados de um grupo e atribuições de usuário convidado a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d6d83-109">The business flow templates include access reviews of assignments to an application, memberships of a group, memberships of an Azure AD role, guest user memberships of a group, and guest user assignments to an application.</span></span> <span data-ttu-id="d6d83-110">Nenhum modelo de fluxo comercial adicional pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="d6d83-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="d6d83-111">Methods</span><span class="sxs-lookup"><span data-stu-id="d6d83-111">Methods</span></span>

| <span data-ttu-id="d6d83-112">Método</span><span class="sxs-lookup"><span data-stu-id="d6d83-112">Method</span></span>           | <span data-ttu-id="d6d83-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d6d83-113">Return Type</span></span>    |<span data-ttu-id="d6d83-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6d83-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d6d83-115">Listar businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="d6d83-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="d6d83-116">[Coleção businessFlowTemplate](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="d6d83-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="d6d83-117">Obter os modelos de fluxo de negócios apropriados para acessar avaliações.</span><span class="sxs-lookup"><span data-stu-id="d6d83-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="d6d83-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6d83-118">Properties</span></span>
| <span data-ttu-id="d6d83-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6d83-119">Property</span></span>     | <span data-ttu-id="d6d83-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6d83-120">Type</span></span>   |<span data-ttu-id="d6d83-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6d83-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="d6d83-122">O identificador atribuído ao recurso do modelo de fluxo de negócios.</span><span class="sxs-lookup"><span data-stu-id="d6d83-122">The feature-assigned identifier of the business flow template.</span></span> <span data-ttu-id="d6d83-123">Esses valores são sensíveis a minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d6d83-123">These values are case sensitive.</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="d6d83-124">O nome do modelo de fluxo comercial</span><span class="sxs-lookup"><span data-stu-id="d6d83-124">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="d6d83-125">Relações</span><span class="sxs-lookup"><span data-stu-id="d6d83-125">Relationships</span></span>

<span data-ttu-id="d6d83-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6d83-126">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="d6d83-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="d6d83-127">See also</span></span>

| <span data-ttu-id="d6d83-128">Método</span><span class="sxs-lookup"><span data-stu-id="d6d83-128">Method</span></span>           | <span data-ttu-id="d6d83-129">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d6d83-129">Return Type</span></span>    |<span data-ttu-id="d6d83-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6d83-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d6d83-131">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="d6d83-131">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="d6d83-132">accessReview</span><span class="sxs-lookup"><span data-stu-id="d6d83-132">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="d6d83-133">Crie um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="d6d83-133">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d6d83-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6d83-134">JSON representation</span></span>

<span data-ttu-id="d6d83-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6d83-135">Here is a JSON representation of the resource.</span></span>

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


