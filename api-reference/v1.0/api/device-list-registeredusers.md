---
title: Listar registeredUsers
description: Recupera uma lista de usuários que são usuários registrados do dispositivo.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7aff307f93258bbeac1b620c3aa12a5983bb4d1c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035649"
---
# <a name="list-registeredusers"></a><span data-ttu-id="5d40a-103">Listar registeredUsers</span><span class="sxs-lookup"><span data-stu-id="5d40a-103">List registeredUsers</span></span>

<span data-ttu-id="5d40a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d40a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d40a-105">Recupera uma lista de usuários que são usuários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5d40a-105">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="5d40a-106">Para dispositivos associados em nuvem e dispositivos pessoais registrados, os usuários registrados são definidos para o mesmo valor que proprietários registrados no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="5d40a-106">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d40a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d40a-107">Permissions</span></span>
<span data-ttu-id="5d40a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d40a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d40a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d40a-110">Permission type</span></span>      | <span data-ttu-id="5d40a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d40a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d40a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d40a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5d40a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5d40a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5d40a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d40a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d40a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d40a-115">Not supported.</span></span>    |
|<span data-ttu-id="5d40a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d40a-116">Application</span></span> | <span data-ttu-id="5d40a-117">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d40a-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="5d40a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d40a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5d40a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5d40a-119">Optional query parameters</span></span>
<span data-ttu-id="5d40a-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5d40a-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5d40a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d40a-121">Request headers</span></span>
| <span data-ttu-id="5d40a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5d40a-122">Name</span></span>       | <span data-ttu-id="5d40a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d40a-123">Type</span></span> | <span data-ttu-id="5d40a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d40a-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5d40a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d40a-125">Authorization</span></span>  | <span data-ttu-id="5d40a-126">string</span><span class="sxs-lookup"><span data-stu-id="5d40a-126">string</span></span>  | <span data-ttu-id="5d40a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d40a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d40a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d40a-129">Request body</span></span>
<span data-ttu-id="5d40a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d40a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d40a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d40a-131">Response</span></span>

<span data-ttu-id="5d40a-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d40a-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d40a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d40a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d40a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d40a-134">Request</span></span>
<span data-ttu-id="5d40a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d40a-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d40a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d40a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
# <a name="c"></a>[<span data-ttu-id="5d40a-137">C#</span><span class="sxs-lookup"><span data-stu-id="5d40a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d40a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d40a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d40a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d40a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d40a-140">Java</span><span class="sxs-lookup"><span data-stu-id="5d40a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5d40a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d40a-141">Response</span></span>
<span data-ttu-id="5d40a-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d40a-142">Here is an example of the response.</span></span> <span data-ttu-id="5d40a-143">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5d40a-143">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
