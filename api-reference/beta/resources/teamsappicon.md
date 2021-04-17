---
title: Tipo de recurso teamsAppIcon
description: Um ícone associado a um aplicativo no Microsoft Teams.
author: jecha
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3e8a256dc0b9e92c414cd3d362bb36579708083f
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882638"
---
# <a name="teamsappicon-resource-type"></a><span data-ttu-id="06189-103">Tipo de recurso teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="06189-103">teamsAppIcon resource type</span></span>

<span data-ttu-id="06189-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06189-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06189-105">Um ícone associado a um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="06189-105">An icon associated with a [teamsApp](teamsapp.md).</span></span>

## <a name="methods"></a><span data-ttu-id="06189-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="06189-106">Methods</span></span>

| <span data-ttu-id="06189-107">Método</span><span class="sxs-lookup"><span data-stu-id="06189-107">Method</span></span>                                            | <span data-ttu-id="06189-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="06189-108">Return Type</span></span>                                       | <span data-ttu-id="06189-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="06189-109">Description</span></span>                                                    | 
| :------------------------------------------------ | :------------------------------------------------ | :------------------------------------------------------------- |
| [<span data-ttu-id="06189-110">Obter ícone</span><span class="sxs-lookup"><span data-stu-id="06189-110">Get icon</span></span>](../api/teamsappicon-get.md)     | [<span data-ttu-id="06189-111">teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="06189-111">teamsAppIcon</span></span>](teamsappicon.md)                   | <span data-ttu-id="06189-112">Obter um ícone associado a uma versão específica de um aplicativo do Teams.</span><span class="sxs-lookup"><span data-stu-id="06189-112">Get an icon associated with a specific version of a Teams app.</span></span> |
| [<span data-ttu-id="06189-113">Obter conteúdo hospedado</span><span class="sxs-lookup"><span data-stu-id="06189-113">Get hosted content</span></span>](../api/teamworkhostedcontent-get.md) | [<span data-ttu-id="06189-114">teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="06189-114">teamworkHostedContent</span></span>](teamworkhostedcontent.md) | <span data-ttu-id="06189-115">Obter conteúdo hospedado (e seus bytes) para um ícone.</span><span class="sxs-lookup"><span data-stu-id="06189-115">Get hosted content (and its bytes) for an icon.</span></span>                |

## <a name="properties"></a><span data-ttu-id="06189-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06189-116">Properties</span></span>

| <span data-ttu-id="06189-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06189-117">Property</span></span>      | <span data-ttu-id="06189-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="06189-118">Type</span></span>                        | <span data-ttu-id="06189-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="06189-119">Description</span></span>                                                                             |
| :------------ | :-------------------------- | :-------------------------------------------------------------------------------------- |
| <span data-ttu-id="06189-120">id</span><span class="sxs-lookup"><span data-stu-id="06189-120">id</span></span>            | <span data-ttu-id="06189-121">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06189-121">string</span></span>                      | <span data-ttu-id="06189-122">A ID exclusiva do ícone do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06189-122">The unique ID of the app icon.</span></span>                                                          |
| <span data-ttu-id="06189-123">webUrl</span><span class="sxs-lookup"><span data-stu-id="06189-123">webUrl</span></span>        | <span data-ttu-id="06189-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06189-124">string</span></span>                      | <span data-ttu-id="06189-125">A URL da Web que pode ser usada para baixar a imagem.</span><span class="sxs-lookup"><span data-stu-id="06189-125">The web URL that can be used for downloading the image.</span></span>                                 |

## <a name="relationships"></a><span data-ttu-id="06189-126">Relações</span><span class="sxs-lookup"><span data-stu-id="06189-126">Relationships</span></span>

| <span data-ttu-id="06189-127">Relação</span><span class="sxs-lookup"><span data-stu-id="06189-127">Relationship</span></span>  | <span data-ttu-id="06189-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="06189-128">Type</span></span>                                              | <span data-ttu-id="06189-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="06189-129">Description</span></span>                                                                         |
| :------------ | :------------------------------------------------ | :---------------------------------------------------------------------------------- |
| <span data-ttu-id="06189-130">hostedContent</span><span class="sxs-lookup"><span data-stu-id="06189-130">hostedContent</span></span> | [<span data-ttu-id="06189-131">teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="06189-131">teamworkHostedContent</span></span>](teamworkhostedcontent.md) | <span data-ttu-id="06189-132">O conteúdo do ícone do aplicativo se o ícone estiver hospedado na infraestrutura do Teams.</span><span class="sxs-lookup"><span data-stu-id="06189-132">The contents of the app icon if the icon is hosted within the Teams infrastructure.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="06189-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06189-133">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppIcon",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "webUrl": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="06189-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="06189-134">See also</span></span>

- [<span data-ttu-id="06189-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="06189-135">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="06189-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="06189-136">teamsAppDefinition</span></span>](teamsappdefinition.md)
