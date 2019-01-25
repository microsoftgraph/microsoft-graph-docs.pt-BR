---
title: tipo de recurso de programControlType
description: 'No Windows Azure AD access analisa o recurso, o tipo de controle do programa é usado quando a associação de um controle a um programa, para indicar o tipo da revisão do acesso de controle se destina.  '
localization_priority: Normal
ms.openlocfilehash: 8b17a0f30fbdceb6b6da24d5cbe972223acb29b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519700"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="7511a-103">tipo de recurso de programControlType</span><span class="sxs-lookup"><span data-stu-id="7511a-103">programControlType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7511a-104">No recurso de [acesso analisa](accessreviews-root.md) Azure AD, o tipo de controle do programa é usado quando a associação de um controle a um programa, para indicar o tipo de revisão de acesso, que o controle se destina.</span><span class="sxs-lookup"><span data-stu-id="7511a-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="7511a-105">Os objetos de tipo de controle do programa são gerados automaticamente quando o onboards administrador global locatário para usar o access revisa o recurso.</span><span class="sxs-lookup"><span data-stu-id="7511a-105">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="7511a-106">Não há tipos de controle de programa adicionais podem ser criados.</span><span class="sxs-lookup"><span data-stu-id="7511a-106">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="7511a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="7511a-107">Methods</span></span>

| <span data-ttu-id="7511a-108">Método</span><span class="sxs-lookup"><span data-stu-id="7511a-108">Method</span></span>           | <span data-ttu-id="7511a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7511a-109">Return Type</span></span>    |<span data-ttu-id="7511a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7511a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7511a-111">Lista programControlTypes</span><span class="sxs-lookup"><span data-stu-id="7511a-111">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="7511a-112">coleção [programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="7511a-112">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="7511a-113">Lista os tipos de controle do programa.</span><span class="sxs-lookup"><span data-stu-id="7511a-113">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="7511a-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7511a-114">Properties</span></span>
| <span data-ttu-id="7511a-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7511a-115">Property</span></span>     | <span data-ttu-id="7511a-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="7511a-116">Type</span></span>   |<span data-ttu-id="7511a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="7511a-117">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="7511a-118">O identificador atribuído pelo recurso do tipo de controle de programa</span><span class="sxs-lookup"><span data-stu-id="7511a-118">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="7511a-119">O nome do tipo de controle de programa</span><span class="sxs-lookup"><span data-stu-id="7511a-119">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="7511a-120">Relações</span><span class="sxs-lookup"><span data-stu-id="7511a-120">Relationships</span></span>

<span data-ttu-id="7511a-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7511a-121">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="7511a-122">Ver também</span><span class="sxs-lookup"><span data-stu-id="7511a-122">See also</span></span>

| <span data-ttu-id="7511a-123">Método</span><span class="sxs-lookup"><span data-stu-id="7511a-123">Method</span></span>           | <span data-ttu-id="7511a-124">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7511a-124">Return Type</span></span>    |<span data-ttu-id="7511a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7511a-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7511a-126">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="7511a-126">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="7511a-127">programControl</span><span class="sxs-lookup"><span data-stu-id="7511a-127">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="7511a-128">Adicione um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="7511a-128">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7511a-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7511a-129">JSON representation</span></span>

<span data-ttu-id="7511a-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7511a-130">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/programcontroltype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
