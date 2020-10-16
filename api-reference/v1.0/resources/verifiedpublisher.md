---
title: tipo de recurso verifiedPublisher
description: Representa o fornecedor verificado do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jesakowi
ms.openlocfilehash: 0285eb767a2fc4606dceaf74693a570f14dd6612
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471501"
---
# <a name="verifiedpublisher-resource-type"></a><span data-ttu-id="74cc5-103">tipo de recurso verifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="74cc5-103">verifiedPublisher resource type</span></span>

<span data-ttu-id="74cc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74cc5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74cc5-105">Representa o fornecedor verificado do [aplicativo](application.md).</span><span class="sxs-lookup"><span data-stu-id="74cc5-105">Represents the verified publisher of the [application](application.md).</span></span> <span data-ttu-id="74cc5-106">Para obter mais informações, consulte [Publisher Verification](https://docs.microsoft.com/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="74cc5-106">For more information, see [Publisher verification](https://docs.microsoft.com/azure/active-directory/develop/publisher-verification-overview).</span></span> <span data-ttu-id="74cc5-107">Os editores verificados são definidos usando o [setVerifiedPublisher](../api/application-setverifiedpublisher.md) e só podem ser removidos usando o [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).</span><span class="sxs-lookup"><span data-stu-id="74cc5-107">Verified publishers are set using [setVerifiedPublisher](../api/application-setverifiedpublisher.md) and can only be removed using [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).</span></span>

## <a name="properties"></a><span data-ttu-id="74cc5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74cc5-108">Properties</span></span>

| <span data-ttu-id="74cc5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74cc5-109">Property</span></span> | <span data-ttu-id="74cc5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="74cc5-110">Type</span></span> | <span data-ttu-id="74cc5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="74cc5-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="74cc5-112">displayName</span><span class="sxs-lookup"><span data-stu-id="74cc5-112">displayName</span></span>|<span data-ttu-id="74cc5-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74cc5-113">String</span></span>|<span data-ttu-id="74cc5-114">O nome do editor verificado da conta do centro de parceria do fornecedor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="74cc5-114">The verified publisher name from the app publisher's Partner Center account.</span></span>|
|<span data-ttu-id="74cc5-115">verifiedPublisherId</span><span class="sxs-lookup"><span data-stu-id="74cc5-115">verifiedPublisherId</span></span>|<span data-ttu-id="74cc5-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74cc5-116">String</span></span>| <span data-ttu-id="74cc5-117">A ID do editor verificado da conta do centro de parceria do fornecedor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="74cc5-117">The ID of the verified publisher from the app publisher's Partner Center account.</span></span> |
|<span data-ttu-id="74cc5-118">addedDateTime</span><span class="sxs-lookup"><span data-stu-id="74cc5-118">addedDateTime</span></span>|<span data-ttu-id="74cc5-119">DateTimeOffSet</span><span class="sxs-lookup"><span data-stu-id="74cc5-119">DateTimeOffSet</span></span>| <span data-ttu-id="74cc5-120">O carimbo de data/hora da primeira adição ou atualização mais recente do editor verificado.</span><span class="sxs-lookup"><span data-stu-id="74cc5-120">The timestamp when the verified publisher was first added or most recently updated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="74cc5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74cc5-121">JSON representation</span></span>
<span data-ttu-id="74cc5-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74cc5-122">Here is a JSON representation of the resource.</span></span>

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


<!-- uuid: 7a355221-34dd-4579-9bdd-4c3e1909e1bb
2020-09-09 20:45:56 UTC -->
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
