---
title: tipo de recurso publicClientApplication
description: Especifica configurações para aplicativo não Web ou API Web. (por exemplo, móvel ou outro cliente público, como um aplicativo instalado em um dispositivo de área de trabalho)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 0fd7715380577097a93cd8d8cc8a62178f50ec24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026422"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="20d55-104">tipo de recurso publicClientApplication</span><span class="sxs-lookup"><span data-stu-id="20d55-104">publicClientApplication resource type</span></span>

<span data-ttu-id="20d55-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20d55-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20d55-106">Especifica configurações para aplicativo não Web ou API não Web (por exemplo, dispositivos móveis ou outros clientes públicos, como um aplicativo instalado em um dispositivo Desktop).</span><span class="sxs-lookup"><span data-stu-id="20d55-106">Specifies settings for non-web app or non-web API (for example, mobile or other public clients such as an installed application running on a desktop device).</span></span>

## <a name="properties"></a><span data-ttu-id="20d55-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20d55-107">Properties</span></span>

| <span data-ttu-id="20d55-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20d55-108">Property</span></span> | <span data-ttu-id="20d55-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="20d55-109">Type</span></span> | <span data-ttu-id="20d55-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="20d55-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="20d55-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="20d55-111">redirectUris</span></span>|<span data-ttu-id="20d55-112">Coleção String</span><span class="sxs-lookup"><span data-stu-id="20d55-112">String collection</span></span>| <span data-ttu-id="20d55-113">Especifica as URLs nas quais os tokens de usuário são enviados para entrada ou os URIs de redirecionamento nos quais os códigos de autorização OAuth 2,0 e tokens de acesso são enviados.</span><span class="sxs-lookup"><span data-stu-id="20d55-113">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="20d55-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20d55-114">JSON representation</span></span>
<span data-ttu-id="20d55-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20d55-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publicClientApplication"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


