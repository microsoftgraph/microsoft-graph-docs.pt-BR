---
title: Listar registeredOwners
description: Recupera uma lista de usuários que são proprietários registrados do dispositivo. Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal. O proprietário registrado é definido no momento do registro. Atualmente, só pode haver um proprietário.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 165ca84b2d081e971311ffa16b1bed5cf620cb17
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883432"
---
# <a name="list-registeredowners"></a><span data-ttu-id="6047b-106">Listar registeredOwners</span><span class="sxs-lookup"><span data-stu-id="6047b-106">List registeredOwners</span></span>

<span data-ttu-id="6047b-107">Recupera uma lista de usuários que são proprietários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6047b-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="6047b-108">Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal.</span><span class="sxs-lookup"><span data-stu-id="6047b-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="6047b-109">O proprietário registrado é definido no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="6047b-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="6047b-110">Atualmente, só pode haver um proprietário.</span><span class="sxs-lookup"><span data-stu-id="6047b-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="6047b-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="6047b-111">Permissions</span></span>
<span data-ttu-id="6047b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6047b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6047b-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6047b-114">Permission type</span></span>      | <span data-ttu-id="6047b-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6047b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6047b-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6047b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="6047b-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6047b-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6047b-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6047b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6047b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6047b-119">Not supported.</span></span>    |
|<span data-ttu-id="6047b-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6047b-120">Application</span></span> | <span data-ttu-id="6047b-121">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6047b-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6047b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6047b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6047b-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6047b-123">Optional query parameters</span></span>
<span data-ttu-id="6047b-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6047b-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6047b-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6047b-125">Request headers</span></span>
| <span data-ttu-id="6047b-126">Nome</span><span class="sxs-lookup"><span data-stu-id="6047b-126">Name</span></span>       | <span data-ttu-id="6047b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6047b-127">Type</span></span> | <span data-ttu-id="6047b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6047b-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6047b-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="6047b-129">Authorization</span></span>  | <span data-ttu-id="6047b-130">string</span><span class="sxs-lookup"><span data-stu-id="6047b-130">string</span></span>  | <span data-ttu-id="6047b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6047b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6047b-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6047b-133">Request body</span></span>
<span data-ttu-id="6047b-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6047b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6047b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6047b-135">Response</span></span>

<span data-ttu-id="6047b-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6047b-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6047b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6047b-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6047b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6047b-138">Request</span></span>
<span data-ttu-id="6047b-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6047b-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6047b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="6047b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6047b-141">C#</span><span class="sxs-lookup"><span data-stu-id="6047b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6047b-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="6047b-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6047b-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6047b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6047b-144">Java</span><span class="sxs-lookup"><span data-stu-id="6047b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6047b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6047b-145">Response</span></span>
<span data-ttu-id="6047b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6047b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
