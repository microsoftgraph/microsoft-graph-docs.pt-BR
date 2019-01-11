---
title: Criar registeredOwner
description: Adiciona um usuário como proprietário registrado do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 295c48c586a6ddf31b1ceef15b9f1137227ba3ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820521"
---
# <a name="create-registeredowner"></a><span data-ttu-id="84c5a-103">Criar registeredOwner</span><span class="sxs-lookup"><span data-stu-id="84c5a-103">Create registeredOwner</span></span>

<span data-ttu-id="84c5a-104">Adiciona um usuário como proprietário registrado do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84c5a-104">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="84c5a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="84c5a-105">Permissions</span></span>
<span data-ttu-id="84c5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84c5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="84c5a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84c5a-108">Permission type</span></span>      | <span data-ttu-id="84c5a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84c5a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84c5a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84c5a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="84c5a-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="84c5a-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="84c5a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84c5a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84c5a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84c5a-113">Not supported.</span></span>    |
|<span data-ttu-id="84c5a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84c5a-114">Application</span></span> | <span data-ttu-id="84c5a-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84c5a-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84c5a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84c5a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="84c5a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84c5a-117">Request headers</span></span>
| <span data-ttu-id="84c5a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="84c5a-118">Name</span></span>       | <span data-ttu-id="84c5a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="84c5a-119">Type</span></span> | <span data-ttu-id="84c5a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="84c5a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="84c5a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="84c5a-121">Authorization</span></span>  | <span data-ttu-id="84c5a-122">string</span><span class="sxs-lookup"><span data-stu-id="84c5a-122">string</span></span>  | <span data-ttu-id="84c5a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84c5a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84c5a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84c5a-125">Request body</span></span>
<span data-ttu-id="84c5a-126">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="84c5a-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="84c5a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="84c5a-127">Response</span></span>

<span data-ttu-id="84c5a-128">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84c5a-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84c5a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84c5a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84c5a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84c5a-130">Request</span></span>
<span data-ttu-id="84c5a-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84c5a-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="84c5a-132">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="84c5a-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="84c5a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="84c5a-133">Response</span></span>
<span data-ttu-id="84c5a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84c5a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
