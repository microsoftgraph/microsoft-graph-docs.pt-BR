---
title: Listar aplicativos
description: Obtenha a lista de applications nesta organização.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 801f568d7f4ee6ad905fec1648683acdc8133d3d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939702"
---
# <a name="list-applications"></a><span data-ttu-id="389f6-103">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="389f6-103">List applications</span></span>

<span data-ttu-id="389f6-104">Obtenha a lista de [applications](../resources/application.md) nesta organização.</span><span class="sxs-lookup"><span data-stu-id="389f6-104">Retrieve the list of applications in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="389f6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="389f6-105">Permissions</span></span>
<span data-ttu-id="389f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="389f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="389f6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="389f6-108">Permission type</span></span>      | <span data-ttu-id="389f6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="389f6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="389f6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="389f6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="389f6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="389f6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="389f6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="389f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="389f6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="389f6-113">Not supported.</span></span>    |
|<span data-ttu-id="389f6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="389f6-114">Application</span></span> | <span data-ttu-id="389f6-115">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="389f6-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="389f6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="389f6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="389f6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="389f6-117">Optional query parameters</span></span>
<span data-ttu-id="389f6-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="389f6-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="389f6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="389f6-119">Request headers</span></span>
| <span data-ttu-id="389f6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="389f6-120">Name</span></span>       | <span data-ttu-id="389f6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="389f6-121">Type</span></span> | <span data-ttu-id="389f6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="389f6-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="389f6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="389f6-123">Authorization</span></span>  | <span data-ttu-id="389f6-124">string</span><span class="sxs-lookup"><span data-stu-id="389f6-124">string</span></span>  | <span data-ttu-id="389f6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="389f6-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="389f6-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="389f6-127">Content-type</span></span>   | <span data-ttu-id="389f6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="389f6-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="389f6-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="389f6-130">Request body</span></span>
<span data-ttu-id="389f6-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="389f6-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="389f6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="389f6-132">Response</span></span>

<span data-ttu-id="389f6-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="389f6-133">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="389f6-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="389f6-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="389f6-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="389f6-135">Request</span></span>
<span data-ttu-id="389f6-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="389f6-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_application"
}-->

```http
GET https://graph.microsoft.com/v1.0/applications
```

### <a name="response"></a><span data-ttu-id="389f6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="389f6-137">Response</span></span>
<span data-ttu-id="389f6-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="389f6-138">Here is an example of the response.</span></span> 

> <span data-ttu-id="389f6-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="389f6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1229

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications",
    "value": [
        {
            "id": "00af5dfb-85da-4b41-a677-0c6b86dd34f8",
            "deletedDateTime": null,
            "isFallbackPublicClient": false,
            "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
            "applicationTemplateId": null,
            "identifierUris": [
                "http://contoso/a7770d29-4321-41a6-b863-ca11d6639448"
            ],
            "createdDateTime": "2019-09-15T05:23:08Z",
            "displayName": "My app",
            "isDeviceOnlyAuthSupported": null,
            "groupMembershipClaims": null,
            "optionalClaims": null,
            "orgRestrictions": [],
            "publisherDomain": "contoso.onmicrosoft.com",
            "signInAudience": "AzureADMyOrg",
            "tags": [],
            "tokenEncryptionKeyId": null,
            "api": {
                "requestedAccessTokenVersion": null,
                "acceptMappedClaims": null,
                "knownClientApplications": [],
                "oauth2PermissionScopes": [],
                "preAuthorizedApplications": []
            },
            "appRoles": [],
            "publicClient": {
                "redirectUris": []
            },
            "info": {
                "termsOfServiceUrl": null,
                "supportUrl": null,
                "privacyStatementUrl": null,
                "marketingUrl": null,
                "logoUrl": null
            },
            "keyCredentials": [],
            "parentalControlSettings": {
                "countriesBlockedForMinors": [],
                "legalAgeGroupRule": "Allow"
            },
            "passwordCredentials": [],
            "requiredResourceAccess": [],
            "web": {
                "redirectUris": [
                    "https://127.0.0.1:444/applications/default.aspx"
                ],
                "homePageUrl": "http://www.contoso.com/landingPage",
                "logoutUrl": null,
                "implicitGrantSettings": {
                    "enableIdTokenIssuance": true,
                    "enableAccessTokenIssuance": false
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
