---
title: tipo de recurso programControlType
description: 'No recurso de revisões do Azure AD Access, o tipo de controle do programa é usado ao associar um controle a um programa, para indicar o tipo de revisão do Access para o qual o controle é.  '
localization_priority: Normal
ms.openlocfilehash: 489fa6e5cac31165fec9f7ce9939d58fa84cb1ab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344035"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="4afba-103">tipo de recurso programControlType</span><span class="sxs-lookup"><span data-stu-id="4afba-103">programControlType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4afba-104">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , o tipo de controle do programa é usado ao associar um controle a um programa, para indicar o tipo de revisão do Access para o qual o controle é.</span><span class="sxs-lookup"><span data-stu-id="4afba-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="4afba-105">Os objetos de tipo de controle do programa são gerados automaticamente quando o administrador global embuti o locatário para usar o recurso de revisões do Access.</span><span class="sxs-lookup"><span data-stu-id="4afba-105">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="4afba-106">Nenhum tipo de controle de programa adicional pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="4afba-106">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="4afba-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4afba-107">Methods</span></span>

| <span data-ttu-id="4afba-108">Método</span><span class="sxs-lookup"><span data-stu-id="4afba-108">Method</span></span>           | <span data-ttu-id="4afba-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4afba-109">Return Type</span></span>    |<span data-ttu-id="4afba-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4afba-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4afba-111">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="4afba-111">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="4afba-112">coleção [programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="4afba-112">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="4afba-113">Listar tipos de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="4afba-113">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="4afba-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4afba-114">Properties</span></span>
| <span data-ttu-id="4afba-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4afba-115">Property</span></span>     | <span data-ttu-id="4afba-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="4afba-116">Type</span></span>   |<span data-ttu-id="4afba-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="4afba-117">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="4afba-118">O identificador atribuído ao recurso do tipo de controle do programa</span><span class="sxs-lookup"><span data-stu-id="4afba-118">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="4afba-119">O nome do tipo de controle do programa</span><span class="sxs-lookup"><span data-stu-id="4afba-119">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="4afba-120">Relações</span><span class="sxs-lookup"><span data-stu-id="4afba-120">Relationships</span></span>

<span data-ttu-id="4afba-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4afba-121">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="4afba-122">Ver também</span><span class="sxs-lookup"><span data-stu-id="4afba-122">See also</span></span>

| <span data-ttu-id="4afba-123">Método</span><span class="sxs-lookup"><span data-stu-id="4afba-123">Method</span></span>           | <span data-ttu-id="4afba-124">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4afba-124">Return Type</span></span>    |<span data-ttu-id="4afba-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="4afba-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4afba-126">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="4afba-126">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="4afba-127">programControl</span><span class="sxs-lookup"><span data-stu-id="4afba-127">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="4afba-128">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="4afba-128">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4afba-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4afba-129">JSON representation</span></span>

<span data-ttu-id="4afba-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4afba-130">Here is a JSON representation of the resource.</span></span>

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
