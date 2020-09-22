---
title: Criar registeredOwner
description: Adiciona um usuário como proprietário registrado do dispositivo.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 20c742c6a474917cace63576d715fc972b75057f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996175"
---
# <a name="create-registeredowner"></a><span data-ttu-id="e0586-103">Criar registeredOwner</span><span class="sxs-lookup"><span data-stu-id="e0586-103">Create registeredOwner</span></span>

<span data-ttu-id="e0586-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0586-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0586-105">Adiciona um usuário como proprietário registrado do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0586-105">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0586-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0586-106">Permissions</span></span>
<span data-ttu-id="e0586-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0586-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e0586-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0586-109">Permission type</span></span>      | <span data-ttu-id="e0586-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0586-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0586-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0586-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e0586-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e0586-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e0586-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0586-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0586-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0586-114">Not supported.</span></span>    |
|<span data-ttu-id="e0586-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0586-115">Application</span></span> | <span data-ttu-id="e0586-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0586-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0586-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0586-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="e0586-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0586-118">Request headers</span></span>
| <span data-ttu-id="e0586-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e0586-119">Name</span></span>       | <span data-ttu-id="e0586-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0586-120">Type</span></span> | <span data-ttu-id="e0586-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0586-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e0586-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0586-122">Authorization</span></span>  | <span data-ttu-id="e0586-123">string</span><span class="sxs-lookup"><span data-stu-id="e0586-123">string</span></span>  | <span data-ttu-id="e0586-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0586-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0586-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0586-126">Request body</span></span>
<span data-ttu-id="e0586-127">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="e0586-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e0586-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0586-128">Response</span></span>

<span data-ttu-id="e0586-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e0586-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e0586-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0586-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0586-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0586-131">Request</span></span>
<span data-ttu-id="e0586-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0586-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0586-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0586-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredOwners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="e0586-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0586-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="e0586-135">C#</span><span class="sxs-lookup"><span data-stu-id="e0586-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0586-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0586-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e0586-137">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="e0586-137">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e0586-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0586-138">Response</span></span>
<span data-ttu-id="e0586-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0586-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


