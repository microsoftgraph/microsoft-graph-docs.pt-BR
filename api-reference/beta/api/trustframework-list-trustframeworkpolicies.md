---
title: Listar trustFrameworkPolicies
description: Essa operação lista todos os objetos trustFrameworkPolicy em um locatário do Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: afdaf352494b0f68f37d88707fad98aa9373969a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637448"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="f1080-103">Listar trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="f1080-103">List trustFrameworkPolicies</span></span>

> <span data-ttu-id="f1080-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f1080-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1080-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f1080-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f1080-106">Recupere uma lista de [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) no locatário/diretório.</span><span class="sxs-lookup"><span data-stu-id="f1080-106">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1080-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1080-107">Permissions</span></span>

<span data-ttu-id="f1080-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1080-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="f1080-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1080-110">Permission type</span></span>      | <span data-ttu-id="f1080-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1080-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1080-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1080-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1080-113">Policy. Read. TrustFramework, Policy. Read. All</span><span class="sxs-lookup"><span data-stu-id="f1080-113">Policy.Read.TrustFramework, Policy.Read.All</span></span>|
|<span data-ttu-id="f1080-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1080-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f1080-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1080-115">Not supported.</span></span>|
|<span data-ttu-id="f1080-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1080-116">Application</span></span>|<span data-ttu-id="f1080-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1080-117">Not supported.</span></span>|

<span data-ttu-id="f1080-118">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="f1080-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="f1080-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1080-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f1080-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1080-120">Optional query parameters</span></span>

<span data-ttu-id="f1080-121">Este método oferece suporte `$select` aos `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1080-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1080-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1080-122">Request headers</span></span>

|<span data-ttu-id="f1080-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f1080-123">Name</span></span>|<span data-ttu-id="f1080-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1080-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f1080-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1080-125">Authorization</span></span>|<span data-ttu-id="f1080-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1080-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1080-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1080-128">Request body</span></span>

<span data-ttu-id="f1080-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1080-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1080-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1080-130">Response</span></span>

<span data-ttu-id="f1080-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) em uma representação JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1080-131">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1080-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1080-132">Example</span></span>

<span data-ttu-id="f1080-133">O exemplo a seguir recupera todos os **trustFrameworkPolicies**.</span><span class="sxs-lookup"><span data-stu-id="f1080-133">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="f1080-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1080-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_trustFrameworks"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies
```

##### <a name="response"></a><span data-ttu-id="f1080-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1080-135">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f1080-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f1080-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f1080-137">Basic</span><span class="sxs-lookup"><span data-stu-id="f1080-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_trustFrameworks-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1080-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1080-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_trustFrameworks-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/trustframework-list-trustframeworkpolicies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/trustframework-list-trustframeworkpolicies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
