---
title: Listar allowedGroups
description: Recupere uma lista de grupos aos quais o acesso foi concedido para enviar trabalhos de impressão à impressora associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 845a8e9a379b72067117ad4f157964f926f89a60
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895564"
---
# <a name="list-allowedgroups"></a><span data-ttu-id="df5c3-103">Listar allowedGroups</span><span class="sxs-lookup"><span data-stu-id="df5c3-103">List allowedGroups</span></span>

<span data-ttu-id="df5c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df5c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df5c3-105">Recupere uma lista de grupos aos quais o acesso foi concedido para enviar trabalhos de impressão à [impressora](../resources/printer.md)associada.</span><span class="sxs-lookup"><span data-stu-id="df5c3-105">Retrieve a list of groups that have been granted access to submit print jobs to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df5c3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df5c3-106">Permissions</span></span>
<span data-ttu-id="df5c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df5c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="df5c3-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="df5c3-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="df5c3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df5c3-110">Permission type</span></span> | <span data-ttu-id="df5c3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df5c3-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="df5c3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df5c3-112">Delegated (work or school account)</span></span>| <span data-ttu-id="df5c3-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="df5c3-113">Users.Read.All</span></span> |
|<span data-ttu-id="df5c3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df5c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df5c3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df5c3-115">Not Supported.</span></span>|
|<span data-ttu-id="df5c3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df5c3-116">Application</span></span>|<span data-ttu-id="df5c3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df5c3-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df5c3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df5c3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/allowedGroups
```

## <a name="request-headers"></a><span data-ttu-id="df5c3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df5c3-119">Request headers</span></span>
| <span data-ttu-id="df5c3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="df5c3-120">Name</span></span>      |<span data-ttu-id="df5c3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="df5c3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="df5c3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="df5c3-122">Authorization</span></span> | <span data-ttu-id="df5c3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df5c3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df5c3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df5c3-125">Request body</span></span>
<span data-ttu-id="df5c3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df5c3-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="df5c3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="df5c3-127">Response</span></span>
<span data-ttu-id="df5c3-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Identity](../resources/identity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df5c3-128">If successful, this method returns a `200 OK` response code and a collection of [identity](../resources/identity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="df5c3-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df5c3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df5c3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df5c3-130">Request</span></span>
<span data-ttu-id="df5c3-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df5c3-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_allowedGroups"
}-->
```http
GET https://graph.microsoft.com/beta/print/printers/{id}/allowedGroups
```
##### <a name="response"></a><span data-ttu-id="df5c3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="df5c3-132">Response</span></span>
<span data-ttu-id="df5c3-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df5c3-133">The following is an example of the response.</span></span>
><span data-ttu-id="df5c3-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df5c3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identity",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 233

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printIdentity)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "GroupName"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List allowedGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->