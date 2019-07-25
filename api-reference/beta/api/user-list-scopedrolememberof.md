---
title: Listar scopedAdministratorOf
description: Recupere uma lista de scopedRoleMembership para o usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 80c74905a8fb98bc34dc317766647b1ec170f760
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867073"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="1759c-103">Listar scopedAdministratorOf</span><span class="sxs-lookup"><span data-stu-id="1759c-103">List scopedAdministratorOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1759c-104">Recupere uma lista de [scopedRoleMembership](../resources/scopedrolemembership.md) para o usuário.</span><span class="sxs-lookup"><span data-stu-id="1759c-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="1759c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1759c-105">Permissions</span></span>
<span data-ttu-id="1759c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1759c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1759c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1759c-108">Permission type</span></span>      | <span data-ttu-id="1759c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1759c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1759c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1759c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1759c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1759c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1759c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1759c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1759c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1759c-113">Not supported.</span></span>    |
|<span data-ttu-id="1759c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1759c-114">Application</span></span> | <span data-ttu-id="1759c-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1759c-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1759c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1759c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedAdministratorOf
GET /users/{id}/scopedAdministratorOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="1759c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1759c-117">Optional query parameters</span></span>
<span data-ttu-id="1759c-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1759c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1759c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1759c-119">Request headers</span></span>
| <span data-ttu-id="1759c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1759c-120">Header</span></span>       | <span data-ttu-id="1759c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1759c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1759c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1759c-122">Authorization</span></span>  | <span data-ttu-id="1759c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1759c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1759c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1759c-125">Request body</span></span>
<span data-ttu-id="1759c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1759c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1759c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1759c-127">Response</span></span>

<span data-ttu-id="1759c-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1759c-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1759c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1759c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1759c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1759c-130">Request</span></span>
<span data-ttu-id="1759c-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1759c-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1759c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1759c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```http
GET https://graph.microsoft.com/beta/me/scopedAdministratorOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1759c-133">C#</span><span class="sxs-lookup"><span data-stu-id="1759c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedadministratorof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1759c-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="1759c-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedadministratorof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1759c-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1759c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedadministratorof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1759c-136">Java</span><span class="sxs-lookup"><span data-stu-id="1759c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedadministratorof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1759c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1759c-137">Response</span></span>
<span data-ttu-id="1759c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1759c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
