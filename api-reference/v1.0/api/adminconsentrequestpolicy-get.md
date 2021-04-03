---
title: Obter adminConsentRequestPolicy
description: Leia as propriedades e as relações de um objeto adminConsentRequestPolicy.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: cfbd3cd98c17c9e261711932a0169c977b1d59ba
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508285"
---
# <a name="get-adminconsentrequestpolicy"></a><span data-ttu-id="2b54c-103">Obter adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="2b54c-103">Get adminConsentRequestPolicy</span></span>

<span data-ttu-id="2b54c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b54c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b54c-105">Leia as propriedades e as relações de um [objeto adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2b54c-105">Read the properties and relationships of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b54c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b54c-106">Permissions</span></span>

<span data-ttu-id="2b54c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b54c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b54c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b54c-109">Permission type</span></span>|<span data-ttu-id="2b54c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b54c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b54c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b54c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2b54c-112">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b54c-112">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="2b54c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b54c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b54c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b54c-114">Not supported.</span></span>|
|<span data-ttu-id="2b54c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b54c-115">Application</span></span>|<span data-ttu-id="2b54c-116">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b54c-116">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span></span>|

<span data-ttu-id="2b54c-117">Ao chamar em nome de um usuário, o usuário precisa pertencer a uma das seguintes funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="2b54c-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="2b54c-118">Para saber mais sobre funções de diretório, consulte Funções do [Azure AD integrados](/azure/active-directory/roles/permissions-reference):</span><span class="sxs-lookup"><span data-stu-id="2b54c-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="2b54c-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="2b54c-119">Global Administrator</span></span>
+ <span data-ttu-id="2b54c-120">Leitor global</span><span class="sxs-lookup"><span data-stu-id="2b54c-120">Global Reader</span></span>
+ <span data-ttu-id="2b54c-121">Administrador de Aplicativos de Nuvem</span><span class="sxs-lookup"><span data-stu-id="2b54c-121">Cloud Application Administrator</span></span>
+ <span data-ttu-id="2b54c-122">Administrador de Aplicativos</span><span class="sxs-lookup"><span data-stu-id="2b54c-122">Application Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="2b54c-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b54c-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/adminConsentRequestPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b54c-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2b54c-124">Optional query parameters</span></span>

<span data-ttu-id="2b54c-125">Este método dá suporte ao  `$select`   parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2b54c-125">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="2b54c-126">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2b54c-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b54c-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b54c-127">Request headers</span></span>

|<span data-ttu-id="2b54c-128">Nome</span><span class="sxs-lookup"><span data-stu-id="2b54c-128">Name</span></span>|<span data-ttu-id="2b54c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b54c-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2b54c-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b54c-130">Authorization</span></span>|<span data-ttu-id="2b54c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b54c-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b54c-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b54c-133">Request body</span></span>

<span data-ttu-id="2b54c-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b54c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b54c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b54c-135">Response</span></span>

<span data-ttu-id="2b54c-136">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b54c-136">If successful, this method returns a `200 OK` response code and an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b54c-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2b54c-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b54c-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b54c-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2b54c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b54c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_adminconsentrequestpolicy"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/adminConsentRequestPolicy
```
# <a name="c"></a>[<span data-ttu-id="2b54c-140">C#</span><span class="sxs-lookup"><span data-stu-id="2b54c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-adminconsentrequestpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b54c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b54c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-adminconsentrequestpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b54c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b54c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-adminconsentrequestpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b54c-143">Java</span><span class="sxs-lookup"><span data-stu-id="2b54c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-adminconsentrequestpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2b54c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b54c-144">Response</span></span>

<span data-ttu-id="2b54c-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2b54c-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.adminConsentRequestPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/adminConsentRequestPolicy/$entity",
  "isEnabled": true,
  "notifyReviewers": false,
  "remindersEnabled": false,
  "requestDurationInDays": 0,
  "version": 0,
  "reviewers": [
    {
      "query": "/users/906e0ee5-6372-4cc8-8248-fdf2846b48ed",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    },
    {
      "query": "/users/daddef1a-acb0-4f62-96d0-49df2495d657",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ]
}
```
