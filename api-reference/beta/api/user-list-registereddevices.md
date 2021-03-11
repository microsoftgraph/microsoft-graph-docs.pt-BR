---
title: Listar registeredDevices
description: Obtenha a lista de dispositivos registrado do usuário.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: dde29d94209f29413cce5ddab5e67e89188803fb
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721502"
---
# <a name="list-registereddevices"></a><span data-ttu-id="28842-103">Listar registeredDevices</span><span class="sxs-lookup"><span data-stu-id="28842-103">List registeredDevices</span></span>

<span data-ttu-id="28842-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28842-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28842-105">Obtenha a lista de dispositivos registrado do usuário.</span><span class="sxs-lookup"><span data-stu-id="28842-105">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="28842-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="28842-106">Permissions</span></span>
<span data-ttu-id="28842-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28842-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28842-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28842-109">Permission type</span></span>      | <span data-ttu-id="28842-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28842-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28842-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28842-111">Delegated (work or school account)</span></span> | <span data-ttu-id="28842-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="28842-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="28842-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28842-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28842-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28842-114">Not supported.</span></span>    |
|<span data-ttu-id="28842-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28842-115">Application</span></span> | <span data-ttu-id="28842-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28842-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="28842-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28842-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="28842-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28842-118">Optional query parameters</span></span>
<span data-ttu-id="28842-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="28842-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="28842-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28842-120">Request headers</span></span>
| <span data-ttu-id="28842-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28842-121">Header</span></span>       | <span data-ttu-id="28842-122">Valor</span><span class="sxs-lookup"><span data-stu-id="28842-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="28842-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="28842-123">Authorization</span></span>  | <span data-ttu-id="28842-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28842-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="28842-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="28842-126">Accept</span></span>  | <span data-ttu-id="28842-127">application/json</span><span class="sxs-lookup"><span data-stu-id="28842-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28842-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28842-128">Request body</span></span>
<span data-ttu-id="28842-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28842-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28842-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="28842-130">Response</span></span>

<span data-ttu-id="28842-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28842-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="28842-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28842-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28842-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28842-133">Request</span></span>
<span data-ttu-id="28842-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28842-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28842-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="28842-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/registeredDevices
```
# <a name="c"></a>[<span data-ttu-id="28842-136">C#</span><span class="sxs-lookup"><span data-stu-id="28842-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registereddevices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28842-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28842-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registereddevices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28842-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28842-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registereddevices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28842-139">Java</span><span class="sxs-lookup"><span data-stu-id="28842-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registereddevices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28842-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="28842-140">Response</span></span>
<span data-ttu-id="28842-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28842-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List registeredDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
