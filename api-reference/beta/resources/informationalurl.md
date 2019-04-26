---
title: tipo de recurso informationalUrl
description: Informações de perfil básicas do aplicativo.
localization_priority: Normal
ms.openlocfilehash: 5085c144045631c530cbb66f5e1f27186a63b380
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548702"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="51b98-103">tipo de recurso informationalUrl</span><span class="sxs-lookup"><span data-stu-id="51b98-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51b98-104">Informações de perfil básicas do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51b98-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="51b98-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51b98-105">Properties</span></span>

| <span data-ttu-id="51b98-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51b98-106">Property</span></span> | <span data-ttu-id="51b98-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="51b98-107">Type</span></span> | <span data-ttu-id="51b98-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="51b98-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="51b98-109">Marketing</span><span class="sxs-lookup"><span data-stu-id="51b98-109">marketing</span></span>|<span data-ttu-id="51b98-110">String</span><span class="sxs-lookup"><span data-stu-id="51b98-110">String</span></span>| <span data-ttu-id="51b98-111">Link para a página de marketing do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51b98-111">Link to the application's marketing page.</span></span> <span data-ttu-id="51b98-112">Por exemplo, https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="51b98-112">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="51b98-113">declaração</span><span class="sxs-lookup"><span data-stu-id="51b98-113">privacy</span></span>|<span data-ttu-id="51b98-114">String</span><span class="sxs-lookup"><span data-stu-id="51b98-114">String</span></span>| <span data-ttu-id="51b98-115">Link para a política de privacidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51b98-115">Link to the application's privacy statement.</span></span> <span data-ttu-id="51b98-116">Por exemplo, https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="51b98-116">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="51b98-117">à</span><span class="sxs-lookup"><span data-stu-id="51b98-117">support</span></span>|<span data-ttu-id="51b98-118">String</span><span class="sxs-lookup"><span data-stu-id="51b98-118">String</span></span>| <span data-ttu-id="51b98-119">Link para a página de suporte do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51b98-119">Link to the application's support page.</span></span> <span data-ttu-id="51b98-120">Por exemplo, https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="51b98-120">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="51b98-121">termsOfService</span><span class="sxs-lookup"><span data-stu-id="51b98-121">termsOfService</span></span>|<span data-ttu-id="51b98-122">String</span><span class="sxs-lookup"><span data-stu-id="51b98-122">String</span></span>| <span data-ttu-id="51b98-123">Link para a instrução de termos de serviço do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51b98-123">Link to the application's terms of service statement.</span></span> <span data-ttu-id="51b98-124">Por exemplo, https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="51b98-124">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="51b98-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51b98-125">JSON representation</span></span>
<span data-ttu-id="51b98-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51b98-126">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/informationalurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
