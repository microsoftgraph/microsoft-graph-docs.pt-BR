---
title: Listar registeredUsers
description: Recupera uma lista de usuários que são usuários registrados do dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 37b42c80f483fa8ccd2aeefb70f01ba46b4be349
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721338"
---
# <a name="list-registeredusers"></a><span data-ttu-id="9956a-103">Listar registeredUsers</span><span class="sxs-lookup"><span data-stu-id="9956a-103">List registeredUsers</span></span>

<span data-ttu-id="9956a-104">Recupera uma lista de usuários que são usuários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9956a-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="9956a-105">Para dispositivos associados em nuvem e dispositivos pessoais registrados, os usuários registrados são definidos para o mesmo valor que proprietários registrados no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="9956a-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="9956a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9956a-106">Permissions</span></span>
<span data-ttu-id="9956a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9956a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9956a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9956a-109">Permission type</span></span>      | <span data-ttu-id="9956a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9956a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9956a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9956a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9956a-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9956a-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9956a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9956a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9956a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9956a-114">Not supported.</span></span>    |
|<span data-ttu-id="9956a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9956a-115">Application</span></span> | <span data-ttu-id="9956a-116">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9956a-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9956a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9956a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9956a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9956a-118">Optional query parameters</span></span>
<span data-ttu-id="9956a-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9956a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9956a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9956a-120">Request headers</span></span>
| <span data-ttu-id="9956a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9956a-121">Name</span></span>       | <span data-ttu-id="9956a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9956a-122">Type</span></span> | <span data-ttu-id="9956a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9956a-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9956a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9956a-124">Authorization</span></span>  | <span data-ttu-id="9956a-125">string</span><span class="sxs-lookup"><span data-stu-id="9956a-125">string</span></span>  | <span data-ttu-id="9956a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9956a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9956a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9956a-128">Request body</span></span>
<span data-ttu-id="9956a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9956a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9956a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9956a-130">Response</span></span>

<span data-ttu-id="9956a-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9956a-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9956a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9956a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9956a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9956a-133">Request</span></span>
<span data-ttu-id="9956a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9956a-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9956a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9956a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9956a-136">C#</span><span class="sxs-lookup"><span data-stu-id="9956a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9956a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9956a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9956a-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9956a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9956a-139">Java</span><span class="sxs-lookup"><span data-stu-id="9956a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9956a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9956a-140">Response</span></span>
<span data-ttu-id="9956a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9956a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
