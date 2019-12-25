---
title: Listar ownedDevices
description: Obtenha a lista de dispositivos de propriedade do usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1641bef934890ea74176965df0f6af7313951799
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870691"
---
# <a name="list-owneddevices"></a><span data-ttu-id="3dd21-103">Listar ownedDevices</span><span class="sxs-lookup"><span data-stu-id="3dd21-103">List ownedDevices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dd21-104">Obtenha a lista de dispositivos de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="3dd21-104">Get the list of devices that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="3dd21-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3dd21-105">Permissions</span></span>
<span data-ttu-id="3dd21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dd21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dd21-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3dd21-108">Permission type</span></span>      | <span data-ttu-id="3dd21-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3dd21-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3dd21-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3dd21-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3dd21-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3dd21-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3dd21-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3dd21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dd21-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dd21-113">Not supported.</span></span>    |
|<span data-ttu-id="3dd21-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3dd21-114">Application</span></span> | <span data-ttu-id="3dd21-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dd21-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="3dd21-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3dd21-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3dd21-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3dd21-117">Optional query parameters</span></span>
<span data-ttu-id="3dd21-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3dd21-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3dd21-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3dd21-119">Request headers</span></span>
| <span data-ttu-id="3dd21-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3dd21-120">Header</span></span>       | <span data-ttu-id="3dd21-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3dd21-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3dd21-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3dd21-122">Authorization</span></span>  | <span data-ttu-id="3dd21-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3dd21-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3dd21-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3dd21-125">Accept</span></span>  | <span data-ttu-id="3dd21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3dd21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dd21-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3dd21-127">Request body</span></span>
<span data-ttu-id="3dd21-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3dd21-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3dd21-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dd21-129">Response</span></span>

<span data-ttu-id="3dd21-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3dd21-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3dd21-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3dd21-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3dd21-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3dd21-132">Request</span></span>
<span data-ttu-id="3dd21-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3dd21-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3dd21-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dd21-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_owneddevices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/ownedDevices
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3dd21-135">C#</span><span class="sxs-lookup"><span data-stu-id="3dd21-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-owneddevices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3dd21-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dd21-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-owneddevices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3dd21-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dd21-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-owneddevices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3dd21-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dd21-138">Response</span></span>
<span data-ttu-id="3dd21-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3dd21-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List ownedDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
