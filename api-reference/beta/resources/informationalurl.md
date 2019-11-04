---
title: tipo de recurso informationalUrl
description: Informações de perfil básicas do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: c8cf7bcc40480042b4cd43230ca0245bd690fd7b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938839"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="69c17-103">tipo de recurso informationalUrl</span><span class="sxs-lookup"><span data-stu-id="69c17-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69c17-104">Informações de perfil básicas do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69c17-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="69c17-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69c17-105">Properties</span></span>

| <span data-ttu-id="69c17-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69c17-106">Property</span></span> | <span data-ttu-id="69c17-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="69c17-107">Type</span></span> | <span data-ttu-id="69c17-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="69c17-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="69c17-109">logoUrl</span><span class="sxs-lookup"><span data-stu-id="69c17-109">logoUrl</span></span>|<span data-ttu-id="69c17-110">String</span><span class="sxs-lookup"><span data-stu-id="69c17-110">String</span></span>|<span data-ttu-id="69c17-111">A URL da CDN para o logotipo do aplicativo, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69c17-111">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="69c17-112">marketingUrl</span><span class="sxs-lookup"><span data-stu-id="69c17-112">marketingUrl</span></span>|<span data-ttu-id="69c17-113">String</span><span class="sxs-lookup"><span data-stu-id="69c17-113">String</span></span>| <span data-ttu-id="69c17-114">Link para a página de marketing do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69c17-114">Link to the application's marketing page.</span></span> <span data-ttu-id="69c17-115">Por exemplo, https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="69c17-115">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="69c17-116">privacyStatementUrl</span><span class="sxs-lookup"><span data-stu-id="69c17-116">privacyStatementUrl</span></span>|<span data-ttu-id="69c17-117">String</span><span class="sxs-lookup"><span data-stu-id="69c17-117">String</span></span>| <span data-ttu-id="69c17-118">Link para a política de privacidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69c17-118">Link to the application's privacy statement.</span></span> <span data-ttu-id="69c17-119">Por exemplo, https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="69c17-119">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="69c17-120">supportUrl</span><span class="sxs-lookup"><span data-stu-id="69c17-120">supportUrl</span></span>|<span data-ttu-id="69c17-121">String</span><span class="sxs-lookup"><span data-stu-id="69c17-121">String</span></span>| <span data-ttu-id="69c17-122">Link para a página de suporte do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69c17-122">Link to the application's support page.</span></span> <span data-ttu-id="69c17-123">Por exemplo, https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="69c17-123">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="69c17-124">termsOfServiceUrl</span><span class="sxs-lookup"><span data-stu-id="69c17-124">termsOfServiceUrl</span></span>|<span data-ttu-id="69c17-125">String</span><span class="sxs-lookup"><span data-stu-id="69c17-125">String</span></span>| <span data-ttu-id="69c17-126">Link para a instrução de termos de serviço do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69c17-126">Link to the application's terms of service statement.</span></span> <span data-ttu-id="69c17-127">Por exemplo, https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="69c17-127">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="69c17-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69c17-128">JSON representation</span></span>
<span data-ttu-id="69c17-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69c17-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "logoUrl": "String",
  "marketingUrl": "String",
  "privacyStatementUrl": "String",
  "supportUrl": "String",
  "termsOfServiceUrl": "String"
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
