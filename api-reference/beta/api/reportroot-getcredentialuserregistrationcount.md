---
title: 'reportRoot: getCredentialUserRegistrationCount'
description: Informe o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e de autenticação multifator (MFA).
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 4b15f41298ae4c6e411d5a8de832f243b277d84e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454491"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="bce38-103">reportRoot: getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="bce38-103">reportRoot: getCredentialUserRegistrationCount</span></span>

<span data-ttu-id="bce38-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bce38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bce38-105">Informe o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e de autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="bce38-105">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="bce38-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bce38-106">Permissions</span></span>

<span data-ttu-id="bce38-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bce38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bce38-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bce38-109">Permission type</span></span>                        | <span data-ttu-id="bce38-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bce38-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bce38-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bce38-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bce38-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bce38-112">Reports.Read.All</span></span> |
| <span data-ttu-id="bce38-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bce38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bce38-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bce38-114">Not supported.</span></span> |
| <span data-ttu-id="bce38-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bce38-115">Application</span></span>                            | <span data-ttu-id="bce38-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bce38-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bce38-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bce38-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="bce38-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bce38-118">Request headers</span></span>

| <span data-ttu-id="bce38-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bce38-119">Name</span></span>          | <span data-ttu-id="bce38-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bce38-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bce38-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bce38-121">Authorization</span></span> | <span data-ttu-id="bce38-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="bce38-122">Bearer {token}</span></span> |
| <span data-ttu-id="bce38-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bce38-123">Content-Type</span></span> | <span data-ttu-id="bce38-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bce38-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bce38-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bce38-125">Request body</span></span>

<span data-ttu-id="bce38-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bce38-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bce38-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bce38-127">Response</span></span>

<span data-ttu-id="bce38-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto da coleção [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bce38-128">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bce38-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bce38-129">Examples</span></span>

<span data-ttu-id="bce38-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="bce38-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="bce38-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bce38-131">Request</span></span>

<span data-ttu-id="bce38-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bce38-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bce38-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bce38-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```
# <a name="c"></a>[<span data-ttu-id="bce38-134">C#</span><span class="sxs-lookup"><span data-stu-id="bce38-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialuserregistrationcount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bce38-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bce38-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialuserregistrationcount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bce38-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bce38-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialuserregistrationcount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bce38-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="bce38-137">Response</span></span>

<span data-ttu-id="bce38-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bce38-138">The following is an example of the response.</span></span>

> <span data-ttu-id="bce38-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bce38-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bce38-140">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bce38-140">All the properties are returned from an actual call.</span></span>

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
