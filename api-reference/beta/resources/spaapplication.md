---
title: Tipo de recurso spaApplication
description: Especifica configurações para um aplicativo de página única.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: hamiltonha
ms.openlocfilehash: a05d2eb997212b3baf88b84e21468475a45a691c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128824"
---
# <a name="spaapplication-resource-type"></a><span data-ttu-id="05c8a-103">Tipo de recurso spaApplication</span><span class="sxs-lookup"><span data-stu-id="05c8a-103">spaApplication resource type</span></span>

<span data-ttu-id="05c8a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05c8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05c8a-105">Especifica configurações para um aplicativo de página única.</span><span class="sxs-lookup"><span data-stu-id="05c8a-105">Specifies settings for a single-page application.</span></span>

## <a name="properties"></a><span data-ttu-id="05c8a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05c8a-106">Properties</span></span>

| <span data-ttu-id="05c8a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05c8a-107">Property</span></span> | <span data-ttu-id="05c8a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="05c8a-108">Type</span></span> | <span data-ttu-id="05c8a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="05c8a-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="05c8a-110">redirectUris</span><span class="sxs-lookup"><span data-stu-id="05c8a-110">redirectUris</span></span> | <span data-ttu-id="05c8a-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="05c8a-111">String collection</span></span> | <span data-ttu-id="05c8a-112">Especifica as URLs para onde os tokens de usuário são enviados para entrada ou os URIs de redirecionamento para os quais os códigos de autorização e tokens de acesso do OAuth 2.0 são enviados.</span><span class="sxs-lookup"><span data-stu-id="05c8a-112">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="05c8a-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05c8a-113">JSON representation</span></span>
<span data-ttu-id="05c8a-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="05c8a-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.spaApplication"
}-->

```json
{
  "redirectUris": ["String"]
}
```
