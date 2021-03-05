---
title: 'applicationTemplate: instaurá-lo'
description: Adicione uma instância de um aplicativo da galeria de aplicativos do Azure AD ao diretório.
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: a059931c14a8aa81190162deb9f35ef28a2173cc
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471387"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="37e65-103">applicationTemplate: instaurá-lo</span><span class="sxs-lookup"><span data-stu-id="37e65-103">applicationTemplate: instantiate</span></span>

<span data-ttu-id="37e65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37e65-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37e65-105">Adicione uma instância de um aplicativo da galeria de aplicativos do Azure AD ao diretório.</span><span class="sxs-lookup"><span data-stu-id="37e65-105">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="37e65-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37e65-106">Permissions</span></span>

<span data-ttu-id="37e65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37e65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37e65-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37e65-109">Permission type</span></span>                        | <span data-ttu-id="37e65-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37e65-110">Permissions (from least to most privileged)</span></span>        |
| :------------------------------------- | :------------------------------------------------- |
| <span data-ttu-id="37e65-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37e65-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="37e65-112">Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37e65-112">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="37e65-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37e65-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37e65-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37e65-114">Not supported.</span></span>                                     |
| <span data-ttu-id="37e65-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37e65-115">Application</span></span>                            | <span data-ttu-id="37e65-116">Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37e65-116">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37e65-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37e65-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="37e65-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37e65-118">Request headers</span></span>

| <span data-ttu-id="37e65-119">Nome</span><span class="sxs-lookup"><span data-stu-id="37e65-119">Name</span></span>          | <span data-ttu-id="37e65-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="37e65-120">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="37e65-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="37e65-121">Authorization</span></span> | <span data-ttu-id="37e65-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="37e65-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="37e65-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37e65-123">Request body</span></span>

<span data-ttu-id="37e65-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37e65-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="37e65-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="37e65-125">Parameter</span></span>   | <span data-ttu-id="37e65-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="37e65-126">Type</span></span>   | <span data-ttu-id="37e65-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="37e65-127">Description</span></span>                    |
| :---------- | :----- | :----------------------------- |
| <span data-ttu-id="37e65-128">displayName</span><span class="sxs-lookup"><span data-stu-id="37e65-128">displayName</span></span> | <span data-ttu-id="37e65-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37e65-129">String</span></span> | <span data-ttu-id="37e65-130">Nome personalizado do aplicativo</span><span class="sxs-lookup"><span data-stu-id="37e65-130">Custom name of the application</span></span> |

## <a name="response"></a><span data-ttu-id="37e65-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="37e65-131">Response</span></span>

<span data-ttu-id="37e65-132">Se tiver êxito, este método retornará um código de resposta e um `201 OK` novo [objeto applicationServicePrincipal](../resources/applicationserviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37e65-132">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37e65-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37e65-133">Examples</span></span>

<span data-ttu-id="37e65-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="37e65-134">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="37e65-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37e65-135">Request</span></span>

<span data-ttu-id="37e65-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37e65-136">The following is an example of the request.</span></span>

> <span data-ttu-id="37e65-137">Você pode usar essa API para insinuar [aplicativos que não são da galeria.](/azure/active-directory/manage-apps/add-non-gallery-app)</span><span class="sxs-lookup"><span data-stu-id="37e65-137">You can use this API to instantiate [non-gallery apps](/azure/active-directory/manage-apps/add-non-gallery-app).</span></span> <span data-ttu-id="37e65-138">Use a ID a seguir para **applicationTemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` .</span><span class="sxs-lookup"><span data-stu-id="37e65-138">Use the following ID for **applicationTemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>

<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```http
POST https://graph.microsoft.com/v1.0/applicationTemplates/{id}/instantiate
Content-type: application/json

{
  "displayName": "My custom name"
}
```

### <a name="response"></a><span data-ttu-id="37e65-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="37e65-139">Response</span></span>

<span data-ttu-id="37e65-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37e65-140">The following is an example of the response.</span></span>

> <span data-ttu-id="37e65-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37e65-141">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json

{
   "servicePrincipal": {
      "accountEnabled": true,
      "addIns": [],
      "alternativeNames": ["http://contoso/a7770d29-4321-41a6-b863-ca11d6639448"],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired":true,
      "appRoles": [],
      "displayName": "Display name",
      "endpoints": [],
      "homepage": null,
      "id": "id-value",
      "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
      },
      "keyCredentials": [],
      "logoutUrl": null,
      "oauth2PermissionScopes": [],
      "passwordCredentials": [],
      "publisherName": null,
      "replyUrls": [],
      "servicePrincipalNames": [],
      "servicePrincipalType": null,
      "tags": [],
      "tokenEncryptionKeyId": null
   },
   "application": {
            "id": "id-value",
            "isFallbackPublicClient": null,
            "appId": "appId-value",
            "applicationTemplateId": null,
            "identifierUris": [],
            "createdDateTime": "2019-09-17T19:10:35.2742618Z",
            "displayName": "Display name",
            "isDeviceOnlyAuthSupported": null,
            "groupMembershipClaims": null,
            "optionalClaims": null,
            "addIns": [],
            "publisherDomain": "contoso.onmicrosoft.com",
            "signInAudience": "AzureADMyOrg",
            "tags": [],
            "tokenEncryptionKeyId": null,
            "api": {
                    "requestedAccessTokenVersion": 2,
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
                    "redirectUris": [],
                    "homePageUrl": null,
                    "logoutUrl": null,
                    "implicitGrantSettings": {
                            "enableIdTokenIssuance": false,
                            "enableAccessTokenIssuance": false
                    }
            }
   }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate: instantiate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
