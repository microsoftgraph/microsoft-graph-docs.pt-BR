---
title: Listar registeredUsers
description: Recupera uma lista de usuários que são usuários registrados do dispositivo.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e679baba5dcdac47fb2a14d45555707afadddc7b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434549"
---
# <a name="list-registeredusers"></a><span data-ttu-id="c9c5f-103">Listar registeredUsers</span><span class="sxs-lookup"><span data-stu-id="c9c5f-103">List registeredUsers</span></span>

<span data-ttu-id="c9c5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9c5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c9c5f-105">Recupera uma lista de usuários que são usuários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c9c5f-105">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="c9c5f-106">Para dispositivos associados em nuvem e dispositivos pessoais registrados, os usuários registrados são definidos para o mesmo valor que proprietários registrados no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="c9c5f-106">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9c5f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9c5f-107">Permissions</span></span>
<span data-ttu-id="c9c5f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9c5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9c5f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9c5f-110">Permission type</span></span>      | <span data-ttu-id="c9c5f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9c5f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9c5f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9c5f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c9c5f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c9c5f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c9c5f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9c5f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9c5f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9c5f-115">Not supported.</span></span>    |
|<span data-ttu-id="c9c5f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9c5f-116">Application</span></span> | <span data-ttu-id="c9c5f-117">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9c5f-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c9c5f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9c5f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c9c5f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c9c5f-119">Optional query parameters</span></span>
<span data-ttu-id="c9c5f-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c9c5f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c9c5f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9c5f-121">Request headers</span></span>
| <span data-ttu-id="c9c5f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c9c5f-122">Name</span></span>       | <span data-ttu-id="c9c5f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9c5f-123">Type</span></span> | <span data-ttu-id="c9c5f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9c5f-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c9c5f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9c5f-125">Authorization</span></span>  | <span data-ttu-id="c9c5f-126">string</span><span class="sxs-lookup"><span data-stu-id="c9c5f-126">string</span></span>  | <span data-ttu-id="c9c5f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9c5f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9c5f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9c5f-129">Request body</span></span>
<span data-ttu-id="c9c5f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9c5f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9c5f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9c5f-131">Response</span></span>

<span data-ttu-id="c9c5f-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9c5f-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c9c5f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9c5f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9c5f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9c5f-134">Request</span></span>
<span data-ttu-id="c9c5f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9c5f-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c9c5f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9c5f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
# <a name="c"></a>[<span data-ttu-id="c9c5f-137">C#</span><span class="sxs-lookup"><span data-stu-id="c9c5f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9c5f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9c5f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9c5f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9c5f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9c5f-140">Java</span><span class="sxs-lookup"><span data-stu-id="c9c5f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c9c5f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9c5f-141">Response</span></span>
<span data-ttu-id="c9c5f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9c5f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
