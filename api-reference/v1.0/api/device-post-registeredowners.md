---
title: Criar registeredOwner
description: Adiciona um usuário como proprietário registrado do dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 59b70c830308c8feedb672b9606a0c0489c2d27f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518081"
---
# <a name="create-registeredowner"></a><span data-ttu-id="2f5bf-103">Criar registeredOwner</span><span class="sxs-lookup"><span data-stu-id="2f5bf-103">Create registeredOwner</span></span>

<span data-ttu-id="2f5bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f5bf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2f5bf-105">Adiciona um usuário como proprietário registrado do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f5bf-105">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="2f5bf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f5bf-106">Permissions</span></span>
<span data-ttu-id="2f5bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f5bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2f5bf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f5bf-109">Permission type</span></span>      | <span data-ttu-id="2f5bf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f5bf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f5bf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f5bf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2f5bf-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2f5bf-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2f5bf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f5bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f5bf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f5bf-114">Not supported.</span></span>    |
|<span data-ttu-id="2f5bf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f5bf-115">Application</span></span> | <span data-ttu-id="2f5bf-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f5bf-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f5bf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f5bf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="2f5bf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f5bf-118">Request headers</span></span>
| <span data-ttu-id="2f5bf-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2f5bf-119">Name</span></span>       | <span data-ttu-id="2f5bf-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f5bf-120">Type</span></span> | <span data-ttu-id="2f5bf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f5bf-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2f5bf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f5bf-122">Authorization</span></span>  | <span data-ttu-id="2f5bf-123">string</span><span class="sxs-lookup"><span data-stu-id="2f5bf-123">string</span></span>  | <span data-ttu-id="2f5bf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f5bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f5bf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f5bf-126">Request body</span></span>
<span data-ttu-id="2f5bf-127">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="2f5bf-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2f5bf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f5bf-128">Response</span></span>

<span data-ttu-id="2f5bf-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f5bf-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f5bf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f5bf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f5bf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f5bf-131">Request</span></span>
<span data-ttu-id="2f5bf-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f5bf-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2f5bf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f5bf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="2f5bf-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f5bf-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2f5bf-135">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="2f5bf-135">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2f5bf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f5bf-136">Response</span></span>
<span data-ttu-id="2f5bf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f5bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
