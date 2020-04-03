---
title: Listar aplicativos
description: Obtenha a lista de applications nesta organização.
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9a12773de45e8f79fca57d17df1668ccd3a32c9d
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108372"
---
# <a name="list-applications"></a><span data-ttu-id="075b7-103">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="075b7-103">List applications</span></span>

<span data-ttu-id="075b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="075b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="075b7-105">Obtenha a lista de [applications](../resources/application.md) nesta organização.</span><span class="sxs-lookup"><span data-stu-id="075b7-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="075b7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="075b7-106">Permissions</span></span>
<span data-ttu-id="075b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="075b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="075b7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="075b7-109">Permission type</span></span>      | <span data-ttu-id="075b7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="075b7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="075b7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="075b7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="075b7-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="075b7-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="075b7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="075b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="075b7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="075b7-114">Not supported.</span></span>    |
|<span data-ttu-id="075b7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="075b7-115">Application</span></span> | <span data-ttu-id="075b7-116">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="075b7-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="075b7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="075b7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="075b7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="075b7-118">Optional query parameters</span></span>
<span data-ttu-id="075b7-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="075b7-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="075b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="075b7-120">Request headers</span></span>
| <span data-ttu-id="075b7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="075b7-121">Name</span></span>       | <span data-ttu-id="075b7-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="075b7-122">Type</span></span> | <span data-ttu-id="075b7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="075b7-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="075b7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="075b7-124">Authorization</span></span>  | <span data-ttu-id="075b7-125">string</span><span class="sxs-lookup"><span data-stu-id="075b7-125">string</span></span>  | <span data-ttu-id="075b7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="075b7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="075b7-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="075b7-128">Content-type</span></span>   | <span data-ttu-id="075b7-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="075b7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="075b7-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="075b7-131">Request body</span></span>
<span data-ttu-id="075b7-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="075b7-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="075b7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="075b7-133">Response</span></span>

<span data-ttu-id="075b7-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="075b7-134">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="075b7-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="075b7-135">Examples</span></span>
### <a name="request"></a><span data-ttu-id="075b7-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="075b7-136">Request</span></span>
<span data-ttu-id="075b7-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="075b7-137">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="075b7-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="075b7-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications
```
# <a name="c"></a>[<span data-ttu-id="075b7-139">C#</span><span class="sxs-lookup"><span data-stu-id="075b7-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="075b7-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="075b7-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="075b7-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="075b7-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="075b7-142">Java</span><span class="sxs-lookup"><span data-stu-id="075b7-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="075b7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="075b7-143">Response</span></span>
<span data-ttu-id="075b7-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="075b7-144">Here is an example of the response.</span></span> 

> <span data-ttu-id="075b7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="075b7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
