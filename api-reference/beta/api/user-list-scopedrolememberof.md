---
title: Listar scopedAdministratorOf
description: Recupere uma lista de scopedRoleMembership para o usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 06c3a59cb8bb10f518df4420e1aff380dec64eb5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270025"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="3575c-103">Listar scopedAdministratorOf</span><span class="sxs-lookup"><span data-stu-id="3575c-103">List scopedAdministratorOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3575c-104">Recupere uma lista de [scopedRoleMembership](../resources/scopedrolemembership.md) para o usuário.</span><span class="sxs-lookup"><span data-stu-id="3575c-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="3575c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3575c-105">Permissions</span></span>
<span data-ttu-id="3575c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3575c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3575c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3575c-108">Permission type</span></span>      | <span data-ttu-id="3575c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3575c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3575c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3575c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3575c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3575c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3575c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3575c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3575c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3575c-113">Not supported.</span></span>    |
|<span data-ttu-id="3575c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3575c-114">Application</span></span> | <span data-ttu-id="3575c-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3575c-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3575c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3575c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedAdministratorOf
GET /users/{id}/scopedAdministratorOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="3575c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3575c-117">Optional query parameters</span></span>
<span data-ttu-id="3575c-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3575c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3575c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3575c-119">Request headers</span></span>
| <span data-ttu-id="3575c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3575c-120">Header</span></span>       | <span data-ttu-id="3575c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3575c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3575c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3575c-122">Authorization</span></span>  | <span data-ttu-id="3575c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3575c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3575c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3575c-125">Request body</span></span>
<span data-ttu-id="3575c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3575c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3575c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3575c-127">Response</span></span>

<span data-ttu-id="3575c-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3575c-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3575c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3575c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3575c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3575c-130">Request</span></span>
<span data-ttu-id="3575c-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3575c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```http
GET https://graph.microsoft.com/beta/me/scopedAdministratorOf
```
##### <a name="response"></a><span data-ttu-id="3575c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3575c-132">Response</span></span>
<span data-ttu-id="3575c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3575c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      },
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3575c-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3575c-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3575c-137">C#</span><span class="sxs-lookup"><span data-stu-id="3575c-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_scopedadministratorof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3575c-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="3575c-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_scopedadministratorof-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3575c-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3575c-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_scopedadministratorof-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedAdministratorOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-scopedrolememberof.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-scopedrolememberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-scopedrolememberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
