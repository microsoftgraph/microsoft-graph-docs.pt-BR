---
title: Criar conditionalAccessPolicy
description: Crie um novo conditionalAccessPolicy.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 60ffa83de871400c49aff07f8508d562e786c73c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964020"
---
# <a name="create-conditionalaccesspolicy"></a><span data-ttu-id="23ea8-103">Criar conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="23ea8-103">Create conditionalAccessPolicy</span></span>

<span data-ttu-id="23ea8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23ea8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23ea8-105">Crie um novo [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="23ea8-105">Create a new [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="23ea8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="23ea8-106">Permissions</span></span>

<span data-ttu-id="23ea8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23ea8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23ea8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23ea8-109">Permission type</span></span>                        | <span data-ttu-id="23ea8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23ea8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="23ea8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23ea8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="23ea8-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess e Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="23ea8-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
| <span data-ttu-id="23ea8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23ea8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23ea8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23ea8-114">Not supported.</span></span> |
| <span data-ttu-id="23ea8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23ea8-115">Application</span></span>                            | <span data-ttu-id="23ea8-116">Policy.Read.All, Policy.ReadWrite.ConditionalAccess e Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="23ea8-116">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23ea8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23ea8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/policies
```

## <a name="request-headers"></a><span data-ttu-id="23ea8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23ea8-118">Request headers</span></span>

| <span data-ttu-id="23ea8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="23ea8-119">Name</span></span>          | <span data-ttu-id="23ea8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="23ea8-120">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="23ea8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="23ea8-121">Authorization</span></span> | <span data-ttu-id="23ea8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23ea8-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="23ea8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23ea8-124">Content-Type</span></span>  | <span data-ttu-id="23ea8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23ea8-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23ea8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23ea8-127">Request body</span></span>

<span data-ttu-id="23ea8-128">No corpo da solicitação, fornece uma representação JSON de [um objeto conditionalAccessPolicy.](../resources/conditionalaccesspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23ea8-128">In the request body, supply a JSON representation of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

<span data-ttu-id="23ea8-129">Uma política válida deve conter pelo menos uma das seguintes:</span><span class="sxs-lookup"><span data-stu-id="23ea8-129">A valid policy should contain at least one of the following:</span></span>

* <span data-ttu-id="23ea8-130">[regra do aplicativo.](../resources/conditionalaccessapplications.md)</span><span class="sxs-lookup"><span data-stu-id="23ea8-130">[application](../resources/conditionalaccessapplications.md) rule.</span></span> <span data-ttu-id="23ea8-131">Por exemplo, `'includeApplications': 'none'`.</span><span class="sxs-lookup"><span data-stu-id="23ea8-131">For example, `'includeApplications': 'none'`.</span></span>
* <span data-ttu-id="23ea8-132">[regra](../resources/conditionalaccessusers.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="23ea8-132">[user](../resources/conditionalaccessusers.md) rule.</span></span> <span data-ttu-id="23ea8-133">Por exemplo, `'includeUsers': 'none'`.</span><span class="sxs-lookup"><span data-stu-id="23ea8-133">For example, `'includeUsers': 'none'`.</span></span>
* <span data-ttu-id="23ea8-134">[grant](../resources/conditionalaccessgrantcontrols.md) / [controle de](../resources/conditionalaccesssessioncontrols.md) sessão.</span><span class="sxs-lookup"><span data-stu-id="23ea8-134">[grant](../resources/conditionalaccessgrantcontrols.md)/[session](../resources/conditionalaccesssessioncontrols.md) control.</span></span>

## <a name="response"></a><span data-ttu-id="23ea8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="23ea8-135">Response</span></span>

<span data-ttu-id="23ea8-136">Se tiver êxito, este método retornará um código de resposta e um novo `201 Created` [objeto conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23ea8-136">If successful, this method returns a `201 Created` response code and a new [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23ea8-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="23ea8-137">Examples</span></span>

### <a name="example-1-require-mfa-to-access-exchange-online-outside-of-trusted-locations"></a><span data-ttu-id="23ea8-138">Exemplo 1: Exigir que o MFA acesse o Exchange Online fora de locais confiáveis</span><span class="sxs-lookup"><span data-stu-id="23ea8-138">Example 1: Require MFA to access Exchange Online outside of trusted locations</span></span>

#### <a name="request"></a><span data-ttu-id="23ea8-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23ea8-139">Request</span></span>
<span data-ttu-id="23ea8-140">O exemplo a seguir mostra uma solicitação comum para exigir autenticação multifa factor para acesso ao Exchange Online de clientes de autenticação modernos fora de locais confiáveis para um determinado grupo.</span><span class="sxs-lookup"><span data-stu-id="23ea8-140">The following example shows a common request to require multi-factor authentication for access to Exchange Online from modern authentication clients outside of trusted locations for a particular group.</span></span>

><span data-ttu-id="23ea8-141">**Observação:** Você deve configurar seus locais confiáveis antes de usar essa operação.</span><span class="sxs-lookup"><span data-stu-id="23ea8-141">**Note:** You must set up your trusted locations before using this operation.</span></span>

# <a name="http"></a>[<span data-ttu-id="23ea8-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="23ea8-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Access to EXO requires MFA",
    "state": "enabled",
    "conditions": {
        "clientAppTypes": [
            "mobileAppsAndDesktopClients",
            "browser"
        ],
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ]
        },
        "users": {
            "includeGroups": ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"]
        },
        "locations": {
            "includeLocations": [
                "All"
            ],
            "excludeLocations": [
                "AllTrusted"
            ]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa"
        ]
    }
}
```
# <a name="c"></a>[<span data-ttu-id="23ea8-143">C#</span><span class="sxs-lookup"><span data-stu-id="23ea8-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conditionalaccesspolicy-from-conditionalaccessroot-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23ea8-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23ea8-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conditionalaccesspolicy-from-conditionalaccessroot-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23ea8-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23ea8-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conditionalaccesspolicy-from-conditionalaccessroot-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23ea8-146">Java</span><span class="sxs-lookup"><span data-stu-id="23ea8-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conditionalaccesspolicy-from-conditionalaccessroot-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="23ea8-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="23ea8-147">Response</span></span>

<span data-ttu-id="23ea8-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="23ea8-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/policies/$entity",
    "id": "7359d0e0-d8a9-4afa-8a93-e23e099d7be8",
    "displayName": "Access to EXO requires MFA",
    "createdDateTime": "2019-10-14T19:52:00.050958Z",
    "modifiedDateTime": null,
    "state": "enabled",
    "sessionControls": null,
    "conditions": {
        "signInRiskLevels": [],
        "clientAppTypes": [
            "mobileAppsAndDesktopClients",
            "browser"
        ],
        "platforms": null,
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ],
            "excludeApplications": [],
            "includeUserActions": []
        },
        "users": {
            "includeUsers": [],
            "excludeUsers": [],
            "includeGroups": [
                "ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"
            ],
            "excludeGroups": [],
            "includeRoles": [],
            "excludeRoles": []
        },
        "locations": {
            "includeLocations": [
                "All"
            ],
            "excludeLocations": [
                "AllTrusted"
            ]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa"
        ],
        "customAuthenticationFactors": [],
        "termsOfUse": []
    }
}
```

### <a name="example-2-block-access-to-exchange-online-from-non-trusted-regions"></a><span data-ttu-id="23ea8-149">Exemplo 2: Bloquear o acesso ao Exchange Online de regiões não confiáveis</span><span class="sxs-lookup"><span data-stu-id="23ea8-149">Example 2: Block access to Exchange Online from non-trusted regions</span></span>

#### <a name="request"></a><span data-ttu-id="23ea8-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23ea8-150">Request</span></span>
<span data-ttu-id="23ea8-151">O exemplo a seguir mostra uma solicitação para bloquear o acesso ao Exchange Online de regiões não confiáveis/desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="23ea8-151">The following example shows a request to block access to Exchange Online from non-trusted/unknown regions.</span></span>
<span data-ttu-id="23ea8-152">Este exemplo supõe que o local nomeado com id = 198ad66e-87b3-4157-85a3-8a7b51794ee9 corresponde a uma lista de regiões não confiáveis/desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="23ea8-152">This example assumes that the named location with id = 198ad66e-87b3-4157-85a3-8a7b51794ee9 corresponds to a list of non-trusted/unknown regions.</span></span>


# <a name="http"></a>[<span data-ttu-id="23ea8-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="23ea8-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot_2"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Block access to EXO non-trusted regions.",
    "state": "enabled",
    "conditions": {
        "clientAppTypes": [
            "all"
        ],
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ]
        },
        "users": {
            "includeGroups": ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"]
        },
        "locations": {
            "includeLocations": [
                "198ad66e-87b3-4157-85a3-8a7b51794ee9"
            ]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "block"
        ]
    }
}
```
# <a name="c"></a>[<span data-ttu-id="23ea8-154">C#</span><span class="sxs-lookup"><span data-stu-id="23ea8-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conditionalaccesspolicy-from-conditionalaccessroot-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23ea8-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23ea8-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conditionalaccesspolicy-from-conditionalaccessroot-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23ea8-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23ea8-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conditionalaccesspolicy-from-conditionalaccessroot-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23ea8-157">Java</span><span class="sxs-lookup"><span data-stu-id="23ea8-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conditionalaccesspolicy-from-conditionalaccessroot-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23ea8-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="23ea8-158">Response</span></span>

<span data-ttu-id="23ea8-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="23ea8-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/policies/$entity",
    "id": "c98e6c3d-f6ca-42ea-a927-773b6f12a0c2",
    "displayName": "Block access to EXO non-trusted regions.",
    "createdDateTime": "2019-10-14T19:53:11.3705634Z",
    "modifiedDateTime": null,
    "state": "enabled",
    "sessionControls": null,
    "conditions": {
        "signInRiskLevels": [],
        "clientAppTypes": [
            "all"
        ],
        "platforms": null,
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ],
            "excludeApplications": [],
            "includeUserActions": []
        },
        "users": {
            "includeUsers": [],
            "excludeUsers": [],
            "includeGroups": [
                "ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"
            ],
            "excludeGroups": [],
            "includeRoles": [],
            "excludeRoles": []
        },
        "locations": {
            "includeLocations": [
                "198ad66e-87b3-4157-85a3-8a7b51794ee9"
            ],
            "excludeLocations": []
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "block"
        ],
        "customAuthenticationFactors": [],
        "termsOfUse": []
    }
}
```

### <a name="example-3-use-all-conditions-and-controls"></a><span data-ttu-id="23ea8-160">Exemplo 3: Usar todas as condições e controles</span><span class="sxs-lookup"><span data-stu-id="23ea8-160">Example 3: Use all conditions and controls</span></span>

#### <a name="request"></a><span data-ttu-id="23ea8-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23ea8-161">Request</span></span>
<span data-ttu-id="23ea8-162">A seguir, um exemplo da solicitação para usar todas as condições e controles.</span><span class="sxs-lookup"><span data-stu-id="23ea8-162">The following is an example of the request to use all the conditions and controls.</span></span>

# <a name="http"></a>[<span data-ttu-id="23ea8-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="23ea8-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot_3"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Demo app for documentation",
    "state": "disabled",
    "conditions": {
        "signInRiskLevels": [
            "high",
            "medium"
        ],
        "clientAppTypes": [
            "mobileAppsAndDesktopClients",
            "exchangeActiveSync",
            "other"
        ],
        "applications": {
            "includeApplications": [
                "All"
            ],
            "excludeApplications": [
                "499b84ac-1321-427f-aa17-267ca6975798",
                "00000007-0000-0000-c000-000000000000",
                "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
                "00000012-0000-0000-c000-000000000000",
                "797f4846-ba00-4fd7-ba43-dac1f8f63013",
                "05a65629-4c1b-48c1-a78b-804c4abdd4af",
                "7df0a125-d3be-4c96-aa54-591f83ff541c"
            ],
            "includeUserActions": []
        },
        "users": {
            "includeUsers": [
                "a702a13d-a437-4a07-8a7e-8c052de62dfd"
            ],
            "excludeUsers": [
                "124c5b6a-ffa5-483a-9b88-04c3fce5574a",
                "GuestsOrExternalUsers"
            ],
            "includeGroups": [],
            "excludeGroups": [],
            "includeRoles": [
                "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
                "cf1c38e5-3621-4004-a7cb-879624dced7c",
                "c4e39bd9-1100-46d3-8c65-fb160da0071f"
            ],
            "excludeRoles": [
                "b0f54661-2d74-4c50-afa3-1ec803f12efe"
            ]
        },
        "platforms": {
            "includePlatforms": [
                "all"
            ],
            "excludePlatforms": [
                "iOS",
                "windowsPhone"
            ]
        },
        "locations": {
            "includeLocations": [
                "AllTrusted"
            ],
            "excludeLocations": [
                "00000000-0000-0000-0000-000000000000",
                "d2136c9c-b049-47ae-b9cf-316e04ef7198"
            ]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa",
            "compliantDevice",
            "domainJoinedDevice",
            "approvedApplication",
            "compliantApplication"
        ],
        "customAuthenticationFactors": [],
        "termsOfUse": [
            "ce580154-086a-40fd-91df-8a60abac81a0",
            "7f29d675-caff-43e1-8a53-1b8516ed2075"
        ]
    },
    "sessionControls": {
        "applicationEnforcedRestrictions": null,
        "persistentBrowser": null,
        "cloudAppSecurity": {
            "cloudAppSecurityType": "blockDownloads",
            "isEnabled": true
        },
        "signInFrequency": {
            "value": 4,
            "type": "hours",
            "isEnabled": true
        }
    }
}
```
# <a name="c"></a>[<span data-ttu-id="23ea8-164">C#</span><span class="sxs-lookup"><span data-stu-id="23ea8-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conditionalaccesspolicy-from-conditionalaccessroot-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23ea8-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23ea8-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conditionalaccesspolicy-from-conditionalaccessroot-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23ea8-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23ea8-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conditionalaccesspolicy-from-conditionalaccessroot-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23ea8-167">Java</span><span class="sxs-lookup"><span data-stu-id="23ea8-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conditionalaccesspolicy-from-conditionalaccessroot-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23ea8-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="23ea8-168">Response</span></span>

<span data-ttu-id="23ea8-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="23ea8-169">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/policies/$entity",
    "id": "6b5e999b-0ba8-4186-a106-e0296c1c4358",
    "displayName": "Demo app for documentation",
    "createdDateTime": "2019-09-26T23:12:16.0792706Z",
    "modifiedDateTime": null,
    "state": "disabled",
    "conditions": {
        "signInRiskLevels": [
            "high",
            "medium"
        ],
        "clientAppTypes": [
            "mobileAppsAndDesktopClients",
            "exchangeActiveSync",
            "other"
        ],
        "applications": {
            "includeApplications": [
                "All"
            ],
            "excludeApplications": [
                "499b84ac-1321-427f-aa17-267ca6975798",
                "00000007-0000-0000-c000-000000000000",
                "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
                "00000012-0000-0000-c000-000000000000",
                "797f4846-ba00-4fd7-ba43-dac1f8f63013",
                "05a65629-4c1b-48c1-a78b-804c4abdd4af",
                "7df0a125-d3be-4c96-aa54-591f83ff541c"
            ],
            "includeUserActions": []
        },
        "users": {
            "includeUsers": [
                "a702a13d-a437-4a07-8a7e-8c052de62dfd"
            ],
            "excludeUsers": [
                "124c5b6a-ffa5-483a-9b88-04c3fce5574a",
                "GuestsOrExternalUsers"
            ],
            "includeGroups": [],
            "excludeGroups": [],
            "includeRoles": [
                "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
                "cf1c38e5-3621-4004-a7cb-879624dced7c",
                "c4e39bd9-1100-46d3-8c65-fb160da0071f"
            ],
            "excludeRoles": [
                "b0f54661-2d74-4c50-afa3-1ec803f12efe"
            ]
        },
        "platforms": {
            "includePlatforms": [
                "all"
            ],
            "excludePlatforms": [
                "iOS",
                "windowsPhone"
            ]
        },
        "locations": {
            "includeLocations": [
                "AllTrusted"
            ],
            "excludeLocations": [
                "00000000-0000-0000-0000-000000000000",
                "d2136c9c-b049-47ae-b9cf-316e04ef7198"
            ]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa",
            "compliantDevice",
            "domainJoinedDevice",
            "approvedApplication",
            "compliantApplication"
        ],
        "customAuthenticationFactors": [],
        "termsOfUse": [
            "ce580154-086a-40fd-91df-8a60abac81a0",
            "7f29d675-caff-43e1-8a53-1b8516ed2075"
        ]
    },
    "sessionControls": {
        "applicationEnforcedRestrictions": null,
        "persistentBrowser": null,
        "cloudAppSecurity": {
            "cloudAppSecurityType": "blockDownloads",
            "isEnabled": true
        },
        "signInFrequency": {
            "value": 4,
            "type": "hours",
            "isEnabled": true
        }
    }
}
```

### <a name="example-4-require-mfa-to-exchange-online-from-non-compliant-devices"></a><span data-ttu-id="23ea8-170">Exemplo 4: Exigir MFA para o Exchange Online de dispositivos não compatíveis</span><span class="sxs-lookup"><span data-stu-id="23ea8-170">Example 4: Require MFA to Exchange Online from non-compliant devices</span></span>

#### <a name="request"></a><span data-ttu-id="23ea8-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23ea8-171">Request</span></span>
<span data-ttu-id="23ea8-172">O exemplo a seguir mostra uma solicitação para exigir MFA para o Exchange Online de dispositivos não compatíveis.</span><span class="sxs-lookup"><span data-stu-id="23ea8-172">The following example shows a request to require MFA to Exchange Online from non-compliant devices.</span></span>


# <a name="http"></a>[<span data-ttu-id="23ea8-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="23ea8-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot_4"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Require MFA to EXO from non-compliant devices.",
    "state": "enabled",
    "conditions": {
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ]
        },
        "users": {
            "includeGroups": ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa"
        ]
    }
}
```
# <a name="c"></a>[<span data-ttu-id="23ea8-174">C#</span><span class="sxs-lookup"><span data-stu-id="23ea8-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conditionalaccesspolicy-from-conditionalaccessroot-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23ea8-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23ea8-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conditionalaccesspolicy-from-conditionalaccessroot-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23ea8-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23ea8-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conditionalaccesspolicy-from-conditionalaccessroot-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23ea8-177">Java</span><span class="sxs-lookup"><span data-stu-id="23ea8-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conditionalaccesspolicy-from-conditionalaccessroot-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23ea8-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="23ea8-178">Response</span></span>

<span data-ttu-id="23ea8-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="23ea8-179">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/policies/$entity",
     "id": "b3f1298e-8e93-49af-bdbf-94cf7d453ca3",
    "displayName": "Require MFA to EXO from non-compliant devices.",
    "createdDateTime": "2020-04-01T00:55:12.9571747Z",
    "modifiedDateTime": null,
    "state": "enabled",
    "sessionControls": null,
    "conditions": {
        "userRiskLevels": [],
        "signInRiskLevels": [],
        "clientAppTypes": [
            "all"
        ],
        "platforms": null,
        "locations": null,
        "times": null,
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ],
            "excludeApplications": [],
            "includeUserActions": [],
            "includeProtectionLevels": []
        },
        "users": {
            "includeUsers": [],
            "excludeUsers": [],
            "includeGroups": [
                "ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"
            ],
            "excludeGroups": [],
            "includeRoles": [],
            "excludeRoles": []
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa"
        ],
        "customAuthenticationFactors": [],
        "termsOfUse": []
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

