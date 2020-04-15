---
title: tipo optionalClaims
description: Declara as declarações opcionais solicitadas por um aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 271fc7a054fce7649ff5b637a0a55d47a566332e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43354102"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="9e6a4-103">tipo de recurso optionalClaims</span><span class="sxs-lookup"><span data-stu-id="9e6a4-103">optionalClaims resource type</span></span>

<span data-ttu-id="9e6a4-104">Namespace: Microsoft. Graph declara as declarações opcionais solicitadas por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e6a4-104">Namespace: microsoft.graph Declares the optional claims requested by an application.</span></span> <span data-ttu-id="9e6a4-105">Um aplicativo pode configurar declarações opcionais a serem retornadas em cada um dos três tipos de tokens (token de ID, token de acesso, token SAML 2) que pode receber do serviço de token de segurança.</span><span class="sxs-lookup"><span data-stu-id="9e6a4-105">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="9e6a4-106">Um aplicativo pode configurar um conjunto diferente de declarações opcionais a serem retornadas em cada tipo de token.</span><span class="sxs-lookup"><span data-stu-id="9e6a4-106">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="9e6a4-107">A propriedade optionalClaims do [aplicativo](application.md) é um objeto **optionalClaims** .</span><span class="sxs-lookup"><span data-stu-id="9e6a4-107">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="9e6a4-108">Desenvolvedores de aplicativos podem configurar declarações opcionais em aplicativos do Azure AD para especificar quais declarações desejam em tokens enviados ao aplicativo pelo serviço de token de segurança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9e6a4-108">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="9e6a4-109">Confira [fornecer declarações opcionais ao aplicativo Azure AD](/azure/active-directory/develop/active-directory-optional-claims) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="9e6a4-109">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="9e6a4-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e6a4-110">Properties</span></span>
| <span data-ttu-id="9e6a4-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e6a4-111">Property</span></span>     | <span data-ttu-id="9e6a4-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e6a4-112">Type</span></span>        | <span data-ttu-id="9e6a4-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e6a4-113">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9e6a4-114">idToken</span><span class="sxs-lookup"><span data-stu-id="9e6a4-114">idToken</span></span>|<span data-ttu-id="9e6a4-115">coleção [optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="9e6a4-115">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="9e6a4-116">As declarações opcionais retornadas no token de ID de JWT.</span><span class="sxs-lookup"><span data-stu-id="9e6a4-116">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="9e6a4-117">accessToken</span><span class="sxs-lookup"><span data-stu-id="9e6a4-117">accessToken</span></span>|<span data-ttu-id="9e6a4-118">coleção [optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="9e6a4-118">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="9e6a4-119">As declarações opcionais retornadas no token de acesso JWT.</span><span class="sxs-lookup"><span data-stu-id="9e6a4-119">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="9e6a4-120">saml2Token</span><span class="sxs-lookup"><span data-stu-id="9e6a4-120">saml2Token</span></span>|<span data-ttu-id="9e6a4-121">coleção [optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="9e6a4-121">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="9e6a4-122">As declarações opcionais retornadas no token SAML.</span><span class="sxs-lookup"><span data-stu-id="9e6a4-122">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e6a4-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e6a4-123">JSON Representation</span></span>
<span data-ttu-id="9e6a4-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e6a4-124">Here is a JSON representation of the resource.</span></span>
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