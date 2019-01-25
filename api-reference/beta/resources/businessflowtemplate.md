---
title: tipo de recurso de businessFlowTemplate
description: No Windows Azure AD access analisa o recurso, o `businesFlowTemplate` representa um modelo de fluxo de negócios do Azure AD. O identificador de um modelo, por exemplo, para revisar os membros de convidado de um grupo, é fornecido pelo chamador ao criar uma revisão de acesso.
localization_priority: Normal
ms.openlocfilehash: 567a7f499e2fb493f3ca519e312e69fb43fe3b79
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529576"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="50255-104">tipo de recurso de businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="50255-104">businessFlowTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50255-105">No recurso de [acesso analisa](accessreviews-root.md) Azure AD, o `businesFlowTemplate` representa um modelo de fluxo de negócios do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50255-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="50255-106">O identificador de um modelo, por exemplo, para revisar os membros de convidado de um grupo, é fornecido pelo chamador ao criar uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="50255-106">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="50255-107">Os objetos de modelo de fluxo de negócios são gerados automaticamente quando o onboards administrador global locatário para usar o access revisa o recurso.</span><span class="sxs-lookup"><span data-stu-id="50255-107">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="50255-108">Nenhum modelo de fluxo de negócios adicionais pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="50255-108">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="50255-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="50255-109">Methods</span></span>

| <span data-ttu-id="50255-110">Método</span><span class="sxs-lookup"><span data-stu-id="50255-110">Method</span></span>           | <span data-ttu-id="50255-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="50255-111">Return Type</span></span>    |<span data-ttu-id="50255-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="50255-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="50255-113">Lista businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="50255-113">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="50255-114">coleção [businessFlowTemplate](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="50255-114">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="50255-115">Obtenha os modelos de fluxo de negócios apropriado para acessar as revisões.</span><span class="sxs-lookup"><span data-stu-id="50255-115">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="50255-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50255-116">Properties</span></span>
| <span data-ttu-id="50255-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50255-117">Property</span></span>     | <span data-ttu-id="50255-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="50255-118">Type</span></span>   |<span data-ttu-id="50255-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="50255-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="50255-120">O identificador atribuído pelo recurso de modelo de fluxo de negócio</span><span class="sxs-lookup"><span data-stu-id="50255-120">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="50255-121">O nome do modelo de fluxo de negócio</span><span class="sxs-lookup"><span data-stu-id="50255-121">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="50255-122">Relações</span><span class="sxs-lookup"><span data-stu-id="50255-122">Relationships</span></span>

<span data-ttu-id="50255-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="50255-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="50255-124">Ver também</span><span class="sxs-lookup"><span data-stu-id="50255-124">See also</span></span>

| <span data-ttu-id="50255-125">Método</span><span class="sxs-lookup"><span data-stu-id="50255-125">Method</span></span>           | <span data-ttu-id="50255-126">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="50255-126">Return Type</span></span>    |<span data-ttu-id="50255-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="50255-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="50255-128">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="50255-128">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="50255-129">accessReview</span><span class="sxs-lookup"><span data-stu-id="50255-129">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="50255-130">Crie um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="50255-130">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="50255-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50255-131">JSON representation</span></span>

<span data-ttu-id="50255-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50255-132">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/businessflowtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
