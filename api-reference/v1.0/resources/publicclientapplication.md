---
title: Tipo de recurso publicClientApplication
description: Especifica configurações para não Web App ou Api da Web. (por exemplo, celular ou outro cliente público, como um aplicativo instalado em execução em um dispositivo de desktop)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: a15f0ea159ab12403186465783200a9e374562bc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137512"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="b6b3e-104">Tipo de recurso publicClientApplication</span><span class="sxs-lookup"><span data-stu-id="b6b3e-104">publicClientApplication resource type</span></span>

<span data-ttu-id="b6b3e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6b3e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6b3e-106">Especifica configurações para aplicativo não Web ou API não Web (por exemplo, dispositivos móveis ou outros clientes públicos, como um aplicativo instalado em execução em um dispositivo de desktop).</span><span class="sxs-lookup"><span data-stu-id="b6b3e-106">Specifies settings for non-web app or non-web API (for example, mobile or other public clients such as an installed application running on a desktop device).</span></span>

## <a name="properties"></a><span data-ttu-id="b6b3e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6b3e-107">Properties</span></span>

| <span data-ttu-id="b6b3e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6b3e-108">Property</span></span> | <span data-ttu-id="b6b3e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6b3e-109">Type</span></span> | <span data-ttu-id="b6b3e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6b3e-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b6b3e-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="b6b3e-111">redirectUris</span></span>|<span data-ttu-id="b6b3e-112">String collection</span><span class="sxs-lookup"><span data-stu-id="b6b3e-112">String collection</span></span>| <span data-ttu-id="b6b3e-113">Especifica as URLs para onde os tokens de usuário são enviados para entrada ou os URIs de redirecionamento para os quais os códigos de autorização e tokens de acesso do OAuth 2.0 são enviados.</span><span class="sxs-lookup"><span data-stu-id="b6b3e-113">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b6b3e-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6b3e-114">JSON representation</span></span>
<span data-ttu-id="b6b3e-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6b3e-115">Here is a JSON representation of the resource.</span></span>

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

