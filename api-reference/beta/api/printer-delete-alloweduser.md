---
title: Excluir allowedUser da impressora
description: Revogar o acesso do usuário especificado para enviar trabalhos de impressão à impressora associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 46ebe8d1b813cd215cbdc663426042e7b2a162f6
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674369"
---
# <a name="delete-alloweduser-from-printer"></a><span data-ttu-id="487ef-103">Excluir allowedUser da impressora</span><span class="sxs-lookup"><span data-stu-id="487ef-103">Delete allowedUser from printer</span></span>

<span data-ttu-id="487ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="487ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="487ef-105">Revogar o acesso do usuário especificado para enviar trabalhos de impressão à [impressora](../resources/printer.md)associada.</span><span class="sxs-lookup"><span data-stu-id="487ef-105">Revoke the specified user's access to submit print jobs to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="487ef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="487ef-106">Permissions</span></span>
<span data-ttu-id="487ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="487ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="487ef-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="487ef-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="487ef-110">O usuário conectado deve ser um [administrador da impressora](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="487ef-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="487ef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="487ef-111">Permission type</span></span> | <span data-ttu-id="487ef-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="487ef-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="487ef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="487ef-113">Delegated (work or school account)</span></span>| <span data-ttu-id="487ef-114">Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="487ef-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="487ef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="487ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="487ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="487ef-116">Not Supported.</span></span>|
|<span data-ttu-id="487ef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="487ef-117">Application</span></span>| <span data-ttu-id="487ef-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="487ef-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="487ef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="487ef-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}/allowedUsers/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="487ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="487ef-120">Request headers</span></span>
| <span data-ttu-id="487ef-121">Nome</span><span class="sxs-lookup"><span data-stu-id="487ef-121">Name</span></span>          | <span data-ttu-id="487ef-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="487ef-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="487ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="487ef-123">Authorization</span></span> | <span data-ttu-id="487ef-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="487ef-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="487ef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="487ef-126">Request body</span></span>
<span data-ttu-id="487ef-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="487ef-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="487ef-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="487ef-128">Response</span></span>
<span data-ttu-id="487ef-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="487ef-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="487ef-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="487ef-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="487ef-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="487ef-132">Request</span></span>
<span data-ttu-id="487ef-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="487ef-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="487ef-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="487ef-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_alloweduser"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/{id}/allowedUsers/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="487ef-135">C#</span><span class="sxs-lookup"><span data-stu-id="487ef-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-alloweduser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="487ef-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="487ef-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-alloweduser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="487ef-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="487ef-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-alloweduser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="487ef-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="487ef-138">Response</span></span>
<span data-ttu-id="487ef-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="487ef-139">The following is an example of the response.</span></span>
><span data-ttu-id="487ef-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="487ef-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete allowedUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
