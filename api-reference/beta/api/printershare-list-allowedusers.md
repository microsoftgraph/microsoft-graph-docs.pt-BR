---
title: Listar allowedUsers para printerShare
description: Recupere uma lista de usuários que receberam acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 3d8e6ee823bc07e01355521108adb169d43b0f3d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035495"
---
# <a name="list-allowedusers-for-printershare"></a><span data-ttu-id="93f31-103">Listar allowedUsers para printerShare</span><span class="sxs-lookup"><span data-stu-id="93f31-103">List allowedUsers for printerShare</span></span>

<span data-ttu-id="93f31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93f31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93f31-105">Recupere uma lista de usuários com acesso concedido para enviar trabalhos de impressão para o [printerShare](../resources/printershare.md)associado.</span><span class="sxs-lookup"><span data-stu-id="93f31-105">Retrieve a list of users who have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="93f31-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="93f31-106">Permissions</span></span>
<span data-ttu-id="93f31-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93f31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="93f31-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="93f31-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="93f31-110">O usuário conectado deve ser um [administrador da impressora](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="93f31-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="93f31-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93f31-111">Permission type</span></span> | <span data-ttu-id="93f31-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93f31-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="93f31-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93f31-113">Delegated (work or school account)</span></span>| <span data-ttu-id="93f31-114">PrinterShare. Read. All, PrinterShare. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="93f31-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="93f31-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93f31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93f31-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93f31-116">Not Supported.</span></span>|
|<span data-ttu-id="93f31-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93f31-117">Application</span></span>|<span data-ttu-id="93f31-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93f31-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93f31-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93f31-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}/allowedUsers
```

## <a name="request-headers"></a><span data-ttu-id="93f31-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93f31-120">Request headers</span></span>
| <span data-ttu-id="93f31-121">Nome</span><span class="sxs-lookup"><span data-stu-id="93f31-121">Name</span></span>      |<span data-ttu-id="93f31-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="93f31-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="93f31-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="93f31-123">Authorization</span></span> | <span data-ttu-id="93f31-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93f31-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93f31-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93f31-126">Request body</span></span>
<span data-ttu-id="93f31-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93f31-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="93f31-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="93f31-128">Response</span></span>
<span data-ttu-id="93f31-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printUserIdentity](../resources/printuseridentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93f31-129">If successful, this method returns a `200 OK` response code and a collection of [printUserIdentity](../resources/printuseridentity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93f31-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93f31-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="93f31-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93f31-131">Request</span></span>
<span data-ttu-id="93f31-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93f31-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="93f31-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="93f31-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedUsers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}/allowedUsers
```
# <a name="c"></a>[<span data-ttu-id="93f31-134">C#</span><span class="sxs-lookup"><span data-stu-id="93f31-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93f31-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93f31-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93f31-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93f31-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="93f31-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="93f31-137">Response</span></span>
<span data-ttu-id="93f31-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="93f31-138">The following is an example of the response.</span></span>
><span data-ttu-id="93f31-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93f31-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


