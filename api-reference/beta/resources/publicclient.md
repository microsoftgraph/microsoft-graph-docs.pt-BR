---
title: tipo de recurso de publicClient
description: Especifica as configurações para não Web App ou o Api da Web. (por exemplo, celular ou outro cliente público, como um aplicativo instalado em execução em um dispositivo de área de trabalho)
ms.openlocfilehash: ba921fecb554a8749a9020508c538c68a7ff342e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033780"
---
# <a name="publicclient-resource-type"></a><span data-ttu-id="21c5f-104">tipo de recurso de publicClient</span><span class="sxs-lookup"><span data-stu-id="21c5f-104">publicClient resource type</span></span>

> <span data-ttu-id="21c5f-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="21c5f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21c5f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="21c5f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="21c5f-107">Especifica as configurações para não Web App ou o Api da Web.</span><span class="sxs-lookup"><span data-stu-id="21c5f-107">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="21c5f-108">(por exemplo, celular ou outro cliente público, como um aplicativo instalado em execução em um dispositivo de área de trabalho)</span><span class="sxs-lookup"><span data-stu-id="21c5f-108">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="21c5f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21c5f-109">Properties</span></span>

| <span data-ttu-id="21c5f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21c5f-110">Property</span></span> | <span data-ttu-id="21c5f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="21c5f-111">Type</span></span> | <span data-ttu-id="21c5f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="21c5f-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="21c5f-113">redirectUris</span><span class="sxs-lookup"><span data-stu-id="21c5f-113">redirectUris</span></span>|<span data-ttu-id="21c5f-114">String collection</span><span class="sxs-lookup"><span data-stu-id="21c5f-114">String collection</span></span>| <span data-ttu-id="21c5f-115">Especifica o redirecionamento de códigos de autorização de URIs que OAuth 2.0 e tokens de acesso são enviados para ou as URLs que os tokens do usuário são enviados para entrar.</span><span class="sxs-lookup"><span data-stu-id="21c5f-115">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="21c5f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21c5f-116">JSON representation</span></span>
<span data-ttu-id="21c5f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21c5f-117">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->