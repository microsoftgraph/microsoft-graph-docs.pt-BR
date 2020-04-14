---
title: Criar registeredUser
description: Adiciona um usuário registrado ao dispositivo.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5ab9c4a526faa5aa7d5f899bcc3655dae74033c8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381740"
---
# <a name="create-registereduser"></a><span data-ttu-id="d3bac-103">Criar registeredUser</span><span class="sxs-lookup"><span data-stu-id="d3bac-103">Create registeredUser</span></span>

<span data-ttu-id="d3bac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3bac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3bac-105">Adiciona um usuário registrado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3bac-105">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3bac-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3bac-106">Permissions</span></span>
<span data-ttu-id="d3bac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3bac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d3bac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3bac-109">Permission type</span></span>      | <span data-ttu-id="d3bac-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3bac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3bac-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3bac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d3bac-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d3bac-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d3bac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3bac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3bac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3bac-114">Not supported.</span></span>    |
|<span data-ttu-id="d3bac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3bac-115">Application</span></span> | <span data-ttu-id="d3bac-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3bac-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3bac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3bac-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="d3bac-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3bac-118">Request headers</span></span>
| <span data-ttu-id="d3bac-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d3bac-119">Name</span></span>       | <span data-ttu-id="d3bac-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3bac-120">Type</span></span> | <span data-ttu-id="d3bac-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3bac-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d3bac-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3bac-122">Authorization</span></span>  | <span data-ttu-id="d3bac-123">string</span><span class="sxs-lookup"><span data-stu-id="d3bac-123">string</span></span>  | <span data-ttu-id="d3bac-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3bac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3bac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3bac-126">Request body</span></span>
<span data-ttu-id="d3bac-127">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="d3bac-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d3bac-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3bac-128">Response</span></span>

<span data-ttu-id="d3bac-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3bac-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3bac-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3bac-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3bac-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3bac-131">Request</span></span>
<span data-ttu-id="d3bac-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3bac-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3bac-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3bac-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredUsers/$ref
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="d3bac-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3bac-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d3bac-135">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="d3bac-135">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d3bac-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3bac-136">Response</span></span>
<span data-ttu-id="d3bac-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3bac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
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
