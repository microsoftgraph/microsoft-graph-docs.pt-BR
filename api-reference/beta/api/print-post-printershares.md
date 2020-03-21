---
title: Criar printerShare
description: Cria um novo compartilhamento de impressora para a impressora especificada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f4a1263f9deffe35eed89b7d7840038948ce409d
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895588"
---
# <a name="create-printershare"></a><span data-ttu-id="e4754-103">Criar printerShare</span><span class="sxs-lookup"><span data-stu-id="e4754-103">Create printerShare</span></span>

<span data-ttu-id="e4754-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4754-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4754-105">Criar um novo **printerShare** para a [impressora](../resources/printer.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="e4754-105">Create a new **printerShare** for the specified [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e4754-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4754-106">Permissions</span></span>
<span data-ttu-id="e4754-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4754-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e4754-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="e4754-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="e4754-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4754-110">Permission type</span></span> | <span data-ttu-id="e4754-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4754-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e4754-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4754-112">Delegated (work or school account)</span></span>| <span data-ttu-id="e4754-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="e4754-113">Users.Read.All</span></span> |
|<span data-ttu-id="e4754-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4754-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4754-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4754-115">Not Supported.</span></span>|
|<span data-ttu-id="e4754-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4754-116">Application</span></span>|<span data-ttu-id="e4754-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4754-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4754-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4754-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printerShares
```
## <a name="request-headers"></a><span data-ttu-id="e4754-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4754-119">Request headers</span></span>
| <span data-ttu-id="e4754-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e4754-120">Name</span></span>          | <span data-ttu-id="e4754-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4754-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e4754-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4754-122">Authorization</span></span> | <span data-ttu-id="e4754-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4754-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4754-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="e4754-125">Content-type</span></span>  | <span data-ttu-id="e4754-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4754-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4754-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4754-128">Request body</span></span>
<span data-ttu-id="e4754-129">No corpo da solicitação, forneça uma representação JSON do objeto [printerShare](../resources/printershare.md) .</span><span class="sxs-lookup"><span data-stu-id="e4754-129">In the request body, supply a JSON representation of [printerShare](../resources/printershare.md) object.</span></span>

<span data-ttu-id="e4754-130">As propriedades **ID** e **createdDateTime** do compartilhamento da impressora são definidas automaticamente na criação de recursos, mas o nome do compartilhamento e a impressora associada devem ser incluídos na solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4754-130">The printer share's **id** and **createdDateTime** properties are set automatically upon resource creation, but the share name and associated printer must be included in the request.</span></span>

<span data-ttu-id="e4754-131">A referência da impressora é definida usando `@odata.bind` a sintaxe, conforme mostrado no exemplo.</span><span class="sxs-lookup"><span data-stu-id="e4754-131">The printer reference is set by using `@odata.bind` syntax, as shown in the example.</span></span>

## <a name="response"></a><span data-ttu-id="e4754-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4754-132">Response</span></span>
<span data-ttu-id="e4754-133">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4754-133">If successful, this method returns a `201 Created` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4754-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4754-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4754-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4754-135">Request</span></span>
<span data-ttu-id="e4754-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4754-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_printershare_from_print"
}-->
```http
POST https://graph.microsoft.com/beta/print/printerShares
Content-type: application/json
Content-length: 114

{
  "name": "name-value",
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
##### <a name="response"></a><span data-ttu-id="e4754-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4754-137">Response</span></span>
<span data-ttu-id="e4754-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4754-138">The following is an example of the response.</span></span>
><span data-ttu-id="e4754-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4754-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 233

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printerShares/$entity",
    "id": "7361c7c1-ff07-4565-9897-bef6895a7d04",
    "name": "ShareName",
    "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->