---
title: Criar registeredOwner
description: Adiciona um usuário como proprietário registrado do dispositivo.
ms.openlocfilehash: 767b28d8af9c26c336e36698024d89dac7f97786
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033590"
---
# <a name="create-registeredowner"></a><span data-ttu-id="a5e62-103">Criar registeredOwner</span><span class="sxs-lookup"><span data-stu-id="a5e62-103">Create registeredOwner</span></span>

> <span data-ttu-id="a5e62-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a5e62-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5e62-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a5e62-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5e62-106">Adiciona um usuário como proprietário registrado do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a5e62-106">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="a5e62-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5e62-107">Permissions</span></span>
<span data-ttu-id="a5e62-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5e62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a5e62-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5e62-110">Permission type</span></span>      | <span data-ttu-id="a5e62-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5e62-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5e62-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5e62-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a5e62-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5e62-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5e62-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5e62-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5e62-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5e62-115">Not supported.</span></span>    |
|<span data-ttu-id="a5e62-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5e62-116">Application</span></span> | <span data-ttu-id="a5e62-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5e62-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5e62-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5e62-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="a5e62-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e62-119">Request headers</span></span>
| <span data-ttu-id="a5e62-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a5e62-120">Name</span></span>       | <span data-ttu-id="a5e62-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5e62-121">Type</span></span> | <span data-ttu-id="a5e62-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5e62-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a5e62-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5e62-123">Authorization</span></span>  | <span data-ttu-id="a5e62-124">string</span><span class="sxs-lookup"><span data-stu-id="a5e62-124">string</span></span>  | <span data-ttu-id="a5e62-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5e62-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5e62-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e62-127">Request body</span></span>
<span data-ttu-id="a5e62-128">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="a5e62-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a5e62-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5e62-129">Response</span></span>

<span data-ttu-id="a5e62-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5e62-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5e62-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5e62-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5e62-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e62-132">Request</span></span>
<span data-ttu-id="a5e62-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5e62-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredOwners/$ref
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="a5e62-134">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="a5e62-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a5e62-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5e62-135">Response</span></span>
<span data-ttu-id="a5e62-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5e62-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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