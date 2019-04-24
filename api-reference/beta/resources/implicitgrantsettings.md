---
title: tipo de recurso implicitGrantSettings
description: Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0. Propriedades separadas estão disponíveis para solicitar tokens de ID e acesso como parte do fluxo implícito. Para habilitar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506219"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="cbfe0-105">tipo de recurso implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="cbfe0-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbfe0-106">Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="cbfe0-107">Propriedades separadas estão disponíveis para solicitar tokens de ID e acesso como parte do fluxo implícito.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="cbfe0-108">Para habilitar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="cbfe0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cbfe0-109">Properties</span></span>

| <span data-ttu-id="cbfe0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbfe0-110">Property</span></span> | <span data-ttu-id="cbfe0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbfe0-111">Type</span></span> | <span data-ttu-id="cbfe0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbfe0-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="cbfe0-113">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="cbfe0-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="cbfe0-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="cbfe0-114">Boolean</span></span> | <span data-ttu-id="cbfe0-115">Especifica se este aplicativo Web pode solicitar um token de ID usando o fluxo implícito do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="cbfe0-116">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="cbfe0-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="cbfe0-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="cbfe0-117">Boolean</span></span> | <span data-ttu-id="cbfe0-118">Especifica se este aplicativo Web pode solicitar um token de acesso usando o fluxo implícito do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cbfe0-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cbfe0-119">JSON representation</span></span>
<span data-ttu-id="cbfe0-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-120">Here is a JSON representation of the resource.</span></span>

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
