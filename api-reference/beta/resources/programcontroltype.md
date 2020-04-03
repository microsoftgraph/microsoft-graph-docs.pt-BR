---
title: tipo de recurso programControlType
description: 'No recurso de revisões do Azure AD Access, o tipo de controle do programa é usado ao associar um controle a um programa, para indicar o tipo de revisão do Access para o qual o controle é.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 7321e4394e5e2a87d4ff51f71bc1589b5e1688cb
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125299"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="ba82f-103">tipo de recurso programControlType</span><span class="sxs-lookup"><span data-stu-id="ba82f-103">programControlType resource type</span></span>

<span data-ttu-id="ba82f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba82f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba82f-105">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , o tipo de controle do programa é usado ao associar um controle a um programa, para indicar o tipo de revisão do Access para o qual o controle é.</span><span class="sxs-lookup"><span data-stu-id="ba82f-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="ba82f-106">Os objetos de tipo de controle do programa são gerados automaticamente quando o administrador global embuti o locatário para usar o recurso de revisões do Access.</span><span class="sxs-lookup"><span data-stu-id="ba82f-106">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="ba82f-107">Nenhum tipo de controle de programa adicional pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="ba82f-107">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="ba82f-108">Methods</span><span class="sxs-lookup"><span data-stu-id="ba82f-108">Methods</span></span>

| <span data-ttu-id="ba82f-109">Método</span><span class="sxs-lookup"><span data-stu-id="ba82f-109">Method</span></span>           | <span data-ttu-id="ba82f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ba82f-110">Return Type</span></span>    |<span data-ttu-id="ba82f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba82f-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ba82f-112">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="ba82f-112">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="ba82f-113">coleção [programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="ba82f-113">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="ba82f-114">Listar tipos de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="ba82f-114">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="ba82f-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba82f-115">Properties</span></span>
| <span data-ttu-id="ba82f-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba82f-116">Property</span></span>     | <span data-ttu-id="ba82f-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba82f-117">Type</span></span>   |<span data-ttu-id="ba82f-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba82f-118">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="ba82f-119">O identificador atribuído ao recurso do tipo de controle do programa</span><span class="sxs-lookup"><span data-stu-id="ba82f-119">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="ba82f-120">O nome do tipo de controle do programa</span><span class="sxs-lookup"><span data-stu-id="ba82f-120">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="ba82f-121">Relações</span><span class="sxs-lookup"><span data-stu-id="ba82f-121">Relationships</span></span>

<span data-ttu-id="ba82f-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba82f-122">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="ba82f-123">Ver também</span><span class="sxs-lookup"><span data-stu-id="ba82f-123">See also</span></span>

| <span data-ttu-id="ba82f-124">Método</span><span class="sxs-lookup"><span data-stu-id="ba82f-124">Method</span></span>           | <span data-ttu-id="ba82f-125">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ba82f-125">Return Type</span></span>    |<span data-ttu-id="ba82f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba82f-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ba82f-127">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="ba82f-127">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="ba82f-128">programControl</span><span class="sxs-lookup"><span data-stu-id="ba82f-128">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="ba82f-129">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="ba82f-129">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ba82f-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba82f-130">JSON representation</span></span>

<span data-ttu-id="ba82f-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba82f-131">Here is a JSON representation of the resource.</span></span>

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
