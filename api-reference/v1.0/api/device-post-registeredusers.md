---
title: Criar registeredUser
description: Adiciona um usuário registrado ao dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 00adeaa417c538753121a322c7d6da634f680ade
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811855"
---
# <a name="create-registereduser"></a><span data-ttu-id="6f762-103">Criar registeredUser</span><span class="sxs-lookup"><span data-stu-id="6f762-103">Create registeredUser</span></span>

<span data-ttu-id="6f762-104">Adiciona um usuário registrado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f762-104">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f762-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f762-105">Permissions</span></span>
<span data-ttu-id="6f762-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f762-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6f762-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f762-108">Permission type</span></span>      | <span data-ttu-id="6f762-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f762-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f762-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f762-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6f762-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6f762-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6f762-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f762-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f762-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f762-113">Not supported.</span></span>    |
|<span data-ttu-id="6f762-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f762-114">Application</span></span> | <span data-ttu-id="6f762-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f762-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f762-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f762-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="6f762-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f762-117">Request headers</span></span>
| <span data-ttu-id="6f762-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6f762-118">Name</span></span>       | <span data-ttu-id="6f762-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f762-119">Type</span></span> | <span data-ttu-id="6f762-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f762-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6f762-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f762-121">Authorization</span></span>  | <span data-ttu-id="6f762-122">string</span><span class="sxs-lookup"><span data-stu-id="6f762-122">string</span></span>  | <span data-ttu-id="6f762-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f762-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f762-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f762-125">Request body</span></span>
<span data-ttu-id="6f762-126">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="6f762-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6f762-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f762-127">Response</span></span>

<span data-ttu-id="6f762-128">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f762-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f762-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f762-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f762-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f762-130">Request</span></span>
<span data-ttu-id="6f762-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f762-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="6f762-132">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="6f762-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6f762-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f762-133">Response</span></span>
<span data-ttu-id="6f762-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f762-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
