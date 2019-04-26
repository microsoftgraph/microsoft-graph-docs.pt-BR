---
title: tipo de recurso informationalUrl
description: Informações de perfil básicas do aplicativo.
localization_priority: Normal
ms.openlocfilehash: c858bb55db083510661edfc36f32b9a511c5e6f3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339986"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="75129-103">tipo de recurso informationalUrl</span><span class="sxs-lookup"><span data-stu-id="75129-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75129-104">Informações de perfil básicas do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75129-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="75129-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75129-105">Properties</span></span>

| <span data-ttu-id="75129-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75129-106">Property</span></span> | <span data-ttu-id="75129-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="75129-107">Type</span></span> | <span data-ttu-id="75129-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="75129-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="75129-109">Marketing</span><span class="sxs-lookup"><span data-stu-id="75129-109">marketing</span></span>|<span data-ttu-id="75129-110">String</span><span class="sxs-lookup"><span data-stu-id="75129-110">String</span></span>| <span data-ttu-id="75129-111">Link para a página de marketing do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75129-111">Link to the application's marketing page.</span></span> <span data-ttu-id="75129-112">Por exemplo, https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="75129-112">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="75129-113">declaração</span><span class="sxs-lookup"><span data-stu-id="75129-113">privacy</span></span>|<span data-ttu-id="75129-114">String</span><span class="sxs-lookup"><span data-stu-id="75129-114">String</span></span>| <span data-ttu-id="75129-115">Link para a política de privacidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75129-115">Link to the application's privacy statement.</span></span> <span data-ttu-id="75129-116">Por exemplo, https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="75129-116">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="75129-117">à</span><span class="sxs-lookup"><span data-stu-id="75129-117">support</span></span>|<span data-ttu-id="75129-118">String</span><span class="sxs-lookup"><span data-stu-id="75129-118">String</span></span>| <span data-ttu-id="75129-119">Link para a página de suporte do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75129-119">Link to the application's support page.</span></span> <span data-ttu-id="75129-120">Por exemplo, https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="75129-120">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="75129-121">termsOfService</span><span class="sxs-lookup"><span data-stu-id="75129-121">termsOfService</span></span>|<span data-ttu-id="75129-122">String</span><span class="sxs-lookup"><span data-stu-id="75129-122">String</span></span>| <span data-ttu-id="75129-123">Link para a instrução de termos de serviço do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75129-123">Link to the application's terms of service statement.</span></span> <span data-ttu-id="75129-124">Por exemplo, https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="75129-124">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="75129-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75129-125">JSON representation</span></span>
<span data-ttu-id="75129-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75129-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "marketing": "String",
  "privacy": "String",
  "support": "String",
  "termsOfService": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
