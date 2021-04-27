---
title: Listar administrativeUnits
description: Recupere uma lista de objetos administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 23d14eb80600309ccb237eaf87a0754ef1c2ea69
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048243"
---
# <a name="list-administrativeunits"></a><span data-ttu-id="c5080-103">Listar administrativeUnits</span><span class="sxs-lookup"><span data-stu-id="c5080-103">List administrativeUnits</span></span>

<span data-ttu-id="c5080-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5080-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5080-105">Recupere uma lista de [objetos administrativeUnit.](../resources/administrativeunit.md)</span><span class="sxs-lookup"><span data-stu-id="c5080-105">Retrieve a list of [administrativeUnit](../resources/administrativeunit.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5080-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5080-106">Permissions</span></span>
<span data-ttu-id="c5080-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5080-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c5080-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5080-109">Permission type</span></span>      | <span data-ttu-id="c5080-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5080-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5080-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5080-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c5080-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5080-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c5080-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5080-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5080-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5080-114">Not supported.</span></span>    |
|<span data-ttu-id="c5080-115">Application</span><span class="sxs-lookup"><span data-stu-id="c5080-115">Application</span></span> | <span data-ttu-id="c5080-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5080-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5080-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5080-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5080-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5080-118">Optional query parameters</span></span>
<span data-ttu-id="c5080-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5080-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5080-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5080-120">Request headers</span></span>
| <span data-ttu-id="c5080-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c5080-121">Name</span></span>      |<span data-ttu-id="c5080-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5080-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c5080-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5080-123">Authorization</span></span>  | <span data-ttu-id="c5080-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5080-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5080-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5080-126">Request body</span></span>
<span data-ttu-id="c5080-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5080-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5080-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5080-128">Response</span></span>

<span data-ttu-id="c5080-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5080-129">If successful, this method returns a `200 OK` response code and collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5080-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5080-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5080-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5080-131">Request</span></span>
<span data-ttu-id="c5080-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5080-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5080-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5080-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunits"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits
```
# <a name="c"></a>[<span data-ttu-id="c5080-134">C#</span><span class="sxs-lookup"><span data-stu-id="c5080-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5080-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5080-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5080-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5080-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5080-137">Java</span><span class="sxs-lookup"><span data-stu-id="c5080-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-administrativeunits-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c5080-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5080-138">Response</span></span>
<span data-ttu-id="c5080-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5080-139">Here is an example of the response.</span></span> <span data-ttu-id="c5080-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c5080-140">Note: The response object shown here might be shortened for readability.</span></span>
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
