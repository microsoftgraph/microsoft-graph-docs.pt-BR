---
title: Listar ownedDevices
description: Obtenha a lista de dispositivos de propriedade do usuário.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ce6396a477d932889fc64661b078c3c94394ae8c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051169"
---
# <a name="list-owneddevices"></a><span data-ttu-id="4c6a4-103">Listar ownedDevices</span><span class="sxs-lookup"><span data-stu-id="4c6a4-103">List ownedDevices</span></span>

<span data-ttu-id="4c6a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c6a4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c6a4-105">Obtenha a lista de dispositivos de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="4c6a4-105">Get the list of devices that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="4c6a4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c6a4-106">Permissions</span></span>
<span data-ttu-id="4c6a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c6a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c6a4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c6a4-109">Permission type</span></span>      | <span data-ttu-id="4c6a4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c6a4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c6a4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c6a4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4c6a4-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4c6a4-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4c6a4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c6a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c6a4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c6a4-114">Not supported.</span></span>    |
|<span data-ttu-id="4c6a4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c6a4-115">Application</span></span> | <span data-ttu-id="4c6a4-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c6a4-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="4c6a4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c6a4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4c6a4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4c6a4-118">Optional query parameters</span></span>
<span data-ttu-id="4c6a4-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4c6a4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4c6a4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c6a4-120">Request headers</span></span>
| <span data-ttu-id="4c6a4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c6a4-121">Header</span></span>       | <span data-ttu-id="4c6a4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4c6a4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4c6a4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c6a4-123">Authorization</span></span>  | <span data-ttu-id="4c6a4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c6a4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4c6a4-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4c6a4-126">Accept</span></span>  | <span data-ttu-id="4c6a4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4c6a4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c6a4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c6a4-128">Request body</span></span>
<span data-ttu-id="4c6a4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c6a4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c6a4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c6a4-130">Response</span></span>

<span data-ttu-id="4c6a4-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c6a4-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c6a4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c6a4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c6a4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c6a4-133">Request</span></span>
<span data-ttu-id="4c6a4-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c6a4-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c6a4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c6a4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_owneddevices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/ownedDevices
```
# <a name="c"></a>[<span data-ttu-id="4c6a4-136">C#</span><span class="sxs-lookup"><span data-stu-id="4c6a4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-owneddevices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c6a4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c6a4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-owneddevices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c6a4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c6a4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-owneddevices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c6a4-139">Java</span><span class="sxs-lookup"><span data-stu-id="4c6a4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-owneddevices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4c6a4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c6a4-140">Response</span></span>
<span data-ttu-id="4c6a4-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c6a4-141">Here is an example of the response.</span></span> <span data-ttu-id="4c6a4-142">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4c6a4-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List ownedDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
