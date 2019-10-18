---
title: Obter um servicePrincipal
description: Recuperar as propriedades e as relações do objeto serviceprincipal.
localization_priority: Priority
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: db48b38404de7e6b1cdfa2c7ddce89e33d6c935e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722458"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="f9ce8-103">Obter um servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="f9ce8-103">Get servicePrincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9ce8-104">Recuperar as propriedades e as relações do objeto serviceprincipal.</span><span class="sxs-lookup"><span data-stu-id="f9ce8-104">Retrieve the properties and relationships of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9ce8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9ce8-105">Permissions</span></span>
<span data-ttu-id="f9ce8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9ce8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f9ce8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9ce8-108">Permission type</span></span>      | <span data-ttu-id="f9ce8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9ce8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9ce8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9ce8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f9ce8-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f9ce8-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f9ce8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9ce8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9ce8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9ce8-113">Not supported.</span></span>    |
|<span data-ttu-id="f9ce8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9ce8-114">Application</span></span> | <span data-ttu-id="f9ce8-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9ce8-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9ce8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9ce8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9ce8-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f9ce8-117">Optional query parameters</span></span>
<span data-ttu-id="f9ce8-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f9ce8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9ce8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ce8-119">Request headers</span></span>
| <span data-ttu-id="f9ce8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f9ce8-120">Name</span></span>       | <span data-ttu-id="f9ce8-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9ce8-121">Type</span></span> | <span data-ttu-id="f9ce8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9ce8-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f9ce8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9ce8-123">Authorization</span></span>  | <span data-ttu-id="f9ce8-124">string</span><span class="sxs-lookup"><span data-stu-id="f9ce8-124">string</span></span>  | <span data-ttu-id="f9ce8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9ce8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9ce8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ce8-127">Request body</span></span>
<span data-ttu-id="f9ce8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9ce8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9ce8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9ce8-129">Response</span></span>

<span data-ttu-id="f9ce8-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9ce8-130">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9ce8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9ce8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9ce8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ce8-132">Request</span></span>
<span data-ttu-id="f9ce8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9ce8-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f9ce8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9ce8-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f9ce8-135">C#</span><span class="sxs-lookup"><span data-stu-id="f9ce8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9ce8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9ce8-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9ce8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9ce8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f9ce8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9ce8-138">Response</span></span>
<span data-ttu-id="f9ce8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9ce8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
