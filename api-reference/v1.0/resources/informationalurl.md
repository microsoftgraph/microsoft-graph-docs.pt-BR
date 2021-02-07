---
title: Tipo de recurso informationalUrl
description: Informações de perfil básicas do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: d249c150870a3a7149b92ad7aab55a84c23896dd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132101"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="51776-103">Tipo de recurso informationalUrl</span><span class="sxs-lookup"><span data-stu-id="51776-103">informationalUrl resource type</span></span>

<span data-ttu-id="51776-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51776-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51776-105">Informações de perfil básicas do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51776-105">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="51776-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51776-106">Properties</span></span>

| <span data-ttu-id="51776-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51776-107">Property</span></span> | <span data-ttu-id="51776-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="51776-108">Type</span></span> | <span data-ttu-id="51776-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="51776-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="51776-110">logoUrl</span><span class="sxs-lookup"><span data-stu-id="51776-110">logoUrl</span></span>|<span data-ttu-id="51776-111">String</span><span class="sxs-lookup"><span data-stu-id="51776-111">String</span></span>|<span data-ttu-id="51776-112">URL da CDN para o logotipo do aplicativo, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51776-112">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="51776-113">marketingUrl</span><span class="sxs-lookup"><span data-stu-id="51776-113">marketingUrl</span></span>|<span data-ttu-id="51776-114">String</span><span class="sxs-lookup"><span data-stu-id="51776-114">String</span></span>| <span data-ttu-id="51776-115">Link para a página de marketing do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51776-115">Link to the application's marketing page.</span></span> <span data-ttu-id="51776-116">Por exemplo, https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="51776-116">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="51776-117">privacyStatementUrl</span><span class="sxs-lookup"><span data-stu-id="51776-117">privacyStatementUrl</span></span>|<span data-ttu-id="51776-118">String</span><span class="sxs-lookup"><span data-stu-id="51776-118">String</span></span>| <span data-ttu-id="51776-119">Link para a política de privacidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51776-119">Link to the application's privacy statement.</span></span> <span data-ttu-id="51776-120">Por exemplo, https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="51776-120">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="51776-121">supportUrl</span><span class="sxs-lookup"><span data-stu-id="51776-121">supportUrl</span></span>|<span data-ttu-id="51776-122">String</span><span class="sxs-lookup"><span data-stu-id="51776-122">String</span></span>| <span data-ttu-id="51776-123">Link para a página de suporte do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51776-123">Link to the application's support page.</span></span> <span data-ttu-id="51776-124">Por exemplo, https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="51776-124">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="51776-125">termsOfServiceUrl</span><span class="sxs-lookup"><span data-stu-id="51776-125">termsOfServiceUrl</span></span>|<span data-ttu-id="51776-126">String</span><span class="sxs-lookup"><span data-stu-id="51776-126">String</span></span>| <span data-ttu-id="51776-127">Link para a instrução de termos de serviço do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51776-127">Link to the application's terms of service statement.</span></span> <span data-ttu-id="51776-128">Por exemplo, https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="51776-128">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="51776-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51776-129">JSON representation</span></span>
<span data-ttu-id="51776-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51776-130">Here is a JSON representation of the resource.</span></span>

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

