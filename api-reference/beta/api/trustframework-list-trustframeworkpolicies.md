---
title: Listar trustFrameworkPolicies
description: Essa operação lista todos os objetos trustFrameworkPolicy em um locatário do Azure AD B2C.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 439573b524465d540e8c167ab9b3961d2c770f31
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215942"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="01f03-103">Listar trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="01f03-103">List trustFrameworkPolicies</span></span>

<span data-ttu-id="01f03-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01f03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01f03-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="01f03-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01f03-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="01f03-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01f03-107">Recupere uma lista de [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) no locatário/diretório.</span><span class="sxs-lookup"><span data-stu-id="01f03-107">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="01f03-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="01f03-108">Permissions</span></span>

<span data-ttu-id="01f03-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01f03-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01f03-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01f03-111">Permission type</span></span>      | <span data-ttu-id="01f03-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01f03-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01f03-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01f03-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01f03-114">Policy. Read. All, Policy. ReadWrite. TrustFramework</span><span class="sxs-lookup"><span data-stu-id="01f03-114">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="01f03-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01f03-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="01f03-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01f03-116">Not supported.</span></span>|
|<span data-ttu-id="01f03-117">Application</span><span class="sxs-lookup"><span data-stu-id="01f03-117">Application</span></span>|<span data-ttu-id="01f03-118">Policy. Read. All, Policy. ReadWrite. TrustFramework</span><span class="sxs-lookup"><span data-stu-id="01f03-118">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="01f03-119">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="01f03-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="01f03-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01f03-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01f03-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="01f03-121">Optional query parameters</span></span>

<span data-ttu-id="01f03-122">Este método oferece suporte `$select` aos `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="01f03-122">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01f03-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01f03-123">Request headers</span></span>

|<span data-ttu-id="01f03-124">Nome</span><span class="sxs-lookup"><span data-stu-id="01f03-124">Name</span></span>|<span data-ttu-id="01f03-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="01f03-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="01f03-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="01f03-126">Authorization</span></span>|<span data-ttu-id="01f03-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01f03-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01f03-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01f03-129">Request body</span></span>

<span data-ttu-id="01f03-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="01f03-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01f03-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="01f03-131">Response</span></span>

<span data-ttu-id="01f03-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) em uma representação JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01f03-132">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01f03-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01f03-133">Example</span></span>

<span data-ttu-id="01f03-134">O exemplo a seguir recupera todos os **trustFrameworkPolicies**.</span><span class="sxs-lookup"><span data-stu-id="01f03-134">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="01f03-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01f03-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="01f03-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="01f03-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustFrameworks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/policies
```
# <a name="c"></a>[<span data-ttu-id="01f03-137">C#</span><span class="sxs-lookup"><span data-stu-id="01f03-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01f03-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01f03-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01f03-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01f03-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="01f03-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="01f03-140">Response</span></span>

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
