---
title: tipo de recurso informationalUrl
description: Informações de perfil básicas do aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: e81d8cc4a1ef25364727049269b420cf426eb0c8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939478"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="006ef-103">tipo de recurso informationalUrl</span><span class="sxs-lookup"><span data-stu-id="006ef-103">informationalUrl resource type</span></span>

<span data-ttu-id="006ef-104">Informações de perfil básicas do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="006ef-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="006ef-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="006ef-105">Properties</span></span>

| <span data-ttu-id="006ef-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="006ef-106">Property</span></span> | <span data-ttu-id="006ef-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="006ef-107">Type</span></span> | <span data-ttu-id="006ef-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="006ef-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="006ef-109">logoUrl</span><span class="sxs-lookup"><span data-stu-id="006ef-109">logoUrl</span></span>|<span data-ttu-id="006ef-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="006ef-110">String</span></span>|<span data-ttu-id="006ef-111">A URL da CDN para o logotipo do aplicativo, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="006ef-111">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="006ef-112">marketingUrl</span><span class="sxs-lookup"><span data-stu-id="006ef-112">marketingUrl</span></span>|<span data-ttu-id="006ef-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="006ef-113">String</span></span>| <span data-ttu-id="006ef-114">Link para a página de marketing do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="006ef-114">Link to the application's marketing page.</span></span> <span data-ttu-id="006ef-115">Por exemplo, https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="006ef-115">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="006ef-116">privacyStatementUrl</span><span class="sxs-lookup"><span data-stu-id="006ef-116">privacyStatementUrl</span></span>|<span data-ttu-id="006ef-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="006ef-117">String</span></span>| <span data-ttu-id="006ef-118">Link para a política de privacidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="006ef-118">Link to the application's privacy statement.</span></span> <span data-ttu-id="006ef-119">Por exemplo, https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="006ef-119">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="006ef-120">supportUrl</span><span class="sxs-lookup"><span data-stu-id="006ef-120">supportUrl</span></span>|<span data-ttu-id="006ef-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="006ef-121">String</span></span>| <span data-ttu-id="006ef-122">Link para a página de suporte do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="006ef-122">Link to the application's support page.</span></span> <span data-ttu-id="006ef-123">Por exemplo, https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="006ef-123">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="006ef-124">termsOfServiceUrl</span><span class="sxs-lookup"><span data-stu-id="006ef-124">termsOfServiceUrl</span></span>|<span data-ttu-id="006ef-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="006ef-125">String</span></span>| <span data-ttu-id="006ef-126">Link para a instrução de termos de serviço do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="006ef-126">Link to the application's terms of service statement.</span></span> <span data-ttu-id="006ef-127">Por exemplo, https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="006ef-127">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="006ef-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="006ef-128">JSON representation</span></span>
<span data-ttu-id="006ef-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="006ef-129">Here is a JSON representation of the resource.</span></span>

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
