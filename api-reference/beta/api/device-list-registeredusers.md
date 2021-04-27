---
title: Listar registeredUsers
description: Recupera uma lista de usuários que são usuários registrados do dispositivo.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d755ec55d997df6aff2a3927951138553d72d1ce
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046962"
---
# <a name="list-registeredusers"></a><span data-ttu-id="1d74f-103">Listar registeredUsers</span><span class="sxs-lookup"><span data-stu-id="1d74f-103">List registeredUsers</span></span>

<span data-ttu-id="1d74f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d74f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d74f-105">Recupera uma lista de usuários que são usuários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1d74f-105">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="1d74f-106">Para dispositivos associados em nuvem e dispositivos pessoais registrados, os usuários registrados são definidos para o mesmo valor que proprietários registrados no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="1d74f-106">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d74f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d74f-107">Permissions</span></span>
<span data-ttu-id="1d74f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d74f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d74f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d74f-110">Permission type</span></span>      | <span data-ttu-id="1d74f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d74f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d74f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d74f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1d74f-113">Directory.Read.All ou Directory.ReadWrite.All ou Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d74f-113">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d74f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d74f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d74f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d74f-115">Not supported.</span></span> |
|<span data-ttu-id="1d74f-116">Application</span><span class="sxs-lookup"><span data-stu-id="1d74f-116">Application</span></span> | <span data-ttu-id="1d74f-117">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d74f-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="1d74f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d74f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="1d74f-119">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="1d74f-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="1d74f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1d74f-120">Optional query parameters</span></span>
<span data-ttu-id="1d74f-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1d74f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1d74f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d74f-122">Request headers</span></span>
| <span data-ttu-id="1d74f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1d74f-123">Name</span></span>       | <span data-ttu-id="1d74f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d74f-124">Type</span></span> | <span data-ttu-id="1d74f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d74f-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1d74f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d74f-126">Authorization</span></span>  | <span data-ttu-id="1d74f-127">string</span><span class="sxs-lookup"><span data-stu-id="1d74f-127">string</span></span>  | <span data-ttu-id="1d74f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d74f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d74f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d74f-130">Request body</span></span>
<span data-ttu-id="1d74f-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1d74f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d74f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d74f-132">Response</span></span>

<span data-ttu-id="1d74f-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d74f-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d74f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d74f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d74f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d74f-135">Request</span></span>
<span data-ttu-id="1d74f-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d74f-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d74f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d74f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
# <a name="c"></a>[<span data-ttu-id="1d74f-138">C#</span><span class="sxs-lookup"><span data-stu-id="1d74f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d74f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d74f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d74f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d74f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d74f-141">Java</span><span class="sxs-lookup"><span data-stu-id="1d74f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1d74f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d74f-142">Response</span></span>
<span data-ttu-id="1d74f-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d74f-143">Here is an example of the response.</span></span> <span data-ttu-id="1d74f-144">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1d74f-144">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
