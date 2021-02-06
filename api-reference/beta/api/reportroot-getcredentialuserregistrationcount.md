---
title: 'reportRoot: getCredentialUserRegistrationCount'
description: Relatar o estado atual de quantos usuários em sua organização estão registrados para redefinição de senha de autoatendado e recursos de autenticação multifatória (MFA).
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 7224d49e71933716fb36b90dfe5cbb2b0d99223f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131345"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="55a73-103">reportRoot: getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="55a73-103">reportRoot: getCredentialUserRegistrationCount</span></span>

<span data-ttu-id="55a73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55a73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55a73-105">Relatar o estado atual de quantos usuários em sua organização estão registrados para redefinição de senha de autoatendado e recursos de autenticação multifatória (MFA).</span><span class="sxs-lookup"><span data-stu-id="55a73-105">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="55a73-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="55a73-106">Permissions</span></span>

<span data-ttu-id="55a73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55a73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55a73-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55a73-109">Permission type</span></span>                        | <span data-ttu-id="55a73-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55a73-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="55a73-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55a73-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="55a73-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="55a73-112">Reports.Read.All</span></span> |
| <span data-ttu-id="55a73-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55a73-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55a73-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55a73-114">Not supported.</span></span> |
| <span data-ttu-id="55a73-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55a73-115">Application</span></span>                            | <span data-ttu-id="55a73-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="55a73-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55a73-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55a73-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="55a73-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55a73-118">Request headers</span></span>

| <span data-ttu-id="55a73-119">Nome</span><span class="sxs-lookup"><span data-stu-id="55a73-119">Name</span></span>          | <span data-ttu-id="55a73-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="55a73-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="55a73-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="55a73-121">Authorization</span></span> | <span data-ttu-id="55a73-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="55a73-122">Bearer {token}</span></span> |
| <span data-ttu-id="55a73-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55a73-123">Content-Type</span></span> | <span data-ttu-id="55a73-124">application/json</span><span class="sxs-lookup"><span data-stu-id="55a73-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="55a73-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55a73-125">Request body</span></span>

<span data-ttu-id="55a73-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55a73-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55a73-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="55a73-127">Response</span></span>

<span data-ttu-id="55a73-128">Se tiver êxito, este método retornará um código de resposta e um novo objeto da coleção `200 OK` [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55a73-128">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55a73-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="55a73-129">Examples</span></span>

<span data-ttu-id="55a73-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="55a73-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="55a73-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55a73-131">Request</span></span>

<span data-ttu-id="55a73-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55a73-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55a73-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="55a73-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```
# <a name="c"></a>[<span data-ttu-id="55a73-134">C#</span><span class="sxs-lookup"><span data-stu-id="55a73-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialuserregistrationcount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55a73-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55a73-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialuserregistrationcount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55a73-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55a73-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialuserregistrationcount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55a73-137">Java</span><span class="sxs-lookup"><span data-stu-id="55a73-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getcredentialuserregistrationcount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="55a73-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="55a73-138">Response</span></span>

<span data-ttu-id="55a73-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55a73-139">The following is an example of the response.</span></span>

> <span data-ttu-id="55a73-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55a73-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="55a73-141">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55a73-141">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.credentialUserRegistrationCount)",
  "value": [
    {
      "id" : "id-value",
      "totalUserCount" : 23123,
      "userRegistrationCounts" :
      [
        { "userRegistrationStatus":"registered", 
          "userRegistationCount": 23423 }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reportRoot: getCredentialUserRegistrationCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


