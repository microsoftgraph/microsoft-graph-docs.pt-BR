---
title: tipo de recurso programControlType
description: 'No recurso de revisões do Azure AD Access, o tipo de controle do programa é usado ao associar um controle a um programa, para indicar o tipo de revisão do Access para o qual o controle é.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: ddf5ee29c01770d06c9725413f362bd0f0e18bee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029055"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="f2476-103">tipo de recurso programControlType</span><span class="sxs-lookup"><span data-stu-id="f2476-103">programControlType resource type</span></span>

<span data-ttu-id="f2476-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2476-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2476-105">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , o tipo de controle do programa é usado ao associar um controle a um programa, para indicar o tipo de revisão do Access para o qual o controle é.</span><span class="sxs-lookup"><span data-stu-id="f2476-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="f2476-106">Os objetos de tipo de controle do programa são gerados automaticamente quando o administrador global embuti o locatário para usar o recurso de revisões do Access.</span><span class="sxs-lookup"><span data-stu-id="f2476-106">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="f2476-107">Nenhum tipo de controle de programa adicional pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="f2476-107">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="f2476-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="f2476-108">Methods</span></span>

| <span data-ttu-id="f2476-109">Método</span><span class="sxs-lookup"><span data-stu-id="f2476-109">Method</span></span>           | <span data-ttu-id="f2476-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f2476-110">Return Type</span></span>    |<span data-ttu-id="f2476-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2476-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2476-112">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="f2476-112">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="f2476-113">coleção [programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="f2476-113">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="f2476-114">Listar tipos de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="f2476-114">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="f2476-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2476-115">Properties</span></span>
| <span data-ttu-id="f2476-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2476-116">Property</span></span>     | <span data-ttu-id="f2476-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2476-117">Type</span></span>   |<span data-ttu-id="f2476-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2476-118">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="f2476-119">O identificador atribuído ao recurso do tipo de controle do programa</span><span class="sxs-lookup"><span data-stu-id="f2476-119">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="f2476-120">O nome do tipo de controle do programa</span><span class="sxs-lookup"><span data-stu-id="f2476-120">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="f2476-121">Relações</span><span class="sxs-lookup"><span data-stu-id="f2476-121">Relationships</span></span>

<span data-ttu-id="f2476-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2476-122">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="f2476-123">Ver também</span><span class="sxs-lookup"><span data-stu-id="f2476-123">See also</span></span>

| <span data-ttu-id="f2476-124">Método</span><span class="sxs-lookup"><span data-stu-id="f2476-124">Method</span></span>           | <span data-ttu-id="f2476-125">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f2476-125">Return Type</span></span>    |<span data-ttu-id="f2476-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2476-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2476-127">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="f2476-127">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="f2476-128">programControl</span><span class="sxs-lookup"><span data-stu-id="f2476-128">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="f2476-129">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="f2476-129">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f2476-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2476-130">JSON representation</span></span>

<span data-ttu-id="f2476-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2476-131">Here is a JSON representation of the resource.</span></span>

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


