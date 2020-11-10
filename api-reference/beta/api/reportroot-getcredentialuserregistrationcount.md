---
title: 'reportRoot: getCredentialUserRegistrationCount'
description: Informe o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e de autenticação multifator (MFA).
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 6f1d6bd3eaa95998ff969437048d20931023a31a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966795"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="dc196-103">reportRoot: getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="dc196-103">reportRoot: getCredentialUserRegistrationCount</span></span>

<span data-ttu-id="dc196-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc196-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc196-105">Informe o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e de autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="dc196-105">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc196-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc196-106">Permissions</span></span>

<span data-ttu-id="dc196-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc196-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dc196-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc196-109">Permission type</span></span>                        | <span data-ttu-id="dc196-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc196-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dc196-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc196-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc196-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc196-112">Reports.Read.All</span></span> |
| <span data-ttu-id="dc196-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc196-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc196-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc196-114">Not supported.</span></span> |
| <span data-ttu-id="dc196-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc196-115">Application</span></span>                            | <span data-ttu-id="dc196-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc196-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc196-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc196-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="dc196-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc196-118">Request headers</span></span>

| <span data-ttu-id="dc196-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dc196-119">Name</span></span>          | <span data-ttu-id="dc196-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc196-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dc196-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc196-121">Authorization</span></span> | <span data-ttu-id="dc196-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="dc196-122">Bearer {token}</span></span> |
| <span data-ttu-id="dc196-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc196-123">Content-Type</span></span> | <span data-ttu-id="dc196-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dc196-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc196-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc196-125">Request body</span></span>

<span data-ttu-id="dc196-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc196-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc196-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc196-127">Response</span></span>

<span data-ttu-id="dc196-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto da coleção [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc196-128">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dc196-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dc196-129">Examples</span></span>

<span data-ttu-id="dc196-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="dc196-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="dc196-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc196-131">Request</span></span>

<span data-ttu-id="dc196-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc196-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dc196-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc196-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```
# <a name="c"></a>[<span data-ttu-id="dc196-134">C#</span><span class="sxs-lookup"><span data-stu-id="dc196-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialuserregistrationcount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc196-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc196-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialuserregistrationcount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc196-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc196-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialuserregistrationcount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc196-137">Java</span><span class="sxs-lookup"><span data-stu-id="dc196-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getcredentialuserregistrationcount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dc196-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc196-138">Response</span></span>

<span data-ttu-id="dc196-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dc196-139">The following is an example of the response.</span></span>

> <span data-ttu-id="dc196-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dc196-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dc196-141">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc196-141">All the properties are returned from an actual call.</span></span>

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


