---
title: tipo optionalClaims
description: Declara as declarações opcionais solicitadas por um aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 19f5233ddb4db55f625460a063a175fc4a3e5efc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447273"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="ffe30-103">tipo de recurso optionalClaims</span><span class="sxs-lookup"><span data-stu-id="ffe30-103">optionalClaims resource type</span></span>

<span data-ttu-id="ffe30-104">Namespace: Microsoft. Graph declara as declarações opcionais solicitadas por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ffe30-104">Namespace: microsoft.graph Declares the optional claims requested by an application.</span></span> <span data-ttu-id="ffe30-105">Um aplicativo pode configurar declarações opcionais a serem retornadas em cada um dos três tipos de tokens (token de ID, token de acesso, token SAML 2) que pode receber do serviço de token de segurança.</span><span class="sxs-lookup"><span data-stu-id="ffe30-105">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="ffe30-106">Um aplicativo pode configurar um conjunto diferente de declarações opcionais a serem retornadas em cada tipo de token.</span><span class="sxs-lookup"><span data-stu-id="ffe30-106">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="ffe30-107">A propriedade optionalClaims do [aplicativo](application.md) é um objeto **optionalClaims** .</span><span class="sxs-lookup"><span data-stu-id="ffe30-107">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="ffe30-108">Desenvolvedores de aplicativos podem configurar declarações opcionais em aplicativos do Azure AD para especificar quais declarações desejam em tokens enviados ao aplicativo pelo serviço de token de segurança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ffe30-108">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="ffe30-109">Confira [fornecer declarações opcionais ao aplicativo Azure AD](/azure/active-directory/develop/active-directory-optional-claims) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="ffe30-109">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="ffe30-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ffe30-110">Properties</span></span>
| <span data-ttu-id="ffe30-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ffe30-111">Property</span></span>     | <span data-ttu-id="ffe30-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffe30-112">Type</span></span>        | <span data-ttu-id="ffe30-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffe30-113">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ffe30-114">idToken</span><span class="sxs-lookup"><span data-stu-id="ffe30-114">idToken</span></span>|<span data-ttu-id="ffe30-115">coleção [optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="ffe30-115">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="ffe30-116">As declarações opcionais retornadas no token de ID de JWT.</span><span class="sxs-lookup"><span data-stu-id="ffe30-116">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="ffe30-117">accessToken</span><span class="sxs-lookup"><span data-stu-id="ffe30-117">accessToken</span></span>|<span data-ttu-id="ffe30-118">coleção [optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="ffe30-118">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="ffe30-119">As declarações opcionais retornadas no token de acesso JWT.</span><span class="sxs-lookup"><span data-stu-id="ffe30-119">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="ffe30-120">saml2Token</span><span class="sxs-lookup"><span data-stu-id="ffe30-120">saml2Token</span></span>|<span data-ttu-id="ffe30-121">coleção [optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="ffe30-121">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="ffe30-122">As declarações opcionais retornadas no token SAML.</span><span class="sxs-lookup"><span data-stu-id="ffe30-122">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffe30-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ffe30-123">JSON Representation</span></span>
<span data-ttu-id="ffe30-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ffe30-124">Here is a JSON representation of the resource.</span></span>
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