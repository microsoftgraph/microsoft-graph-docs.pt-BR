---
title: Tipo de recurso businessFlowTemplate
description: No recurso de revisões de acesso do Azure AD, o representa um modelo de fluxo de negócios do `businesFlowTemplate` Azure AD. O identificador de um modelo, como para revisar membros convidados de um grupo, é fornecido pelo chamador ao criar uma revisão de acesso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: b1fce9de1c2f21d4a5c918985028acfee50dc390
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751241"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="dc594-104">Tipo de recurso businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="dc594-104">businessFlowTemplate resource type</span></span>

<span data-ttu-id="dc594-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc594-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc594-106">No recurso de análises de acesso do Azure [AD,](accessreviews-root.md) **o businesFlowTemplate** representa um modelo de fluxo de negócios do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dc594-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the **businesFlowTemplate** represents an Azure AD business flow template.</span></span> <span data-ttu-id="dc594-107">O identificador de um modelo, como para revisar membros convidados de um grupo, é fornecido pelo chamador ao criar uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="dc594-107">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="dc594-108">Os objetos do modelo de fluxo de negócios são gerados automaticamente quando o administrador global integra o locatário para usar o recurso de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="dc594-108">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="dc594-109">Os modelos de fluxo de negócios incluem revisões de acesso de atribuições a um aplicativo, associações de um grupo, associações de uma função do Azure AD, associações de usuários convidados de um grupo e atribuições de usuário convidado a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc594-109">The business flow templates include access reviews of assignments to an application, memberships of a group, memberships of an Azure AD role, guest user memberships of a group, and guest user assignments to an application.</span></span> <span data-ttu-id="dc594-110">Nenhum modelo de fluxo comercial adicional pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="dc594-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="dc594-111">Methods</span><span class="sxs-lookup"><span data-stu-id="dc594-111">Methods</span></span>

| <span data-ttu-id="dc594-112">Método</span><span class="sxs-lookup"><span data-stu-id="dc594-112">Method</span></span>           | <span data-ttu-id="dc594-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dc594-113">Return Type</span></span>    |<span data-ttu-id="dc594-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc594-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dc594-115">Listar businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="dc594-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="dc594-116">[Coleção businessFlowTemplate](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="dc594-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="dc594-117">Obter os modelos de fluxo de negócios apropriados para acessar avaliações.</span><span class="sxs-lookup"><span data-stu-id="dc594-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc594-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc594-118">Properties</span></span>
| <span data-ttu-id="dc594-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc594-119">Property</span></span>     | <span data-ttu-id="dc594-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc594-120">Type</span></span>   |<span data-ttu-id="dc594-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc594-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dc594-122">id</span><span class="sxs-lookup"><span data-stu-id="dc594-122">id</span></span>                     |<span data-ttu-id="dc594-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc594-123">String</span></span>                | <span data-ttu-id="dc594-124">O identificador atribuído ao recurso do modelo de fluxo de negócios.</span><span class="sxs-lookup"><span data-stu-id="dc594-124">The feature-assigned identifier of the business flow template.</span></span> <span data-ttu-id="dc594-125">Esses valores são sensíveis a minúsculas.</span><span class="sxs-lookup"><span data-stu-id="dc594-125">These values are case sensitive.</span></span>                                      |
| <span data-ttu-id="dc594-126">displayName</span><span class="sxs-lookup"><span data-stu-id="dc594-126">displayName</span></span>            |<span data-ttu-id="dc594-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc594-127">String</span></span>                | <span data-ttu-id="dc594-128">O nome do modelo de fluxo comercial</span><span class="sxs-lookup"><span data-stu-id="dc594-128">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="dc594-129">Relações</span><span class="sxs-lookup"><span data-stu-id="dc594-129">Relationships</span></span>

<span data-ttu-id="dc594-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dc594-130">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="dc594-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="dc594-131">See also</span></span>

| <span data-ttu-id="dc594-132">Método</span><span class="sxs-lookup"><span data-stu-id="dc594-132">Method</span></span>           | <span data-ttu-id="dc594-133">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dc594-133">Return Type</span></span>    |<span data-ttu-id="dc594-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc594-134">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dc594-135">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="dc594-135">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="dc594-136">accessReview</span><span class="sxs-lookup"><span data-stu-id="dc594-136">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="dc594-137">Crie um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="dc594-137">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="dc594-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc594-138">JSON representation</span></span>

<span data-ttu-id="dc594-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc594-139">Here is a JSON representation of the resource.</span></span>

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


