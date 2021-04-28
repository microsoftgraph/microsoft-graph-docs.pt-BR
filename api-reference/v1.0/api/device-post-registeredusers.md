---
title: Criar registeredUser
description: Adiciona um usuário registrado ao dispositivo.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 29a2314eb53d1ff1e79ef2375d8f887434809a6e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053213"
---
# <a name="create-registereduser"></a><span data-ttu-id="83a03-103">Criar registeredUser</span><span class="sxs-lookup"><span data-stu-id="83a03-103">Create registeredUser</span></span>

<span data-ttu-id="83a03-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83a03-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83a03-105">Adiciona um usuário registrado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83a03-105">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="83a03-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="83a03-106">Permissions</span></span>
<span data-ttu-id="83a03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83a03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="83a03-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83a03-109">Permission type</span></span>      | <span data-ttu-id="83a03-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83a03-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83a03-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83a03-111">Delegated (work or school account)</span></span> | <span data-ttu-id="83a03-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="83a03-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="83a03-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83a03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83a03-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83a03-114">Not supported.</span></span>    |
|<span data-ttu-id="83a03-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83a03-115">Application</span></span> | <span data-ttu-id="83a03-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83a03-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83a03-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83a03-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="83a03-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83a03-118">Request headers</span></span>
| <span data-ttu-id="83a03-119">Nome</span><span class="sxs-lookup"><span data-stu-id="83a03-119">Name</span></span>       | <span data-ttu-id="83a03-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="83a03-120">Type</span></span> | <span data-ttu-id="83a03-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="83a03-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="83a03-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="83a03-122">Authorization</span></span>  | <span data-ttu-id="83a03-123">string</span><span class="sxs-lookup"><span data-stu-id="83a03-123">string</span></span>  | <span data-ttu-id="83a03-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83a03-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83a03-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83a03-126">Request body</span></span>
<span data-ttu-id="83a03-127">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="83a03-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="83a03-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="83a03-128">Response</span></span>

<span data-ttu-id="83a03-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="83a03-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="83a03-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83a03-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83a03-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83a03-131">Request</span></span>
<span data-ttu-id="83a03-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83a03-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="83a03-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="83a03-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="83a03-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83a03-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="83a03-135">C#</span><span class="sxs-lookup"><span data-stu-id="83a03-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-device-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83a03-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83a03-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-device-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="83a03-137">Java</span><span class="sxs-lookup"><span data-stu-id="83a03-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-device-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="83a03-138">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="83a03-138">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="83a03-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="83a03-139">Response</span></span>
<span data-ttu-id="83a03-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83a03-140">Here is an example of the response.</span></span> <span data-ttu-id="83a03-141">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="83a03-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

