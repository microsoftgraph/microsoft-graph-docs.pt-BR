---
title: 'reportRoot: getCredentialUserRegistrationCount'
description: Informe o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e de autenticação multifator (MFA).
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: db1324efe4148deefeb83f662ab363f0671d9da4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874093"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="da716-103">reportRoot: getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="da716-103">reportRoot: getCredentialUserRegistrationCount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da716-104">Informe o estado atual de quantos usuários da sua organização estão registrados para recursos de redefinição de senha de autoatendimento e de autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="da716-104">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="da716-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="da716-105">Permissions</span></span>

<span data-ttu-id="da716-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da716-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da716-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da716-108">Permission type</span></span>                        | <span data-ttu-id="da716-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da716-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="da716-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da716-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="da716-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="da716-111">Reports.Read.All</span></span> |
| <span data-ttu-id="da716-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da716-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da716-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da716-113">Not supported.</span></span> |
| <span data-ttu-id="da716-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da716-114">Application</span></span>                            | <span data-ttu-id="da716-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="da716-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da716-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da716-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="da716-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da716-117">Request headers</span></span>

| <span data-ttu-id="da716-118">Nome</span><span class="sxs-lookup"><span data-stu-id="da716-118">Name</span></span>          | <span data-ttu-id="da716-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="da716-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="da716-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="da716-120">Authorization</span></span> | <span data-ttu-id="da716-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="da716-121">Bearer {token}</span></span> |
| <span data-ttu-id="da716-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da716-122">Content-Type</span></span> | <span data-ttu-id="da716-123">application/json</span><span class="sxs-lookup"><span data-stu-id="da716-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="da716-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da716-124">Request body</span></span>

<span data-ttu-id="da716-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da716-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da716-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="da716-126">Response</span></span>

<span data-ttu-id="da716-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto da coleção [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da716-127">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da716-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="da716-128">Examples</span></span>

<span data-ttu-id="da716-129">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="da716-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="da716-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da716-130">Request</span></span>

<span data-ttu-id="da716-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="da716-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="da716-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="da716-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="da716-133">C#</span><span class="sxs-lookup"><span data-stu-id="da716-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialuserregistrationcount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da716-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="da716-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialuserregistrationcount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="da716-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="da716-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialuserregistrationcount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="da716-136">Java</span><span class="sxs-lookup"><span data-stu-id="da716-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getcredentialuserregistrationcount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="da716-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="da716-137">Response</span></span>

<span data-ttu-id="da716-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="da716-138">The following is an example of the response.</span></span>

> <span data-ttu-id="da716-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="da716-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="da716-140">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da716-140">All the properties are returned from an actual call.</span></span>

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
