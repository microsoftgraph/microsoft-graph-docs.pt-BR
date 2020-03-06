---
title: Listar registeredOwners
description: Recupera uma lista de usuários que são proprietários registrados do dispositivo. Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal. O proprietário registrado é definido no momento do registro. Atualmente, só pode haver um proprietário.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bf56b72389ae3ffebde2dbf27af70f216107e10a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518116"
---
# <a name="list-registeredowners"></a><span data-ttu-id="afd4c-106">Listar registeredOwners</span><span class="sxs-lookup"><span data-stu-id="afd4c-106">List registeredOwners</span></span>

<span data-ttu-id="afd4c-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afd4c-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="afd4c-108">Recupera uma lista de usuários que são proprietários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="afd4c-108">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="afd4c-109">Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal.</span><span class="sxs-lookup"><span data-stu-id="afd4c-109">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="afd4c-110">O proprietário registrado é definido no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="afd4c-110">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="afd4c-111">Atualmente, só pode haver um proprietário.</span><span class="sxs-lookup"><span data-stu-id="afd4c-111">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="afd4c-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="afd4c-112">Permissions</span></span>
<span data-ttu-id="afd4c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afd4c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="afd4c-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afd4c-115">Permission type</span></span>      | <span data-ttu-id="afd4c-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="afd4c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afd4c-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afd4c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="afd4c-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="afd4c-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="afd4c-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afd4c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afd4c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afd4c-120">Not supported.</span></span>    |
|<span data-ttu-id="afd4c-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afd4c-121">Application</span></span> | <span data-ttu-id="afd4c-122">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afd4c-122">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="afd4c-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afd4c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="afd4c-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="afd4c-124">Optional query parameters</span></span>
<span data-ttu-id="afd4c-125">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="afd4c-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="afd4c-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afd4c-126">Request headers</span></span>
| <span data-ttu-id="afd4c-127">Nome</span><span class="sxs-lookup"><span data-stu-id="afd4c-127">Name</span></span>       | <span data-ttu-id="afd4c-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="afd4c-128">Type</span></span> | <span data-ttu-id="afd4c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="afd4c-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="afd4c-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="afd4c-130">Authorization</span></span>  | <span data-ttu-id="afd4c-131">string</span><span class="sxs-lookup"><span data-stu-id="afd4c-131">string</span></span>  | <span data-ttu-id="afd4c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afd4c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="afd4c-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afd4c-134">Request body</span></span>
<span data-ttu-id="afd4c-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="afd4c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afd4c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="afd4c-136">Response</span></span>

<span data-ttu-id="afd4c-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afd4c-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="afd4c-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afd4c-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="afd4c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afd4c-139">Request</span></span>
<span data-ttu-id="afd4c-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="afd4c-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="afd4c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="afd4c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
# <a name="c"></a>[<span data-ttu-id="afd4c-142">C#</span><span class="sxs-lookup"><span data-stu-id="afd4c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afd4c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afd4c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afd4c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afd4c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="afd4c-145">Java</span><span class="sxs-lookup"><span data-stu-id="afd4c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="afd4c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="afd4c-146">Response</span></span>
<span data-ttu-id="afd4c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afd4c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
