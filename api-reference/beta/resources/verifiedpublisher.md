---
title: Tipo de recurso verifiedPublisher
description: Representa o editor verificado do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: 5acc66bd72c65b25d8301c4870fa5ff0f98a0d73
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135622"
---
# <a name="verifiedpublisher-resource-type"></a><span data-ttu-id="a8fe7-103">tipo de recurso verifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="a8fe7-103">verifiedPublisher resource type</span></span>

<span data-ttu-id="a8fe7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8fe7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8fe7-105">Representa um editor verificado de um [aplicativo](application.md).</span><span class="sxs-lookup"><span data-stu-id="a8fe7-105">Represents a verified publisher of an [application](application.md).</span></span> <span data-ttu-id="a8fe7-106">Para obter mais informações, consulte Verificação [do Publisher.](/azure/active-directory/develop/publisher-verification-overview)</span><span class="sxs-lookup"><span data-stu-id="a8fe7-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span> <span data-ttu-id="a8fe7-107">Os editores verificados são definidos usando [setVerifiedPublisher](../api/application-setverifiedpublisher.md) e só podem ser removidos usando [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).</span><span class="sxs-lookup"><span data-stu-id="a8fe7-107">Verified publishers are set using [setVerifiedPublisher](../api/application-setverifiedpublisher.md) and can only be removed using [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a8fe7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8fe7-108">Properties</span></span>

| <span data-ttu-id="a8fe7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8fe7-109">Property</span></span> | <span data-ttu-id="a8fe7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8fe7-110">Type</span></span> | <span data-ttu-id="a8fe7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8fe7-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a8fe7-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a8fe7-112">displayName</span></span>|<span data-ttu-id="a8fe7-113">String</span><span class="sxs-lookup"><span data-stu-id="a8fe7-113">String</span></span>|<span data-ttu-id="a8fe7-114">O nome do editor verificado da conta do Microsoft Partner Network (MPN) do editor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="a8fe7-114">The verified publisher name from the app publisher's Microsoft Partner Network (MPN) account.</span></span>|
|<span data-ttu-id="a8fe7-115">verifiedPublisherId</span><span class="sxs-lookup"><span data-stu-id="a8fe7-115">verifiedPublisherId</span></span>|<span data-ttu-id="a8fe7-116">String</span><span class="sxs-lookup"><span data-stu-id="a8fe7-116">String</span></span>| <span data-ttu-id="a8fe7-117">A ID do editor verificado da conta do Partner Center do editor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="a8fe7-117">The ID of the verified publisher from the app publisher's Partner Center account.</span></span> |
|<span data-ttu-id="a8fe7-118">addedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8fe7-118">addedDateTime</span></span>|<span data-ttu-id="a8fe7-119">DateTimeOffSet</span><span class="sxs-lookup"><span data-stu-id="a8fe7-119">DateTimeOffSet</span></span>| <span data-ttu-id="a8fe7-120">O timestamp quando o editor verificado foi adicionado pela primeira vez ou atualizado mais recentemente.</span><span class="sxs-lookup"><span data-stu-id="a8fe7-120">The timestamp when the verified publisher was first added or most recently updated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a8fe7-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8fe7-121">JSON representation</span></span>
<span data-ttu-id="a8fe7-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8fe7-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedPublisher"
}-->

```json
{
  "displayName": "String",
  "verifiedPublisherId": "String",
  "addedDateTime": "DateTimeOffSet"
}

```


<!-- uuid: e9aa37e1-f0b7-4201-a6b2-d26ce091dff6
2020-09-09 20:42:32 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedPublisher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
