---
title: tipo de recurso businessFlowTemplate
description: No recurso de revisões do Azure AD Access, `businesFlowTemplate` o representa um modelo de fluxo de negócios do Azure AD. O identificador de um modelo, como a análise de membros convidados de um grupo, é fornecido pelo chamador durante a criação de uma revisão do Access.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: markwahl-msft
ms.openlocfilehash: 00075813d011f6c6e66e0c853bfad6545bbc8c97
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507856"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="d4187-104">tipo de recurso businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="d4187-104">businessFlowTemplate resource type</span></span>

<span data-ttu-id="d4187-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d4187-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4187-106">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , `businesFlowTemplate` o representa um modelo de fluxo de negócios do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d4187-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="d4187-107">O identificador de um modelo, como a análise de membros convidados de um grupo, é fornecido pelo chamador durante a criação de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="d4187-107">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="d4187-108">Os objetos do modelo de fluxo de negócios são gerados automaticamente quando o administrador global embuti o locatário para usar o recurso de revisões do Access.</span><span class="sxs-lookup"><span data-stu-id="d4187-108">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="d4187-109">Os modelos de fluxo de negócios incluem revisões de acesso de atribuições para um aplicativo, associações de um grupo, associações de uma função do Azure AD, associações de usuários convidados de um grupo e atribuições de usuários convidados a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d4187-109">The business flow templates include access reviews of assignments to an application, memberships of a group, memberships of an Azure AD role, guest user memberships of a group, and guest user assignments to an application.</span></span> <span data-ttu-id="d4187-110">Nenhum modelo de fluxo de negócios adicional pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="d4187-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="d4187-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="d4187-111">Methods</span></span>

| <span data-ttu-id="d4187-112">Método</span><span class="sxs-lookup"><span data-stu-id="d4187-112">Method</span></span>           | <span data-ttu-id="d4187-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d4187-113">Return Type</span></span>    |<span data-ttu-id="d4187-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4187-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4187-115">Listar businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="d4187-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="d4187-116">coleção [businessFlowTemplate](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="d4187-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="d4187-117">Obtenha os modelos de fluxo de negócios apropriados para as revisões do Access.</span><span class="sxs-lookup"><span data-stu-id="d4187-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4187-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4187-118">Properties</span></span>
| <span data-ttu-id="d4187-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4187-119">Property</span></span>     | <span data-ttu-id="d4187-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4187-120">Type</span></span>   |<span data-ttu-id="d4187-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4187-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="d4187-122">O identificador atribuído ao recurso do modelo de fluxo de negócios.</span><span class="sxs-lookup"><span data-stu-id="d4187-122">The feature-assigned identifier of the business flow template.</span></span> <span data-ttu-id="d4187-123">Esses valores diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d4187-123">These values are case sensitive.</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="d4187-124">O nome do modelo de fluxo de negócios</span><span class="sxs-lookup"><span data-stu-id="d4187-124">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="d4187-125">Relações</span><span class="sxs-lookup"><span data-stu-id="d4187-125">Relationships</span></span>

<span data-ttu-id="d4187-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4187-126">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="d4187-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="d4187-127">See also</span></span>

| <span data-ttu-id="d4187-128">Método</span><span class="sxs-lookup"><span data-stu-id="d4187-128">Method</span></span>           | <span data-ttu-id="d4187-129">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d4187-129">Return Type</span></span>    |<span data-ttu-id="d4187-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4187-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4187-131">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="d4187-131">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="d4187-132">accessReview</span><span class="sxs-lookup"><span data-stu-id="d4187-132">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="d4187-133">Criar um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="d4187-133">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d4187-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4187-134">JSON representation</span></span>

<span data-ttu-id="d4187-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4187-135">Here is a JSON representation of the resource.</span></span>

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
