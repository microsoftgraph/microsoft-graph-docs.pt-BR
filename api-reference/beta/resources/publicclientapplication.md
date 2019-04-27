---
title: tipo de recurso publicClientApplication
description: Especifica configurações para aplicativo não Web ou API Web. (por exemplo, móvel ou outro cliente público, como um aplicativo instalado em um dispositivo de área de trabalho)
localization_priority: Normal
ms.openlocfilehash: 8118d1e771cb55ce5b82c9ddac14aaa45260ab56
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348485"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="d87d6-104">tipo de recurso publicClientApplication</span><span class="sxs-lookup"><span data-stu-id="d87d6-104">publicClientApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d87d6-105">Especifica configurações para aplicativo não Web ou API Web.</span><span class="sxs-lookup"><span data-stu-id="d87d6-105">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="d87d6-106">(por exemplo, móvel ou outro cliente público, como um aplicativo instalado em um dispositivo de área de trabalho)</span><span class="sxs-lookup"><span data-stu-id="d87d6-106">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="d87d6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d87d6-107">Properties</span></span>

| <span data-ttu-id="d87d6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d87d6-108">Property</span></span> | <span data-ttu-id="d87d6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d87d6-109">Type</span></span> | <span data-ttu-id="d87d6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d87d6-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d87d6-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="d87d6-111">redirectUris</span></span>|<span data-ttu-id="d87d6-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d87d6-112">String collection</span></span>| <span data-ttu-id="d87d6-113">Especifica as URLs às quais os tokens de usuário são enviados para entrar ou os URIs de redirecionamento aos quais os códigos de autorização OAuth 2,0 e tokens de acesso são enviados.</span><span class="sxs-lookup"><span data-stu-id="d87d6-113">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d87d6-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d87d6-114">JSON representation</span></span>
<span data-ttu-id="d87d6-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d87d6-115">Here is a JSON representation of the resource.</span></span>

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
