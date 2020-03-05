---
title: tipo de recurso informationalUrl
description: Informações de perfil básicas do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 88b3ae7af8604b6092ad87f2751791f48d273a68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496093"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="37370-103">tipo de recurso informationalUrl</span><span class="sxs-lookup"><span data-stu-id="37370-103">informationalUrl resource type</span></span>

<span data-ttu-id="37370-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="37370-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37370-105">Informações de perfil básicas do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="37370-105">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="37370-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37370-106">Properties</span></span>

| <span data-ttu-id="37370-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37370-107">Property</span></span> | <span data-ttu-id="37370-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="37370-108">Type</span></span> | <span data-ttu-id="37370-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="37370-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="37370-110">logoUrl</span><span class="sxs-lookup"><span data-stu-id="37370-110">logoUrl</span></span>|<span data-ttu-id="37370-111">String</span><span class="sxs-lookup"><span data-stu-id="37370-111">String</span></span>|<span data-ttu-id="37370-112">A URL da CDN para o logotipo do aplicativo, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37370-112">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="37370-113">marketingUrl</span><span class="sxs-lookup"><span data-stu-id="37370-113">marketingUrl</span></span>|<span data-ttu-id="37370-114">String</span><span class="sxs-lookup"><span data-stu-id="37370-114">String</span></span>| <span data-ttu-id="37370-115">Link para a página de marketing do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="37370-115">Link to the application's marketing page.</span></span> <span data-ttu-id="37370-116">Por exemplo, https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="37370-116">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="37370-117">privacyStatementUrl</span><span class="sxs-lookup"><span data-stu-id="37370-117">privacyStatementUrl</span></span>|<span data-ttu-id="37370-118">String</span><span class="sxs-lookup"><span data-stu-id="37370-118">String</span></span>| <span data-ttu-id="37370-119">Link para a política de privacidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="37370-119">Link to the application's privacy statement.</span></span> <span data-ttu-id="37370-120">Por exemplo, https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="37370-120">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="37370-121">supportUrl</span><span class="sxs-lookup"><span data-stu-id="37370-121">supportUrl</span></span>|<span data-ttu-id="37370-122">String</span><span class="sxs-lookup"><span data-stu-id="37370-122">String</span></span>| <span data-ttu-id="37370-123">Link para a página de suporte do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="37370-123">Link to the application's support page.</span></span> <span data-ttu-id="37370-124">Por exemplo, https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="37370-124">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="37370-125">termsOfServiceUrl</span><span class="sxs-lookup"><span data-stu-id="37370-125">termsOfServiceUrl</span></span>|<span data-ttu-id="37370-126">String</span><span class="sxs-lookup"><span data-stu-id="37370-126">String</span></span>| <span data-ttu-id="37370-127">Link para a instrução de termos de serviço do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="37370-127">Link to the application's terms of service statement.</span></span> <span data-ttu-id="37370-128">Por exemplo, https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="37370-128">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="37370-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37370-129">JSON representation</span></span>
<span data-ttu-id="37370-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37370-130">Here is a JSON representation of the resource.</span></span>

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
