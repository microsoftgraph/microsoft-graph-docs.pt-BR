---
title: Criar registeredUser
description: Adiciona um usuário registrado ao dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 040974c2bc7ed29217e7a78cab5ff257fbb35752
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951320"
---
# <a name="create-registereduser"></a><span data-ttu-id="71f97-103">Criar registeredUser</span><span class="sxs-lookup"><span data-stu-id="71f97-103">Create registeredUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71f97-104">Adiciona um usuário registrado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="71f97-104">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="71f97-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="71f97-105">Permissions</span></span>
<span data-ttu-id="71f97-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71f97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="71f97-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71f97-108">Permission type</span></span>      | <span data-ttu-id="71f97-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71f97-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71f97-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71f97-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71f97-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="71f97-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="71f97-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71f97-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71f97-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71f97-113">Not supported.</span></span>    |
|<span data-ttu-id="71f97-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71f97-114">Application</span></span> | <span data-ttu-id="71f97-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71f97-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71f97-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71f97-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="71f97-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71f97-117">Request headers</span></span>
| <span data-ttu-id="71f97-118">Nome</span><span class="sxs-lookup"><span data-stu-id="71f97-118">Name</span></span>       | <span data-ttu-id="71f97-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="71f97-119">Type</span></span> | <span data-ttu-id="71f97-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="71f97-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="71f97-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="71f97-121">Authorization</span></span>  | <span data-ttu-id="71f97-122">string</span><span class="sxs-lookup"><span data-stu-id="71f97-122">string</span></span>  | <span data-ttu-id="71f97-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71f97-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71f97-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71f97-125">Request body</span></span>
<span data-ttu-id="71f97-126">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="71f97-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="71f97-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="71f97-127">Response</span></span>

<span data-ttu-id="71f97-128">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71f97-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71f97-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71f97-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71f97-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71f97-130">Request</span></span>
<span data-ttu-id="71f97-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71f97-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="71f97-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="71f97-132">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71f97-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="71f97-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="71f97-134">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="71f97-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="71f97-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="71f97-135">Response</span></span>
<span data-ttu-id="71f97-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71f97-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
