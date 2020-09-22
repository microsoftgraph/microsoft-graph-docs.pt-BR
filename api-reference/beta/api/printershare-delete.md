---
title: Eliminar printerShare
description: Excluir um compartilhamento de impressora (descompartilhar a impressora associada). Não é possível desfazer a ação. Se a impressora for compartilhada novamente no futuro, qualquer usuário do Windows que tenha instalado anteriormente a impressora deverá descobrir e reinstalá-la.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f86270c9662ed74204cf193c35b57a12060a4e73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035516"
---
# <a name="delete-printershare"></a><span data-ttu-id="e1b8e-105">Eliminar printerShare</span><span class="sxs-lookup"><span data-stu-id="e1b8e-105">Delete printerShare</span></span>

<span data-ttu-id="e1b8e-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1b8e-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1b8e-107">Excluir um compartilhamento de impressora (descompartilhar a [impressora](../resources/printer.md)associada).</span><span class="sxs-lookup"><span data-stu-id="e1b8e-107">Delete a printer share (unshare the associated [printer](../resources/printer.md)).</span></span> <span data-ttu-id="e1b8e-108">Não é possível desfazer a ação.</span><span class="sxs-lookup"><span data-stu-id="e1b8e-108">This action cannot be undone.</span></span> <span data-ttu-id="e1b8e-109">Se a [impressora](../resources/printer.md) for compartilhada novamente no futuro, qualquer usuário do Windows que tenha instalado anteriormente a [impressora](../resources/printer.md) deverá descobrir e reinstalá-la.</span><span class="sxs-lookup"><span data-stu-id="e1b8e-109">If the [printer](../resources/printer.md) is shared again in the future, any Windows users who had previously installed the [printer](../resources/printer.md) will need to discover and reinstall it.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1b8e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1b8e-110">Permissions</span></span>
<span data-ttu-id="e1b8e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1b8e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e1b8e-113">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="e1b8e-113">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="e1b8e-114">O usuário conectado deve ser um [administrador da impressora](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="e1b8e-114">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="e1b8e-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1b8e-115">Permission type</span></span> | <span data-ttu-id="e1b8e-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1b8e-116">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e1b8e-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1b8e-117">Delegated (work or school account)</span></span>| <span data-ttu-id="e1b8e-118">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b8e-118">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="e1b8e-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1b8e-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1b8e-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1b8e-120">Not Supported.</span></span>|
|<span data-ttu-id="e1b8e-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1b8e-121">Application</span></span>|<span data-ttu-id="e1b8e-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1b8e-122">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1b8e-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1b8e-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{id}
DELETE /print/printers/{id}/share
```
## <a name="request-headers"></a><span data-ttu-id="e1b8e-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1b8e-124">Request headers</span></span>
| <span data-ttu-id="e1b8e-125">Nome</span><span class="sxs-lookup"><span data-stu-id="e1b8e-125">Name</span></span>          | <span data-ttu-id="e1b8e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1b8e-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e1b8e-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1b8e-127">Authorization</span></span> | <span data-ttu-id="e1b8e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1b8e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1b8e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1b8e-130">Request body</span></span>
<span data-ttu-id="e1b8e-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1b8e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1b8e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1b8e-132">Response</span></span>
<span data-ttu-id="e1b8e-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1b8e-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1b8e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1b8e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1b8e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1b8e-136">Request</span></span>
<span data-ttu-id="e1b8e-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1b8e-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1b8e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1b8e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printershare"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/shares/{id}
```
# <a name="c"></a>[<span data-ttu-id="e1b8e-139">C#</span><span class="sxs-lookup"><span data-stu-id="e1b8e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1b8e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1b8e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1b8e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1b8e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e1b8e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1b8e-142">Response</span></span>
<span data-ttu-id="e1b8e-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1b8e-143">The following is an example of the response.</span></span>
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
  "description": "Delete printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


