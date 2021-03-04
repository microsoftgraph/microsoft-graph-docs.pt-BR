---
title: Tipo de recurso programControlType
description: 'No recurso de revisões de acesso do Azure AD, o tipo de controle de programa é usado ao associar um controle a um programa, para indicar o tipo de revisão de acesso para o qual o controle se trata.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 593d8a8fa36c03515dbad9a1ee1dd0b267f98577
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443941"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="18b67-103">Tipo de recurso programControlType</span><span class="sxs-lookup"><span data-stu-id="18b67-103">programControlType resource type</span></span>

<span data-ttu-id="18b67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18b67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18b67-105">No recurso de revisões de acesso do Azure [AD,](accessreviews-root.md) o tipo de controle de programa é usado ao associar um controle a um programa, para indicar o tipo de revisão de acesso para o qual o controle se trata.</span><span class="sxs-lookup"><span data-stu-id="18b67-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="18b67-106">Os objetos do tipo de controle do programa são gerados automaticamente quando o administrador global inscarda o locatário para usar o recurso de críticas de acesso.</span><span class="sxs-lookup"><span data-stu-id="18b67-106">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="18b67-107">Nenhum tipo de controle de programa adicional pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="18b67-107">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="18b67-108">Methods</span><span class="sxs-lookup"><span data-stu-id="18b67-108">Methods</span></span>

| <span data-ttu-id="18b67-109">Método</span><span class="sxs-lookup"><span data-stu-id="18b67-109">Method</span></span>           | <span data-ttu-id="18b67-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="18b67-110">Return Type</span></span>    |<span data-ttu-id="18b67-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="18b67-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18b67-112">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="18b67-112">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="18b67-113">[Coleção programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="18b67-113">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="18b67-114">Listar tipos de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="18b67-114">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="18b67-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18b67-115">Properties</span></span>
| <span data-ttu-id="18b67-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18b67-116">Property</span></span>     | <span data-ttu-id="18b67-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="18b67-117">Type</span></span>   |<span data-ttu-id="18b67-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="18b67-118">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="18b67-119">O identificador atribuído ao recurso do tipo de controle do programa</span><span class="sxs-lookup"><span data-stu-id="18b67-119">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="18b67-120">O nome do tipo de controle do programa</span><span class="sxs-lookup"><span data-stu-id="18b67-120">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="18b67-121">Relações</span><span class="sxs-lookup"><span data-stu-id="18b67-121">Relationships</span></span>

<span data-ttu-id="18b67-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18b67-122">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="18b67-123">Ver também</span><span class="sxs-lookup"><span data-stu-id="18b67-123">See also</span></span>

| <span data-ttu-id="18b67-124">Método</span><span class="sxs-lookup"><span data-stu-id="18b67-124">Method</span></span>           | <span data-ttu-id="18b67-125">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="18b67-125">Return Type</span></span>    |<span data-ttu-id="18b67-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="18b67-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18b67-127">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="18b67-127">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="18b67-128">programControl</span><span class="sxs-lookup"><span data-stu-id="18b67-128">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="18b67-129">Adicione um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="18b67-129">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="18b67-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18b67-130">JSON representation</span></span>

<span data-ttu-id="18b67-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18b67-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControlType"
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
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


