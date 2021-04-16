---
title: Tipo de recurso spaApplication
description: Especifica configurações para um aplicativo de página única.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 82848c5ea8427111b2d8b02c1886f3990faba79e
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836939"
---
# <a name="spaapplication-resource-type"></a><span data-ttu-id="9d274-103">Tipo de recurso spaApplication</span><span class="sxs-lookup"><span data-stu-id="9d274-103">spaApplication resource type</span></span>

<span data-ttu-id="9d274-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d274-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d274-105">Especifica configurações para um aplicativo de página única.</span><span class="sxs-lookup"><span data-stu-id="9d274-105">Specifies settings for a single-page application.</span></span>

## <a name="properties"></a><span data-ttu-id="9d274-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d274-106">Properties</span></span>

| <span data-ttu-id="9d274-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d274-107">Property</span></span> | <span data-ttu-id="9d274-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d274-108">Type</span></span> | <span data-ttu-id="9d274-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d274-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="9d274-110">redirectUris</span><span class="sxs-lookup"><span data-stu-id="9d274-110">redirectUris</span></span> | <span data-ttu-id="9d274-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d274-111">String collection</span></span> | <span data-ttu-id="9d274-112">Especifica as URLs para as quais os tokens de usuário são enviados para entrar ou as URIs de redirecionamento para as quais os códigos de autorização do OAuth 2.0 e tokens de acesso são enviados.</span><span class="sxs-lookup"><span data-stu-id="9d274-112">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9d274-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d274-113">JSON representation</span></span>
<span data-ttu-id="9d274-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d274-114">The following is a JSON representation of the resource.</span></span>

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
