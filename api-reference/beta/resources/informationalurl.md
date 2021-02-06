---
title: Tipo de recurso informationalUrl
description: Informações de perfil básicas do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: d17ce96d1f714845d07bee3505a28d5a4e7e3978
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130238"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="1be94-103">Tipo de recurso informationalUrl</span><span class="sxs-lookup"><span data-stu-id="1be94-103">informationalUrl resource type</span></span>

<span data-ttu-id="1be94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1be94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1be94-105">Informações de perfil básicas do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1be94-105">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="1be94-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1be94-106">Properties</span></span>

| <span data-ttu-id="1be94-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1be94-107">Property</span></span> | <span data-ttu-id="1be94-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1be94-108">Type</span></span> | <span data-ttu-id="1be94-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1be94-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1be94-110">logoUrl</span><span class="sxs-lookup"><span data-stu-id="1be94-110">logoUrl</span></span>|<span data-ttu-id="1be94-111">String</span><span class="sxs-lookup"><span data-stu-id="1be94-111">String</span></span>|<span data-ttu-id="1be94-112">URL da CDN para o logotipo do aplicativo, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1be94-112">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="1be94-113">marketingUrl</span><span class="sxs-lookup"><span data-stu-id="1be94-113">marketingUrl</span></span>|<span data-ttu-id="1be94-114">String</span><span class="sxs-lookup"><span data-stu-id="1be94-114">String</span></span>| <span data-ttu-id="1be94-115">Link para a página de marketing do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1be94-115">Link to the application's marketing page.</span></span> <span data-ttu-id="1be94-116">Por exemplo, https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="1be94-116">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="1be94-117">privacyStatementUrl</span><span class="sxs-lookup"><span data-stu-id="1be94-117">privacyStatementUrl</span></span>|<span data-ttu-id="1be94-118">String</span><span class="sxs-lookup"><span data-stu-id="1be94-118">String</span></span>| <span data-ttu-id="1be94-119">Link para a política de privacidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1be94-119">Link to the application's privacy statement.</span></span> <span data-ttu-id="1be94-120">Por exemplo, https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="1be94-120">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="1be94-121">supportUrl</span><span class="sxs-lookup"><span data-stu-id="1be94-121">supportUrl</span></span>|<span data-ttu-id="1be94-122">String</span><span class="sxs-lookup"><span data-stu-id="1be94-122">String</span></span>| <span data-ttu-id="1be94-123">Link para a página de suporte do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1be94-123">Link to the application's support page.</span></span> <span data-ttu-id="1be94-124">Por exemplo, https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="1be94-124">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="1be94-125">termsOfServiceUrl</span><span class="sxs-lookup"><span data-stu-id="1be94-125">termsOfServiceUrl</span></span>|<span data-ttu-id="1be94-126">String</span><span class="sxs-lookup"><span data-stu-id="1be94-126">String</span></span>| <span data-ttu-id="1be94-127">Link para a instrução de termos de serviço do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1be94-127">Link to the application's terms of service statement.</span></span> <span data-ttu-id="1be94-128">Por exemplo, https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="1be94-128">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1be94-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1be94-129">JSON representation</span></span>
<span data-ttu-id="1be94-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1be94-130">Here is a JSON representation of the resource.</span></span>

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


