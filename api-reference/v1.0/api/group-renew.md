---
title: 'group: renew'
description: Renova o período de validade de um grupo. Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.
ms.openlocfilehash: 82cbc4f982b5636cc53436091a40492d7ad83afa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005377"
---
# <a name="group-renew"></a><span data-ttu-id="9ef38-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="9ef38-104">group: renew</span></span>

<span data-ttu-id="9ef38-105">Renova o período de validade de um grupo.</span><span class="sxs-lookup"><span data-stu-id="9ef38-105">Renews a group's expiration.</span></span> <span data-ttu-id="9ef38-106">Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="9ef38-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ef38-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ef38-107">Permissions</span></span>

<span data-ttu-id="9ef38-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ef38-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="9ef38-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ef38-110">Permission type</span></span>      | <span data-ttu-id="9ef38-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ef38-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ef38-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ef38-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9ef38-113">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef38-113">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="9ef38-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ef38-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ef38-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9ef38-115">Not supported</span></span> |
|<span data-ttu-id="9ef38-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ef38-116">Application</span></span> | <span data-ttu-id="9ef38-117">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef38-117">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ef38-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ef38-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="9ef38-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ef38-119">Request headers</span></span>
| <span data-ttu-id="9ef38-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9ef38-120">Name</span></span>       | <span data-ttu-id="9ef38-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ef38-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9ef38-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ef38-122">Authorization</span></span>  | <span data-ttu-id="9ef38-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="9ef38-123">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="9ef38-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ef38-124">Request body</span></span>

<span data-ttu-id="9ef38-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ef38-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ef38-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ef38-126">Response</span></span>

<span data-ttu-id="9ef38-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ef38-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ef38-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ef38-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9ef38-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ef38-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```

##### <a name="response"></a><span data-ttu-id="9ef38-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ef38-131">Response</span></span>
<span data-ttu-id="9ef38-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ef38-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->