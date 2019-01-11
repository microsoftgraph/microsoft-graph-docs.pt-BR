---
title: tipo de recurso de programControlType
description: 'No Windows Azure AD access analisa o recurso, o tipo de controle do programa é usado quando a associação de um controle a um programa, para indicar o tipo da revisão do acesso de controle se destina.  '
localization_priority: Normal
ms.openlocfilehash: 0091c23fd5d537e7c1fd62051778e56b510a3dab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808229"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="fb74d-103">tipo de recurso de programControlType</span><span class="sxs-lookup"><span data-stu-id="fb74d-103">programControlType resource type</span></span>

> <span data-ttu-id="fb74d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fb74d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb74d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fb74d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb74d-106">No recurso de [acesso analisa](accessreviews-root.md) Azure AD, o tipo de controle do programa é usado quando a associação de um controle a um programa, para indicar o tipo de revisão de acesso, que o controle se destina.</span><span class="sxs-lookup"><span data-stu-id="fb74d-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="fb74d-107">Os objetos de tipo de controle do programa são gerados automaticamente quando o onboards administrador global locatário para usar o access revisa o recurso.</span><span class="sxs-lookup"><span data-stu-id="fb74d-107">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="fb74d-108">Não há tipos de controle de programa adicionais podem ser criados.</span><span class="sxs-lookup"><span data-stu-id="fb74d-108">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="fb74d-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="fb74d-109">Methods</span></span>

| <span data-ttu-id="fb74d-110">Método</span><span class="sxs-lookup"><span data-stu-id="fb74d-110">Method</span></span>           | <span data-ttu-id="fb74d-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fb74d-111">Return Type</span></span>    |<span data-ttu-id="fb74d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb74d-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fb74d-113">Lista programControlTypes</span><span class="sxs-lookup"><span data-stu-id="fb74d-113">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="fb74d-114">coleção [programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="fb74d-114">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="fb74d-115">Lista os tipos de controle do programa.</span><span class="sxs-lookup"><span data-stu-id="fb74d-115">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="fb74d-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb74d-116">Properties</span></span>
| <span data-ttu-id="fb74d-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb74d-117">Property</span></span>     | <span data-ttu-id="fb74d-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb74d-118">Type</span></span>   |<span data-ttu-id="fb74d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb74d-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="fb74d-120">O identificador atribuído pelo recurso do tipo de controle de programa</span><span class="sxs-lookup"><span data-stu-id="fb74d-120">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="fb74d-121">O nome do tipo de controle de programa</span><span class="sxs-lookup"><span data-stu-id="fb74d-121">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="fb74d-122">Relações</span><span class="sxs-lookup"><span data-stu-id="fb74d-122">Relationships</span></span>

<span data-ttu-id="fb74d-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fb74d-123">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="fb74d-124">Ver também</span><span class="sxs-lookup"><span data-stu-id="fb74d-124">See also</span></span>

| <span data-ttu-id="fb74d-125">Método</span><span class="sxs-lookup"><span data-stu-id="fb74d-125">Method</span></span>           | <span data-ttu-id="fb74d-126">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fb74d-126">Return Type</span></span>    |<span data-ttu-id="fb74d-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb74d-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fb74d-128">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="fb74d-128">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="fb74d-129">programControl</span><span class="sxs-lookup"><span data-stu-id="fb74d-129">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="fb74d-130">Adicione um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="fb74d-130">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fb74d-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb74d-131">JSON representation</span></span>

<span data-ttu-id="fb74d-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb74d-132">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
