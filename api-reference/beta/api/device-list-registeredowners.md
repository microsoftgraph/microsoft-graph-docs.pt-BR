---
title: Listar registeredOwners
description: Recupera uma lista de usuários que são proprietários registrados do dispositivo. Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal. O proprietário registrado é definido no momento do registro. Atualmente, só pode haver um proprietário.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9efc543911d2549573abd454ef0c99e9e637f5d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435826"
---
# <a name="list-registeredowners"></a><span data-ttu-id="c98c2-106">Listar registeredOwners</span><span class="sxs-lookup"><span data-stu-id="c98c2-106">List registeredOwners</span></span>

<span data-ttu-id="c98c2-107">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c98c2-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c98c2-108">Recupera uma lista de usuários que são proprietários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c98c2-108">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="c98c2-109">Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal.</span><span class="sxs-lookup"><span data-stu-id="c98c2-109">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="c98c2-110">O proprietário registrado é definido no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="c98c2-110">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="c98c2-111">Atualmente, só pode haver um proprietário.</span><span class="sxs-lookup"><span data-stu-id="c98c2-111">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="c98c2-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="c98c2-112">Permissions</span></span>

<span data-ttu-id="c98c2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c98c2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c98c2-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c98c2-115">Permission type</span></span>      | <span data-ttu-id="c98c2-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c98c2-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c98c2-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c98c2-117">Delegated (work or school account)</span></span> | <span data-ttu-id="c98c2-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c98c2-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c98c2-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c98c2-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c98c2-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c98c2-120">Not supported.</span></span>    |
|<span data-ttu-id="c98c2-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c98c2-121">Application</span></span> | <span data-ttu-id="c98c2-122">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c98c2-122">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c98c2-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c98c2-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```

> <span data-ttu-id="c98c2-124">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="c98c2-124">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c98c2-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c98c2-125">Optional query parameters</span></span>
<span data-ttu-id="c98c2-126">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c98c2-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c98c2-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c98c2-127">Request headers</span></span>
| <span data-ttu-id="c98c2-128">Nome</span><span class="sxs-lookup"><span data-stu-id="c98c2-128">Name</span></span>       | <span data-ttu-id="c98c2-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c98c2-129">Type</span></span> | <span data-ttu-id="c98c2-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c98c2-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c98c2-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="c98c2-131">Authorization</span></span>  | <span data-ttu-id="c98c2-132">string</span><span class="sxs-lookup"><span data-stu-id="c98c2-132">string</span></span>  | <span data-ttu-id="c98c2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c98c2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c98c2-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c98c2-135">Request body</span></span>
<span data-ttu-id="c98c2-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c98c2-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c98c2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c98c2-137">Response</span></span>

<span data-ttu-id="c98c2-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c98c2-138">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c98c2-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c98c2-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c98c2-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c98c2-140">Request</span></span>
<span data-ttu-id="c98c2-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c98c2-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c98c2-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="c98c2-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/registeredOwners
```
# <a name="c"></a>[<span data-ttu-id="c98c2-143">C#</span><span class="sxs-lookup"><span data-stu-id="c98c2-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c98c2-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c98c2-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c98c2-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c98c2-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c98c2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c98c2-146">Response</span></span>
<span data-ttu-id="c98c2-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c98c2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
