---
title: Excluir um grupo de roteamento de áudio
description: Exclua o grupo de roteamento de áudio especificado.
author: VinodRavichandran
ms.openlocfilehash: a21c90722b63d582f3c76ff518bcc68837135593
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380370"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="18a99-103">Excluir um grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="18a99-103">Delete audio routing group</span></span>

> <span data-ttu-id="18a99-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="18a99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18a99-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="18a99-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18a99-106">Exclua o especificado [audioRoutingGroup](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="18a99-106">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="18a99-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="18a99-107">Permissions</span></span>
<span data-ttu-id="18a99-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18a99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18a99-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18a99-110">Permission type</span></span> | <span data-ttu-id="18a99-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18a99-111">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="18a99-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18a99-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="18a99-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="18a99-113">Not Supported</span></span>        |
| <span data-ttu-id="18a99-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18a99-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18a99-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="18a99-115">Not Supported</span></span>        |
| <span data-ttu-id="18a99-116">Application</span><span class="sxs-lookup"><span data-stu-id="18a99-116">Application</span></span>     | <span data-ttu-id="18a99-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="18a99-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18a99-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18a99-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="18a99-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18a99-119">Request headers</span></span>
| <span data-ttu-id="18a99-120">Nome</span><span class="sxs-lookup"><span data-stu-id="18a99-120">Name</span></span>          | <span data-ttu-id="18a99-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="18a99-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="18a99-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="18a99-122">Authorization</span></span> | <span data-ttu-id="18a99-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18a99-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18a99-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18a99-125">Request body</span></span>
<span data-ttu-id="18a99-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="18a99-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18a99-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="18a99-127">Response</span></span>
<span data-ttu-id="18a99-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18a99-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18a99-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18a99-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="18a99-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18a99-131">Request</span></span>
<span data-ttu-id="18a99-132">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="18a99-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="18a99-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="18a99-133">Response</span></span>

> <span data-ttu-id="18a99-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18a99-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
