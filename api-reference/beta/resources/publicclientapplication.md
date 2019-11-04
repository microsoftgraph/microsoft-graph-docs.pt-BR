---
title: tipo de recurso publicClientApplication
description: Especifica configurações para aplicativo não Web ou API Web. (por exemplo, móvel ou outro cliente público, como um aplicativo instalado em um dispositivo de área de trabalho)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a9d54ed7f15f6bbcabd85ee50e8137b131399b22
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939380"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="a0b93-104">tipo de recurso publicClientApplication</span><span class="sxs-lookup"><span data-stu-id="a0b93-104">publicClientApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0b93-105">Especifica configurações para aplicativo não Web ou API não Web (por exemplo, dispositivos móveis ou outros clientes públicos, como um aplicativo instalado em um dispositivo Desktop).</span><span class="sxs-lookup"><span data-stu-id="a0b93-105">Specifies settings for non-web app or non-web API (for example, mobile or other public clients such as an installed application running on a desktop device).</span></span>

## <a name="properties"></a><span data-ttu-id="a0b93-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0b93-106">Properties</span></span>

| <span data-ttu-id="a0b93-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0b93-107">Property</span></span> | <span data-ttu-id="a0b93-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0b93-108">Type</span></span> | <span data-ttu-id="a0b93-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0b93-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a0b93-110">redirectUris</span><span class="sxs-lookup"><span data-stu-id="a0b93-110">redirectUris</span></span>|<span data-ttu-id="a0b93-111">String collection</span><span class="sxs-lookup"><span data-stu-id="a0b93-111">String collection</span></span>| <span data-ttu-id="a0b93-112">Especifica as URLs nas quais os tokens de usuário são enviados para entrada ou os URIs de redirecionamento nos quais os códigos de autorização OAuth 2,0 e tokens de acesso são enviados.</span><span class="sxs-lookup"><span data-stu-id="a0b93-112">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a0b93-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0b93-113">JSON representation</span></span>
<span data-ttu-id="a0b93-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0b93-114">Here is a JSON representation of the resource.</span></span>

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
