---
title: Listar Administrativeunits dos quais
description: Recupere uma lista de objetos administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8e48373cb2e26111e9ffe2fbd12213db0207396e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719154"
---
# <a name="list-administrativeunits"></a><span data-ttu-id="5b967-103">Listar Administrativeunits dos quais</span><span class="sxs-lookup"><span data-stu-id="5b967-103">List administrativeUnits</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b967-104">Recupere uma lista de objetos [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="5b967-104">Retrieve a list of [administrativeUnit](../resources/administrativeunit.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5b967-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b967-105">Permissions</span></span>
<span data-ttu-id="5b967-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b967-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5b967-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b967-108">Permission type</span></span>      | <span data-ttu-id="5b967-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b967-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b967-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b967-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5b967-111">AdministrativeUnit. Read. All, Directory. Read. All, AdministrativeUnit. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="5b967-111">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5b967-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b967-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b967-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b967-113">Not supported.</span></span>    |
|<span data-ttu-id="5b967-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b967-114">Application</span></span> | <span data-ttu-id="5b967-115">AdministrativeUnit. Read. All, Directory. Read. All, AdministrativeUnit. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5b967-115">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b967-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b967-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b967-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5b967-117">Optional query parameters</span></span>
<span data-ttu-id="5b967-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5b967-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b967-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b967-119">Request headers</span></span>
| <span data-ttu-id="5b967-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5b967-120">Name</span></span>      |<span data-ttu-id="5b967-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b967-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5b967-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b967-122">Authorization</span></span>  | <span data-ttu-id="5b967-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b967-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b967-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b967-125">Request body</span></span>
<span data-ttu-id="5b967-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b967-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b967-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b967-127">Response</span></span>

<span data-ttu-id="5b967-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b967-128">If successful, this method returns a `200 OK` response code and collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5b967-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b967-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b967-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b967-130">Request</span></span>
<span data-ttu-id="5b967-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b967-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5b967-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b967-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunits"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5b967-133">C#</span><span class="sxs-lookup"><span data-stu-id="5b967-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b967-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b967-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5b967-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5b967-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5b967-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b967-136">Response</span></span>
<span data-ttu-id="5b967-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b967-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "value": [
    {
      "displayName": "displayName-value",
      "description": "description-value",
      "visibility": "visibility-value",
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
  "description": "List administrativeUnits",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
