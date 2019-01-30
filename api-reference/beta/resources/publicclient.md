---
title: tipo de recurso de publicClient
description: Especifica as configurações para não Web App ou o Api da Web. (por exemplo, celular ou outro cliente público, como um aplicativo instalado em execução em um dispositivo de área de trabalho)
localization_priority: Normal
ms.openlocfilehash: ff1d77709293a7167868451671e1660196c9a4db
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644053"
---
# <a name="publicclient-resource-type"></a><span data-ttu-id="ee5e0-104">tipo de recurso de publicClient</span><span class="sxs-lookup"><span data-stu-id="ee5e0-104">publicClient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee5e0-105">Especifica as configurações para não Web App ou o Api da Web.</span><span class="sxs-lookup"><span data-stu-id="ee5e0-105">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="ee5e0-106">(por exemplo, celular ou outro cliente público, como um aplicativo instalado em execução em um dispositivo de área de trabalho)</span><span class="sxs-lookup"><span data-stu-id="ee5e0-106">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="ee5e0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee5e0-107">Properties</span></span>

| <span data-ttu-id="ee5e0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee5e0-108">Property</span></span> | <span data-ttu-id="ee5e0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee5e0-109">Type</span></span> | <span data-ttu-id="ee5e0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee5e0-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ee5e0-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="ee5e0-111">redirectUris</span></span>|<span data-ttu-id="ee5e0-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee5e0-112">String collection</span></span>| <span data-ttu-id="ee5e0-113">Especifica o redirecionamento de códigos de autorização de URIs que OAuth 2.0 e tokens de acesso são enviados para ou as URLs que os tokens do usuário são enviados para entrar.</span><span class="sxs-lookup"><span data-stu-id="ee5e0-113">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ee5e0-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee5e0-114">JSON representation</span></span>
<span data-ttu-id="ee5e0-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee5e0-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.installedClient"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/publicclient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
