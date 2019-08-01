---
title: Listar ownedDevices
description: Obtenha a lista de dispositivos de propriedade do usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8edac4e161b27cf0016965944d5dcd6daf5e2565
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026800"
---
# <a name="list-owneddevices"></a><span data-ttu-id="08715-103">Listar ownedDevices</span><span class="sxs-lookup"><span data-stu-id="08715-103">List ownedDevices</span></span>

<span data-ttu-id="08715-104">Obtenha a lista de dispositivos de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="08715-104">Get the list of devices that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="08715-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="08715-105">Permissions</span></span>
<span data-ttu-id="08715-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08715-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08715-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08715-108">Permission type</span></span>      | <span data-ttu-id="08715-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08715-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08715-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08715-110">Delegated (work or school account)</span></span> | <span data-ttu-id="08715-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08715-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="08715-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08715-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08715-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08715-113">Not supported.</span></span>    |
|<span data-ttu-id="08715-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08715-114">Application</span></span> | <span data-ttu-id="08715-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08715-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08715-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08715-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="08715-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="08715-117">Optional query parameters</span></span>
<span data-ttu-id="08715-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="08715-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="08715-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08715-119">Request headers</span></span>
| <span data-ttu-id="08715-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="08715-120">Header</span></span>       | <span data-ttu-id="08715-121">Valor</span><span class="sxs-lookup"><span data-stu-id="08715-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="08715-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="08715-122">Authorization</span></span>  | <span data-ttu-id="08715-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08715-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="08715-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="08715-125">Accept</span></span>  | <span data-ttu-id="08715-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08715-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08715-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08715-127">Request body</span></span>
<span data-ttu-id="08715-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="08715-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08715-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="08715-129">Response</span></span>

<span data-ttu-id="08715-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08715-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="08715-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08715-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08715-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08715-132">Request</span></span>
<span data-ttu-id="08715-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08715-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="08715-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="08715-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_owneddevices"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/ownedDevices
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="08715-135">C#</span><span class="sxs-lookup"><span data-stu-id="08715-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-owneddevices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08715-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="08715-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-owneddevices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08715-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="08715-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-owneddevices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="08715-138">Java</span><span class="sxs-lookup"><span data-stu-id="08715-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-owneddevices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="08715-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="08715-139">Response</span></span>
<span data-ttu-id="08715-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08715-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
