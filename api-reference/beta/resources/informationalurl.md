---
title: tipo de recurso de informationalUrl
description: Informações básicas de perfil do aplicativo.
localization_priority: Normal
ms.openlocfilehash: 78fd03a2673b342d1a0c904f521fe5a0f8cba205
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816979"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="5b49e-103">tipo de recurso de informationalUrl</span><span class="sxs-lookup"><span data-stu-id="5b49e-103">informationalUrl resource type</span></span>

> <span data-ttu-id="5b49e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5b49e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b49e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5b49e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b49e-106">Informações básicas de perfil do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5b49e-106">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="5b49e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b49e-107">Properties</span></span>

| <span data-ttu-id="5b49e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b49e-108">Property</span></span> | <span data-ttu-id="5b49e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b49e-109">Type</span></span> | <span data-ttu-id="5b49e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b49e-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5b49e-111">marketing</span><span class="sxs-lookup"><span data-stu-id="5b49e-111">marketing</span></span>|<span data-ttu-id="5b49e-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b49e-112">String</span></span>| <span data-ttu-id="5b49e-113">Link para a página de marketing do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5b49e-113">Link to the application's marketing page.</span></span> <span data-ttu-id="5b49e-114">Por exemplo, https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="5b49e-114">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="5b49e-115">privacidade</span><span class="sxs-lookup"><span data-stu-id="5b49e-115">privacy</span></span>|<span data-ttu-id="5b49e-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b49e-116">String</span></span>| <span data-ttu-id="5b49e-117">Link para a declaração de privacidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5b49e-117">Link to the application's privacy statement.</span></span> <span data-ttu-id="5b49e-118">Por exemplo, https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="5b49e-118">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="5b49e-119">suporte</span><span class="sxs-lookup"><span data-stu-id="5b49e-119">support</span></span>|<span data-ttu-id="5b49e-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b49e-120">String</span></span>| <span data-ttu-id="5b49e-121">Link para a página de suporte do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5b49e-121">Link to the application's support page.</span></span> <span data-ttu-id="5b49e-122">Por exemplo, https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="5b49e-122">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="5b49e-123">termsOfService</span><span class="sxs-lookup"><span data-stu-id="5b49e-123">termsOfService</span></span>|<span data-ttu-id="5b49e-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b49e-124">String</span></span>| <span data-ttu-id="5b49e-125">Link para os termos do aplicativo de instrução de serviço.</span><span class="sxs-lookup"><span data-stu-id="5b49e-125">Link to the application's terms of service statement.</span></span> <span data-ttu-id="5b49e-126">Por exemplo, https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="5b49e-126">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5b49e-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b49e-127">JSON representation</span></span>
<span data-ttu-id="5b49e-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b49e-128">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
