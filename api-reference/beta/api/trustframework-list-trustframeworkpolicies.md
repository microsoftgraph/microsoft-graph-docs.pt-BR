---
title: Listar trustFrameworkPolicies
description: Essa operação lista todos os objetos trustFrameworkPolicy em um locatário do Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8515d73db6740d2e1dbf4b2fc90368c02515c70e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421173"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="ae13f-103">Listar trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="ae13f-103">List trustFrameworkPolicies</span></span>

> <span data-ttu-id="ae13f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ae13f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae13f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ae13f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae13f-106">Recupere uma lista de [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) no locatário/diretório.</span><span class="sxs-lookup"><span data-stu-id="ae13f-106">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae13f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae13f-107">Permissions</span></span>

<span data-ttu-id="ae13f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae13f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae13f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae13f-110">Permission type</span></span>      | <span data-ttu-id="ae13f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae13f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae13f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae13f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae13f-113">Policy. Read. TrustFramework, Policy. Read. All</span><span class="sxs-lookup"><span data-stu-id="ae13f-113">Policy.Read.TrustFramework, Policy.Read.All</span></span>|
|<span data-ttu-id="ae13f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae13f-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ae13f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae13f-115">Not supported.</span></span>|
|<span data-ttu-id="ae13f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae13f-116">Application</span></span>|<span data-ttu-id="ae13f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae13f-117">Not supported.</span></span>|

<span data-ttu-id="ae13f-118">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="ae13f-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="ae13f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae13f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae13f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ae13f-120">Optional query parameters</span></span>

<span data-ttu-id="ae13f-121">Este método oferece suporte `$select` aos `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ae13f-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae13f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae13f-122">Request headers</span></span>

|<span data-ttu-id="ae13f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ae13f-123">Name</span></span>|<span data-ttu-id="ae13f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae13f-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ae13f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae13f-125">Authorization</span></span>|<span data-ttu-id="ae13f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae13f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae13f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae13f-128">Request body</span></span>

<span data-ttu-id="ae13f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae13f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae13f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae13f-130">Response</span></span>

<span data-ttu-id="ae13f-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) em uma representação JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae13f-131">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae13f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae13f-132">Example</span></span>

<span data-ttu-id="ae13f-133">O exemplo a seguir recupera todos os **trustFrameworkPolicies**.</span><span class="sxs-lookup"><span data-stu-id="ae13f-133">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="ae13f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae13f-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ae13f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae13f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustFrameworks"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ae13f-136">C#</span><span class="sxs-lookup"><span data-stu-id="ae13f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae13f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae13f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ae13f-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ae13f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ae13f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae13f-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "B2C_1A_CustomPolicy2"
        },
        {
            "id": "B2C_1A_CustomPolicy3"
        },
        {
            "id": "B2C_1A_SocialAndLocalAccounts_Base"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
