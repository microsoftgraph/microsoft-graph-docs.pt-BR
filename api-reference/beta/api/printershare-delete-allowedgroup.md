---
title: Excluir allowedGroup de printerShare
description: Revogar o acesso do grupo especificado para enviar trabalhos de impressão para o compartilhamento de impressora associado.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: dce2a4d044b555116396953e926ef3c5d8c13fb0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051057"
---
# <a name="delete-allowedgroup-from-printershare"></a><span data-ttu-id="3e47a-103">Excluir allowedGroup de printerShare</span><span class="sxs-lookup"><span data-stu-id="3e47a-103">Delete allowedGroup from printerShare</span></span>

<span data-ttu-id="3e47a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e47a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e47a-105">Revogar o acesso do grupo especificado para enviar trabalhos de impressão para a [impressora associadaShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="3e47a-105">Revoke the specified group's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e47a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e47a-106">Permissions</span></span>
<span data-ttu-id="3e47a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e47a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3e47a-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="3e47a-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="3e47a-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="3e47a-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="3e47a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e47a-111">Permission type</span></span> | <span data-ttu-id="3e47a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e47a-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3e47a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e47a-113">Delegated (work or school account)</span></span>| <span data-ttu-id="3e47a-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e47a-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="3e47a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e47a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e47a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e47a-116">Not Supported.</span></span>|
|<span data-ttu-id="3e47a-117">Application</span><span class="sxs-lookup"><span data-stu-id="3e47a-117">Application</span></span>|<span data-ttu-id="3e47a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e47a-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e47a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e47a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{id}/allowedGroups/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="3e47a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e47a-120">Request headers</span></span>
| <span data-ttu-id="3e47a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3e47a-121">Name</span></span>          | <span data-ttu-id="3e47a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e47a-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3e47a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e47a-123">Authorization</span></span> | <span data-ttu-id="3e47a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e47a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e47a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e47a-126">Request body</span></span>
<span data-ttu-id="3e47a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e47a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e47a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e47a-128">Response</span></span>
<span data-ttu-id="3e47a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e47a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e47a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e47a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e47a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e47a-132">Request</span></span>
<span data-ttu-id="3e47a-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e47a-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3e47a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e47a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_allowedgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/shares/{id}/allowedGroups/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="3e47a-135">C#</span><span class="sxs-lookup"><span data-stu-id="3e47a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-allowedgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e47a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e47a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-allowedgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e47a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e47a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-allowedgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3e47a-138">Java</span><span class="sxs-lookup"><span data-stu-id="3e47a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-allowedgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3e47a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e47a-139">Response</span></span>
<span data-ttu-id="3e47a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3e47a-140">The following is an example of the response.</span></span>
><span data-ttu-id="3e47a-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3e47a-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Delete allowedGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
