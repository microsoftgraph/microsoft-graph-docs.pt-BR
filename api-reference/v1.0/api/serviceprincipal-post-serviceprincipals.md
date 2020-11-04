---
title: Criar serviceprincipal
description: Criar um novo objeto do servicePrincipal.
author: sureshja
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fa5641c79a165a0b65e7173f57a17f9440c4912b
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905367"
---
# <a name="create-serviceprincipal"></a><span data-ttu-id="0bddf-103">Criar servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="0bddf-103">Create servicePrincipal</span></span>

<span data-ttu-id="0bddf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bddf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0bddf-105">Criar um novo objeto do [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="0bddf-105">Create a new [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0bddf-106">Não há suporte para a adição de [**passwordCredential**](../resources/passwordcredential.md) durante a criação de servicePrincipals.</span><span class="sxs-lookup"><span data-stu-id="0bddf-106">Adding [**passwordCredential**](../resources/passwordcredential.md) when creating servicePrincipals is not supported.</span></span> <span data-ttu-id="0bddf-107">Use o método [addpassword](serviceprincipal-addpassword.md) para adicionar senhas a um servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="0bddf-107">Use the [addPassword](serviceprincipal-addpassword.md) method to add passwords for a servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bddf-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0bddf-108">Permissions</span></span>
<span data-ttu-id="0bddf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bddf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0bddf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bddf-111">Permission type</span></span>      | <span data-ttu-id="0bddf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0bddf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bddf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bddf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0bddf-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0bddf-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0bddf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bddf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bddf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bddf-116">Not supported.</span></span>    |
|<span data-ttu-id="0bddf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bddf-117">Application</span></span> | <span data-ttu-id="0bddf-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bddf-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bddf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bddf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals
```

## <a name="request-headers"></a><span data-ttu-id="0bddf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bddf-120">Request headers</span></span>
| <span data-ttu-id="0bddf-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0bddf-121">Name</span></span>       | <span data-ttu-id="0bddf-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bddf-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="0bddf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bddf-123">Authorization</span></span> | <span data-ttu-id="0bddf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bddf-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0bddf-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0bddf-126">Content-Type</span></span> | <span data-ttu-id="0bddf-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bddf-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0bddf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bddf-129">Request body</span></span>
<span data-ttu-id="0bddf-130">No corpo da solicitação, forneça uma representação JSON de um objeto [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="0bddf-130">In the request body, supply a JSON representation of a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span> <span data-ttu-id="0bddf-131">O corpo da solicitação deve conter  **appId**.</span><span class="sxs-lookup"><span data-stu-id="0bddf-131">The request body must contain  **appId**.</span></span>

## <a name="response"></a><span data-ttu-id="0bddf-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bddf-132">Response</span></span>

<span data-ttu-id="0bddf-133">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bddf-133">If successful, this method returns a `201 Created` response code and a [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0bddf-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0bddf-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="0bddf-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bddf-135">Request</span></span>
<span data-ttu-id="0bddf-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bddf-136">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0bddf-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0bddf-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_serviceprincipal_from_serviceprincipals"
}-->
```http
POST https://graph.microsoft.com/v1.0/servicePrincipals
Content-type: application/json

{
  "appId": "65415bb1-9267-4313-bbf5-ae259732ee12"
}
```
# <a name="c"></a>[<span data-ttu-id="0bddf-138">C#</span><span class="sxs-lookup"><span data-stu-id="0bddf-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-serviceprincipal-from-serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0bddf-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0bddf-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-serviceprincipal-from-serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0bddf-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0bddf-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-serviceprincipal-from-serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0bddf-141">Java</span><span class="sxs-lookup"><span data-stu-id="0bddf-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-serviceprincipal-from-serviceprincipals-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0bddf-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bddf-142">Response</span></span>
<span data-ttu-id="0bddf-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bddf-143">Here is an example of the response.</span></span> 

> <span data-ttu-id="0bddf-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0bddf-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals/$entity",
    "id": "59e617e5-e447-4adc-8b88-00af644d7c92",
    "deletedDateTime": null,
    "accountEnabled": true,
    "appDisplayName": "My App",
    "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
    "appOwnerOrganizationId": "1bc1c026-2f7b-48a5-98da-afa2fd8bc7bc",
    "appRoleAssignmentRequired": false,
    "displayName": "foo",
    "homepage": null,
    "logoutUrl": null,
    "publisherName": "Contoso",
    "replyUrls": [],
    "servicePrincipalNames": [
        "f1bd758f-4a1a-4b71-aa20-a248a22a8928"
    ],
    "tags": [],
    "addIns": [],
    "appRoles": [],
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "oauth2PermissionScopes": [],
    "passwordCredentials": []
}
```

