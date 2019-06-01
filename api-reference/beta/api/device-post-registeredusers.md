---
title: Criar registeredUser
description: Adiciona um usuário registrado ao dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0508b0fad410d1edc09297e9e2a2f9c409dcf63c
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656227"
---
# <a name="create-registereduser"></a><span data-ttu-id="7f36e-103">Criar registeredUser</span><span class="sxs-lookup"><span data-stu-id="7f36e-103">Create registeredUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f36e-104">Adiciona um usuário registrado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7f36e-104">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f36e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f36e-105">Permissions</span></span>
<span data-ttu-id="7f36e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f36e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7f36e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f36e-108">Permission type</span></span>      | <span data-ttu-id="7f36e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f36e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f36e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f36e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7f36e-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7f36e-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7f36e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f36e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f36e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f36e-113">Not supported.</span></span>    |
|<span data-ttu-id="7f36e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f36e-114">Application</span></span> | <span data-ttu-id="7f36e-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f36e-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f36e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f36e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="7f36e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f36e-117">Request headers</span></span>
| <span data-ttu-id="7f36e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7f36e-118">Name</span></span>       | <span data-ttu-id="7f36e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f36e-119">Type</span></span> | <span data-ttu-id="7f36e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f36e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7f36e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f36e-121">Authorization</span></span>  | <span data-ttu-id="7f36e-122">string</span><span class="sxs-lookup"><span data-stu-id="7f36e-122">string</span></span>  | <span data-ttu-id="7f36e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f36e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f36e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f36e-125">Request body</span></span>
<span data-ttu-id="7f36e-126">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="7f36e-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7f36e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f36e-127">Response</span></span>

<span data-ttu-id="7f36e-128">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f36e-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f36e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f36e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f36e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f36e-130">Request</span></span>
<span data-ttu-id="7f36e-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f36e-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="7f36e-132">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="7f36e-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7f36e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f36e-133">Response</span></span>
<span data-ttu-id="7f36e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f36e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7f36e-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="7f36e-137">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f36e-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="7f36e-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_device-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/device-post-registeredusers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
