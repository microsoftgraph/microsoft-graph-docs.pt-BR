---
title: tipo de recurso de informationalUrl
description: Informações básicas de perfil do aplicativo.
ms.openlocfilehash: c8a13f4f686fe3b6ffd460ab05342b7da9b4a808
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038196"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="cd3c6-103">tipo de recurso de informationalUrl</span><span class="sxs-lookup"><span data-stu-id="cd3c6-103">informationalUrl resource type</span></span>

> <span data-ttu-id="cd3c6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cd3c6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd3c6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cd3c6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd3c6-106">Informações básicas de perfil do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cd3c6-106">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="cd3c6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd3c6-107">Properties</span></span>

| <span data-ttu-id="cd3c6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd3c6-108">Property</span></span> | <span data-ttu-id="cd3c6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd3c6-109">Type</span></span> | <span data-ttu-id="cd3c6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd3c6-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cd3c6-111">marketing</span><span class="sxs-lookup"><span data-stu-id="cd3c6-111">marketing</span></span>|<span data-ttu-id="cd3c6-112">String</span><span class="sxs-lookup"><span data-stu-id="cd3c6-112">String</span></span>| <span data-ttu-id="cd3c6-113">Link para a página de marketing do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cd3c6-113">Link to the application's marketing page.</span></span> <span data-ttu-id="cd3c6-114">Por exemplo, https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="cd3c6-114">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="cd3c6-115">privacidade</span><span class="sxs-lookup"><span data-stu-id="cd3c6-115">privacy</span></span>|<span data-ttu-id="cd3c6-116">String</span><span class="sxs-lookup"><span data-stu-id="cd3c6-116">String</span></span>| <span data-ttu-id="cd3c6-117">Link para a declaração de privacidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cd3c6-117">Link to the application's privacy statement.</span></span> <span data-ttu-id="cd3c6-118">Por exemplo, https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="cd3c6-118">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="cd3c6-119">suporte</span><span class="sxs-lookup"><span data-stu-id="cd3c6-119">support</span></span>|<span data-ttu-id="cd3c6-120">String</span><span class="sxs-lookup"><span data-stu-id="cd3c6-120">String</span></span>| <span data-ttu-id="cd3c6-121">Link para a página de suporte do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cd3c6-121">Link to the application's support page.</span></span> <span data-ttu-id="cd3c6-122">Por exemplo, https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="cd3c6-122">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="cd3c6-123">termsOfService</span><span class="sxs-lookup"><span data-stu-id="cd3c6-123">termsOfService</span></span>|<span data-ttu-id="cd3c6-124">String</span><span class="sxs-lookup"><span data-stu-id="cd3c6-124">String</span></span>| <span data-ttu-id="cd3c6-125">Link para os termos do aplicativo de instrução de serviço.</span><span class="sxs-lookup"><span data-stu-id="cd3c6-125">Link to the application's terms of service statement.</span></span> <span data-ttu-id="cd3c6-126">Por exemplo, https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="cd3c6-126">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cd3c6-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd3c6-127">JSON representation</span></span>
<span data-ttu-id="cd3c6-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd3c6-128">Here is a JSON representation of the resource.</span></span>

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