---
title: Criar registeredOwner
description: Adiciona um usuário como proprietário registrado do dispositivo.
author: tfitzmac
ms.openlocfilehash: 39cbd53b634b3f1388a27acf81e80ca2a7953693
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342556"
---
# <a name="create-registeredowner"></a><span data-ttu-id="b5fc2-103">Criar registeredOwner</span><span class="sxs-lookup"><span data-stu-id="b5fc2-103">Create registeredOwner</span></span>

> <span data-ttu-id="b5fc2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b5fc2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5fc2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b5fc2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b5fc2-106">Adiciona um usuário como proprietário registrado do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b5fc2-106">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5fc2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5fc2-107">Permissions</span></span>
<span data-ttu-id="b5fc2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5fc2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b5fc2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5fc2-110">Permission type</span></span>      | <span data-ttu-id="b5fc2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5fc2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5fc2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5fc2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b5fc2-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b5fc2-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b5fc2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5fc2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5fc2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5fc2-115">Not supported.</span></span>    |
|<span data-ttu-id="b5fc2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5fc2-116">Application</span></span> | <span data-ttu-id="b5fc2-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5fc2-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5fc2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5fc2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="b5fc2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5fc2-119">Request headers</span></span>
| <span data-ttu-id="b5fc2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b5fc2-120">Name</span></span>       | <span data-ttu-id="b5fc2-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5fc2-121">Type</span></span> | <span data-ttu-id="b5fc2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5fc2-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b5fc2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5fc2-123">Authorization</span></span>  | <span data-ttu-id="b5fc2-124">string</span><span class="sxs-lookup"><span data-stu-id="b5fc2-124">string</span></span>  | <span data-ttu-id="b5fc2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5fc2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5fc2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5fc2-127">Request body</span></span>
<span data-ttu-id="b5fc2-128">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="b5fc2-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b5fc2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5fc2-129">Response</span></span>

<span data-ttu-id="b5fc2-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5fc2-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5fc2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5fc2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5fc2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5fc2-132">Request</span></span>
<span data-ttu-id="b5fc2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5fc2-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="b5fc2-134">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="b5fc2-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b5fc2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5fc2-135">Response</span></span>
<span data-ttu-id="b5fc2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5fc2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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