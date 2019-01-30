---
title: tipo de recurso de implicitGrantSettings
description: Especifica se esse aplicativo web pode solicitar tokens usando o fluxo de implícita OAuth 2.0. Propriedades separadas estão disponíveis para solicitar tokens de acesso e a ID como parte do fluxo de implícita. Para ativar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642762"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="3cd7d-105">tipo de recurso de implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="3cd7d-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cd7d-106">Especifica se esse aplicativo web pode solicitar tokens usando o fluxo de implícita OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="3cd7d-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="3cd7d-107">Propriedades separadas estão disponíveis para solicitar tokens de acesso e a ID como parte do fluxo de implícita.</span><span class="sxs-lookup"><span data-stu-id="3cd7d-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="3cd7d-108">Para ativar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.</span><span class="sxs-lookup"><span data-stu-id="3cd7d-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="3cd7d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3cd7d-109">Properties</span></span>

| <span data-ttu-id="3cd7d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cd7d-110">Property</span></span> | <span data-ttu-id="3cd7d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cd7d-111">Type</span></span> | <span data-ttu-id="3cd7d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cd7d-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="3cd7d-113">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="3cd7d-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="3cd7d-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="3cd7d-114">Boolean</span></span> | <span data-ttu-id="3cd7d-115">Especifica se esse aplicativo web pode solicitar um token de ID usando o fluxo de implícita OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="3cd7d-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="3cd7d-116">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="3cd7d-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="3cd7d-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="3cd7d-117">Boolean</span></span> | <span data-ttu-id="3cd7d-118">Especifica se esse aplicativo web pode solicitar um token de acesso usando o fluxo de implícita OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="3cd7d-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3cd7d-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3cd7d-119">JSON representation</span></span>
<span data-ttu-id="3cd7d-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3cd7d-120">Here is a JSON representation of the resource.</span></span>

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/implicitgrantsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
