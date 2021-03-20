---
title: Criar registeredUser
description: Adiciona um usuário registrado ao dispositivo.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b2b395f3953cec4299431289b5fc79502264114c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946702"
---
# <a name="create-registereduser"></a><span data-ttu-id="60a4b-103">Criar registeredUser</span><span class="sxs-lookup"><span data-stu-id="60a4b-103">Create registeredUser</span></span>

<span data-ttu-id="60a4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60a4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60a4b-105">Adiciona um usuário registrado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="60a4b-105">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="60a4b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="60a4b-106">Permissions</span></span>
<span data-ttu-id="60a4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60a4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="60a4b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60a4b-109">Permission type</span></span>      | <span data-ttu-id="60a4b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60a4b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60a4b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60a4b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="60a4b-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="60a4b-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="60a4b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60a4b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60a4b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60a4b-114">Not supported.</span></span>    |
|<span data-ttu-id="60a4b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60a4b-115">Application</span></span> | <span data-ttu-id="60a4b-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60a4b-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60a4b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60a4b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="60a4b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60a4b-118">Request headers</span></span>
| <span data-ttu-id="60a4b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="60a4b-119">Name</span></span>       | <span data-ttu-id="60a4b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="60a4b-120">Type</span></span> | <span data-ttu-id="60a4b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="60a4b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="60a4b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="60a4b-122">Authorization</span></span>  | <span data-ttu-id="60a4b-123">string</span><span class="sxs-lookup"><span data-stu-id="60a4b-123">string</span></span>  | <span data-ttu-id="60a4b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60a4b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60a4b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60a4b-126">Request body</span></span>
<span data-ttu-id="60a4b-127">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="60a4b-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="60a4b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="60a4b-128">Response</span></span>

<span data-ttu-id="60a4b-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="60a4b-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="60a4b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60a4b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60a4b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60a4b-131">Request</span></span>
<span data-ttu-id="60a4b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60a4b-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="60a4b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="60a4b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device_2"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredUsers/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="60a4b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60a4b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="60a4b-135">C#</span><span class="sxs-lookup"><span data-stu-id="60a4b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-device-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60a4b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60a4b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-device-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60a4b-137">Java</span><span class="sxs-lookup"><span data-stu-id="60a4b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-device-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="60a4b-138">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="60a4b-138">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="60a4b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="60a4b-139">Response</span></span>
<span data-ttu-id="60a4b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60a4b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


