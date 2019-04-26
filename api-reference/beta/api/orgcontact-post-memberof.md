---
title: Criar memberOf
description: Use esta API para criar um novo memberOf.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 01d36b92bae6546cc3c279de3bbb4429eb67dc06
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332679"
---
# <a name="create-memberof"></a><span data-ttu-id="78035-103">Criar memberOf</span><span class="sxs-lookup"><span data-stu-id="78035-103">Create memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78035-104">Use esta API para criar um novo memberOf.</span><span class="sxs-lookup"><span data-stu-id="78035-104">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="78035-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="78035-105">Permissions</span></span>
<span data-ttu-id="78035-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78035-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78035-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78035-108">Permission type</span></span>      | <span data-ttu-id="78035-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78035-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78035-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78035-110">Delegated (work or school account)</span></span> | <span data-ttu-id="78035-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78035-111">Not supported.</span></span>    |
|<span data-ttu-id="78035-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78035-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78035-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78035-113">Not supported.</span></span>    |
|<span data-ttu-id="78035-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78035-114">Application</span></span> | <span data-ttu-id="78035-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78035-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78035-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78035-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="78035-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78035-117">Request headers</span></span>
| <span data-ttu-id="78035-118">Nome</span><span class="sxs-lookup"><span data-stu-id="78035-118">Name</span></span>       | <span data-ttu-id="78035-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="78035-119">Type</span></span> | <span data-ttu-id="78035-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="78035-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="78035-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="78035-121">Authorization</span></span>  | <span data-ttu-id="78035-122">string</span><span class="sxs-lookup"><span data-stu-id="78035-122">string</span></span>  | <span data-ttu-id="78035-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78035-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78035-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78035-125">Request body</span></span>
<span data-ttu-id="78035-126">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="78035-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="78035-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="78035-127">Response</span></span>

<span data-ttu-id="78035-128">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78035-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78035-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78035-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78035-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78035-130">Request</span></span>
<span data-ttu-id="78035-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78035-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/memberOf
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="78035-132">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="78035-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="78035-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="78035-133">Response</span></span>
<span data-ttu-id="78035-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78035-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
