---
title: Tipo de recurso spaApplication
description: Especifica configurações para um aplicativo de página única.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 25f907aa8c7e5b47960bb3a482b9745c488d16a9
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836980"
---
# <a name="spaapplication-resource-type"></a><span data-ttu-id="14bc5-103">Tipo de recurso spaApplication</span><span class="sxs-lookup"><span data-stu-id="14bc5-103">spaApplication resource type</span></span>

<span data-ttu-id="14bc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14bc5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14bc5-105">Especifica configurações para um aplicativo de página única.</span><span class="sxs-lookup"><span data-stu-id="14bc5-105">Specifies settings for a single-page application.</span></span>

## <a name="properties"></a><span data-ttu-id="14bc5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14bc5-106">Properties</span></span>

| <span data-ttu-id="14bc5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14bc5-107">Property</span></span> | <span data-ttu-id="14bc5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="14bc5-108">Type</span></span> | <span data-ttu-id="14bc5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="14bc5-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="14bc5-110">redirectUris</span><span class="sxs-lookup"><span data-stu-id="14bc5-110">redirectUris</span></span> | <span data-ttu-id="14bc5-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="14bc5-111">String collection</span></span> | <span data-ttu-id="14bc5-112">Especifica as URLs para as quais os tokens de usuário são enviados para entrar ou as URIs de redirecionamento para as quais os códigos de autorização do OAuth 2.0 e tokens de acesso são enviados.</span><span class="sxs-lookup"><span data-stu-id="14bc5-112">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="14bc5-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14bc5-113">JSON representation</span></span>
<span data-ttu-id="14bc5-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14bc5-114">The following is a JSON representation of the resource.</span></span>

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
