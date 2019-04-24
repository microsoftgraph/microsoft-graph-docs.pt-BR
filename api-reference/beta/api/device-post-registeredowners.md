---
title: Criar registeredOwner
description: Adiciona um usuário como proprietário registrado do dispositivo.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 24c5c7977e8989bd4b790df3ec0629f61a654422
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455150"
---
# <a name="create-registeredowner"></a><span data-ttu-id="9eafb-103">Criar registeredOwner</span><span class="sxs-lookup"><span data-stu-id="9eafb-103">Create registeredOwner</span></span>

<span data-ttu-id="9eafb-104">Adiciona um usuário como proprietário registrado do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9eafb-104">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="9eafb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9eafb-105">Permissions</span></span>
<span data-ttu-id="9eafb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9eafb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9eafb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9eafb-108">Permission type</span></span>      | <span data-ttu-id="9eafb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9eafb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9eafb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9eafb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9eafb-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9eafb-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9eafb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9eafb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9eafb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9eafb-113">Not supported.</span></span>    |
|<span data-ttu-id="9eafb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9eafb-114">Application</span></span> | <span data-ttu-id="9eafb-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9eafb-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9eafb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9eafb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="9eafb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9eafb-117">Request headers</span></span>
| <span data-ttu-id="9eafb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9eafb-118">Name</span></span>       | <span data-ttu-id="9eafb-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9eafb-119">Type</span></span> | <span data-ttu-id="9eafb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9eafb-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9eafb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9eafb-121">Authorization</span></span>  | <span data-ttu-id="9eafb-122">string</span><span class="sxs-lookup"><span data-stu-id="9eafb-122">string</span></span>  | <span data-ttu-id="9eafb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9eafb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9eafb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9eafb-125">Request body</span></span>
<span data-ttu-id="9eafb-126">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="9eafb-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9eafb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9eafb-127">Response</span></span>

<span data-ttu-id="9eafb-128">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9eafb-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9eafb-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9eafb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9eafb-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9eafb-130">Request</span></span>
<span data-ttu-id="9eafb-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9eafb-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="9eafb-132">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="9eafb-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9eafb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9eafb-133">Response</span></span>
<span data-ttu-id="9eafb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9eafb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
