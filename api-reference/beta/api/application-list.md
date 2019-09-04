---
title: Listar aplicativos
description: Recupere a lista de aplicativos nesta organização.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1642eac11159ac016669ecb9b9c058c7eb4ca1de
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719028"
---
# <a name="list-applications"></a><span data-ttu-id="9b720-103">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="9b720-103">List applications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b720-104">Recupere a lista de aplicativos nesta organização.</span><span class="sxs-lookup"><span data-stu-id="9b720-104">Retrieve the list of applications in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b720-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b720-105">Permissions</span></span>
<span data-ttu-id="9b720-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b720-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9b720-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b720-108">Permission type</span></span>      | <span data-ttu-id="9b720-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b720-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b720-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b720-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9b720-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9b720-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9b720-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b720-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b720-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b720-113">Not supported.</span></span>    |
|<span data-ttu-id="9b720-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b720-114">Application</span></span> | <span data-ttu-id="9b720-115">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b720-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b720-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b720-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9b720-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9b720-117">Optional query parameters</span></span>
<span data-ttu-id="9b720-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9b720-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b720-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b720-119">Request headers</span></span>
| <span data-ttu-id="9b720-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9b720-120">Name</span></span>       | <span data-ttu-id="9b720-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b720-121">Type</span></span> | <span data-ttu-id="9b720-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b720-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9b720-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b720-123">Authorization</span></span>  | <span data-ttu-id="9b720-124">string</span><span class="sxs-lookup"><span data-stu-id="9b720-124">string</span></span>  | <span data-ttu-id="9b720-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b720-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9b720-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b720-127">Request body</span></span>
<span data-ttu-id="9b720-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b720-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b720-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b720-129">Response</span></span>

<span data-ttu-id="9b720-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b720-130">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9b720-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b720-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b720-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b720-132">Request</span></span>
<span data-ttu-id="9b720-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b720-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9b720-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b720-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9b720-135">C#</span><span class="sxs-lookup"><span data-stu-id="9b720-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b720-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b720-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9b720-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b720-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9b720-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b720-138">Response</span></span>
<span data-ttu-id="9b720-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b720-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1229

{
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
