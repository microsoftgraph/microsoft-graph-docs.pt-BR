---
title: Listar trustFrameworkPolicies
description: Essa operação lista todos os objetos trustFrameworkPolicy em um locatário do Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 67531e5364256e55bb94f88647b1b56a915dce36
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867948"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="bd597-103">Listar trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="bd597-103">List trustFrameworkPolicies</span></span>

> <span data-ttu-id="bd597-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bd597-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd597-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bd597-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd597-106">Recupere uma lista de [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) no locatário/diretório.</span><span class="sxs-lookup"><span data-stu-id="bd597-106">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd597-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd597-107">Permissions</span></span>

<span data-ttu-id="bd597-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd597-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd597-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd597-110">Permission type</span></span>      | <span data-ttu-id="bd597-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd597-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd597-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd597-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bd597-113">Policy. Read. TrustFramework, Policy. Read. All</span><span class="sxs-lookup"><span data-stu-id="bd597-113">Policy.Read.TrustFramework, Policy.Read.All</span></span>|
|<span data-ttu-id="bd597-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd597-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="bd597-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd597-115">Not supported.</span></span>|
|<span data-ttu-id="bd597-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd597-116">Application</span></span>|<span data-ttu-id="bd597-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd597-117">Not supported.</span></span>|

<span data-ttu-id="bd597-118">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="bd597-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="bd597-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd597-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bd597-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bd597-120">Optional query parameters</span></span>

<span data-ttu-id="bd597-121">Este método oferece suporte `$select` aos `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bd597-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd597-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd597-122">Request headers</span></span>

|<span data-ttu-id="bd597-123">Nome</span><span class="sxs-lookup"><span data-stu-id="bd597-123">Name</span></span>|<span data-ttu-id="bd597-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd597-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="bd597-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd597-125">Authorization</span></span>|<span data-ttu-id="bd597-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd597-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd597-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd597-128">Request body</span></span>

<span data-ttu-id="bd597-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd597-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd597-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd597-130">Response</span></span>

<span data-ttu-id="bd597-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) em uma representação JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd597-131">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd597-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd597-132">Example</span></span>

<span data-ttu-id="bd597-133">O exemplo a seguir recupera todos os **trustFrameworkPolicies**.</span><span class="sxs-lookup"><span data-stu-id="bd597-133">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="bd597-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd597-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bd597-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd597-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustFrameworks"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bd597-136">C#</span><span class="sxs-lookup"><span data-stu-id="bd597-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd597-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="bd597-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bd597-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bd597-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bd597-139">Java</span><span class="sxs-lookup"><span data-stu-id="bd597-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-trustframeworks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bd597-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd597-140">Response</span></span>

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
