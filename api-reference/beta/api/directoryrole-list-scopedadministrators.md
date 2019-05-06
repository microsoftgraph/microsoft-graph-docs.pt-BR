---
title: Listar scopedMembers para uma função de diretório
description: Recupere uma lista de objetos scopedRoleMembership para uma função de diretório.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5dd74a5e540693e64afa8ed4ce72b165c72e2b63
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590380"
---
# <a name="list-scopedmembers-for-a-directory-role"></a><span data-ttu-id="d2447-103">Listar scopedMembers para uma função de diretório</span><span class="sxs-lookup"><span data-stu-id="d2447-103">List scopedMembers for a directory role</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2447-104">Recupere uma lista de objetos [scopedRoleMembership](../resources/scopedrolemembership.md) para uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="d2447-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) objects for a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="d2447-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2447-105">Permissions</span></span>
<span data-ttu-id="d2447-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2447-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2447-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2447-108">Permission type</span></span>      | <span data-ttu-id="d2447-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2447-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2447-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2447-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2447-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d2447-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d2447-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2447-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2447-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2447-113">Not supported.</span></span>    |
|<span data-ttu-id="d2447-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2447-114">Application</span></span> | <span data-ttu-id="d2447-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2447-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2447-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2447-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryroles/{id}/scopedMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d2447-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d2447-117">Optional query parameters</span></span>
<span data-ttu-id="d2447-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d2447-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2447-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2447-119">Request headers</span></span>
| <span data-ttu-id="d2447-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d2447-120">Name</span></span>      |<span data-ttu-id="d2447-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2447-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2447-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2447-122">Authorization</span></span>  | <span data-ttu-id="d2447-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2447-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2447-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2447-125">Request body</span></span>
<span data-ttu-id="d2447-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2447-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2447-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2447-127">Response</span></span>

<span data-ttu-id="d2447-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2447-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2447-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2447-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2447-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2447-130">Request</span></span>
<span data-ttu-id="d2447-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2447-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/scopedMembers
```
##### <a name="response"></a><span data-ttu-id="d2447-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2447-132">Response</span></span>
<span data-ttu-id="d2447-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2447-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "id-value",
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d2447-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d2447-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d2447-137">Basic</span><span class="sxs-lookup"><span data-stu-id="d2447-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_scopedmembers_directoryrole-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2447-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2447-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_scopedmembers_directoryrole-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedmembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-list-scopedadministrators.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryrole-list-scopedadministrators.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
