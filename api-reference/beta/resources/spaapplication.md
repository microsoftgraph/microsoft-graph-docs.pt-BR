---
title: tipo de recurso spaApplication
description: Especifica as configurações para um aplicativo de página única.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: hamiltonha
ms.openlocfilehash: dd5e2c6419acd66cb482f2ccff2914b1bf0245dc
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031887"
---
# <a name="spaapplication-resource-type"></a><span data-ttu-id="4c824-103">tipo de recurso spaApplication</span><span class="sxs-lookup"><span data-stu-id="4c824-103">spaApplication resource type</span></span>

<span data-ttu-id="4c824-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c824-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c824-105">Especifica as configurações para um aplicativo de página única.</span><span class="sxs-lookup"><span data-stu-id="4c824-105">Specifies settings for a single-page application.</span></span>

## <a name="properties"></a><span data-ttu-id="4c824-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c824-106">Properties</span></span>

| <span data-ttu-id="4c824-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c824-107">Property</span></span> | <span data-ttu-id="4c824-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c824-108">Type</span></span> | <span data-ttu-id="4c824-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c824-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="4c824-110">redirectUris</span><span class="sxs-lookup"><span data-stu-id="4c824-110">redirectUris</span></span> | <span data-ttu-id="4c824-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c824-111">String collection</span></span> | <span data-ttu-id="4c824-112">Especifica as URLs nas quais os tokens de usuário são enviados para entrada ou os URIs de redirecionamento nos quais os códigos de autorização OAuth 2,0 e tokens de acesso são enviados.</span><span class="sxs-lookup"><span data-stu-id="4c824-112">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4c824-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c824-113">JSON representation</span></span>
<span data-ttu-id="4c824-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c824-114">The following is a JSON representation of the resource.</span></span>

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
