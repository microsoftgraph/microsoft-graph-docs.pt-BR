---
title: tipo optionalClaims
description: Declara as declarações opcionais solicitadas por um aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: d50b514fa29cf99f22bb42238ac9d6a66126ab53
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132653"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="b9d31-103">Tipo de recurso optionalClaims</span><span class="sxs-lookup"><span data-stu-id="b9d31-103">optionalClaims resource type</span></span>

<span data-ttu-id="b9d31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9d31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9d31-105">Declara as declarações opcionais solicitadas por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9d31-105">Declares the optional claims requested by an application.</span></span> <span data-ttu-id="b9d31-106">Um aplicativo pode configurar declarações opcionais a serem retornadas em cada um dos três tipos de tokens (token de ID, token de acesso, token SAML 2) que ele pode receber do serviço de token de segurança.</span><span class="sxs-lookup"><span data-stu-id="b9d31-106">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="b9d31-107">Um aplicativo pode configurar um conjunto diferente de declarações opcionais a serem retornadas em cada tipo de token.</span><span class="sxs-lookup"><span data-stu-id="b9d31-107">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="b9d31-108">A propriedade optionalClaims do [aplicativo é](application.md) um **objeto optionalClaims.**</span><span class="sxs-lookup"><span data-stu-id="b9d31-108">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="b9d31-109">Desenvolvedores de aplicativos podem configurar declarações opcionais em aplicativos do Azure AD para especificar quais declarações desejam em tokens enviados ao aplicativo pelo serviço de token de segurança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b9d31-109">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="b9d31-110">Confira [fornecer declarações opcionais ao aplicativo Azure AD](/azure/active-directory/develop/active-directory-optional-claims) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="b9d31-110">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="b9d31-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9d31-111">Properties</span></span>
| <span data-ttu-id="b9d31-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9d31-112">Property</span></span>     | <span data-ttu-id="b9d31-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9d31-113">Type</span></span>        | <span data-ttu-id="b9d31-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9d31-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b9d31-115">idToken</span><span class="sxs-lookup"><span data-stu-id="b9d31-115">idToken</span></span>|<span data-ttu-id="b9d31-116">[coleção optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="b9d31-116">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="b9d31-117">As declarações opcionais retornadas no token de ID JWT.</span><span class="sxs-lookup"><span data-stu-id="b9d31-117">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="b9d31-118">accessToken</span><span class="sxs-lookup"><span data-stu-id="b9d31-118">accessToken</span></span>|<span data-ttu-id="b9d31-119">[coleção optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="b9d31-119">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="b9d31-120">As declarações opcionais retornadas no token de acesso JWT.</span><span class="sxs-lookup"><span data-stu-id="b9d31-120">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="b9d31-121">saml2Token</span><span class="sxs-lookup"><span data-stu-id="b9d31-121">saml2Token</span></span>|<span data-ttu-id="b9d31-122">[coleção optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="b9d31-122">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="b9d31-123">As declarações opcionais retornadas no token SAML.</span><span class="sxs-lookup"><span data-stu-id="b9d31-123">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9d31-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9d31-124">JSON Representation</span></span>
<span data-ttu-id="b9d31-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9d31-125">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.optionalClaims"
}-->
``` json
{
  "idToken": [{"@odata.type": "microsoft.graph.optionalClaim"}],
  "accessToken": [{"@odata.type": "microsoft.graph.optionalClaim"}],
  "saml2Token": [{"@odata.type": "microsoft.graph.optionalClaim"}]
}
```
