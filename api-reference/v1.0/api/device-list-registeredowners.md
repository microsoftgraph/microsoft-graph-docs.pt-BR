---
title: Listar registeredOwners
description: Recupera uma lista de usuários que são proprietários registrados do dispositivo.
localization_priority: Normal
author: spunukol
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0f9abc53e3e76d8fe8eba2aab666a9b77e79a75e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055166"
---
# <a name="list-registeredowners"></a><span data-ttu-id="3f31b-103">Listar registeredOwners</span><span class="sxs-lookup"><span data-stu-id="3f31b-103">List registeredOwners</span></span>

<span data-ttu-id="3f31b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f31b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3f31b-105">Recupera uma lista de usuários que são proprietários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3f31b-105">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="3f31b-106">Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal.</span><span class="sxs-lookup"><span data-stu-id="3f31b-106">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="3f31b-107">O proprietário registrado é definido no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="3f31b-107">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="3f31b-108">Atualmente, só pode haver um proprietário.</span><span class="sxs-lookup"><span data-stu-id="3f31b-108">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f31b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f31b-109">Permissions</span></span>
<span data-ttu-id="3f31b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f31b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3f31b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f31b-112">Permission type</span></span>      | <span data-ttu-id="3f31b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3f31b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f31b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f31b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3f31b-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3f31b-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3f31b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f31b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f31b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f31b-117">Not supported.</span></span>    |
|<span data-ttu-id="3f31b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f31b-118">Application</span></span> | <span data-ttu-id="3f31b-119">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f31b-119">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="3f31b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f31b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3f31b-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3f31b-121">Optional query parameters</span></span>
<span data-ttu-id="3f31b-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3f31b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3f31b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f31b-123">Request headers</span></span>
| <span data-ttu-id="3f31b-124">Nome</span><span class="sxs-lookup"><span data-stu-id="3f31b-124">Name</span></span>       | <span data-ttu-id="3f31b-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f31b-125">Type</span></span> | <span data-ttu-id="3f31b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f31b-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3f31b-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f31b-127">Authorization</span></span>  | <span data-ttu-id="3f31b-128">string</span><span class="sxs-lookup"><span data-stu-id="3f31b-128">string</span></span>  | <span data-ttu-id="3f31b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f31b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f31b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f31b-131">Request body</span></span>
<span data-ttu-id="3f31b-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3f31b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f31b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f31b-133">Response</span></span>

<span data-ttu-id="3f31b-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f31b-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3f31b-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f31b-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f31b-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f31b-136">Request</span></span>
<span data-ttu-id="3f31b-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f31b-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3f31b-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f31b-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
# <a name="c"></a>[<span data-ttu-id="3f31b-139">C#</span><span class="sxs-lookup"><span data-stu-id="3f31b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f31b-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f31b-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f31b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f31b-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f31b-142">Java</span><span class="sxs-lookup"><span data-stu-id="3f31b-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3f31b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f31b-143">Response</span></span>
<span data-ttu-id="3f31b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f31b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

