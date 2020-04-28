---
title: Listar allowedUsers
description: Recupere uma lista de usuários que receberam acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: b89a8aaf1064fe837ceaae121fcf656353c8c410
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916939"
---
# <a name="list-allowedusers"></a><span data-ttu-id="14e13-103">Listar allowedUsers</span><span class="sxs-lookup"><span data-stu-id="14e13-103">List allowedUsers</span></span>

<span data-ttu-id="14e13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14e13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14e13-105">Recupere uma lista de usuários com acesso concedido para enviar trabalhos de impressão para o [printerShare](../resources/printershare.md)associado.</span><span class="sxs-lookup"><span data-stu-id="14e13-105">Retrieve a list of users who have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="14e13-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="14e13-106">Permissions</span></span>
<span data-ttu-id="14e13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14e13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="14e13-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="14e13-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="14e13-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14e13-110">Permission type</span></span> | <span data-ttu-id="14e13-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14e13-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="14e13-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14e13-112">Delegated (work or school account)</span></span>| <span data-ttu-id="14e13-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="14e13-113">Users.Read.All</span></span> |
|<span data-ttu-id="14e13-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14e13-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14e13-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14e13-115">Not Supported.</span></span>|
|<span data-ttu-id="14e13-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14e13-116">Application</span></span>|<span data-ttu-id="14e13-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14e13-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14e13-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14e13-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printerShares/{id}/allowedUsers
```

## <a name="request-headers"></a><span data-ttu-id="14e13-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14e13-119">Request headers</span></span>
| <span data-ttu-id="14e13-120">Nome</span><span class="sxs-lookup"><span data-stu-id="14e13-120">Name</span></span>      |<span data-ttu-id="14e13-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="14e13-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="14e13-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="14e13-122">Authorization</span></span> | <span data-ttu-id="14e13-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14e13-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14e13-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14e13-125">Request body</span></span>
<span data-ttu-id="14e13-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14e13-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="14e13-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="14e13-127">Response</span></span>
<span data-ttu-id="14e13-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [printUserIdentity](../resources/printuseridentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14e13-128">If successful, this method returns a `200 OK` response code and a collection of [printUserIdentity](../resources/printuseridentity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14e13-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14e13-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="14e13-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14e13-130">Request</span></span>
<span data-ttu-id="14e13-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14e13-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_allowedUsers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printerShares/{id}/allowedUsers
```

### <a name="response"></a><span data-ttu-id="14e13-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="14e13-132">Response</span></span>
<span data-ttu-id="14e13-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14e13-133">The following is an example of the response.</span></span>
><span data-ttu-id="14e13-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14e13-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUserIdentity",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 286

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printUserIdentity)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "UserName",
      "userPrincipalName": "username@microsoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List allowedUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
