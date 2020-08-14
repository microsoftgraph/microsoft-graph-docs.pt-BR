---
title: Excluir printerShare
description: Excluir um compartilhamento de impressora (descompartilhar a impressora associada). Não é possível desfazer a ação. Se a impressora for compartilhada novamente no futuro, qualquer usuário do Windows que tenha instalado anteriormente a impressora deverá descobrir e reinstalá-la.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 312a5e9a3cdfd8c03c4c7dae3d2d712c7c374248
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2020
ms.locfileid: "46673935"
---
# <a name="delete-printershare"></a><span data-ttu-id="cf558-105">Excluir printerShare</span><span class="sxs-lookup"><span data-stu-id="cf558-105">Delete printerShare</span></span>

<span data-ttu-id="cf558-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf558-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf558-107">Excluir um compartilhamento de impressora (descompartilhar a [impressora](../resources/printer.md)associada).</span><span class="sxs-lookup"><span data-stu-id="cf558-107">Delete a printer share (unshare the associated [printer](../resources/printer.md)).</span></span> <span data-ttu-id="cf558-108">Não é possível desfazer a ação.</span><span class="sxs-lookup"><span data-stu-id="cf558-108">This action cannot be undone.</span></span> <span data-ttu-id="cf558-109">Se a [impressora](../resources/printer.md) for compartilhada novamente no futuro, qualquer usuário do Windows que tenha instalado anteriormente a [impressora](../resources/printer.md) deverá descobrir e reinstalá-la.</span><span class="sxs-lookup"><span data-stu-id="cf558-109">If the [printer](../resources/printer.md) is shared again in the future, any Windows users who had previously installed the [printer](../resources/printer.md) will need to discover and reinstall it.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf558-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf558-110">Permissions</span></span>
<span data-ttu-id="cf558-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf558-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="cf558-113">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="cf558-113">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="cf558-114">O usuário conectado deve ser um [administrador da impressora](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="cf558-114">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="cf558-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf558-115">Permission type</span></span> | <span data-ttu-id="cf558-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf558-116">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="cf558-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf558-117">Delegated (work or school account)</span></span>| <span data-ttu-id="cf558-118">PrinterShare. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cf558-118">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="cf558-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf558-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf558-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf558-120">Not Supported.</span></span>|
|<span data-ttu-id="cf558-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf558-121">Application</span></span>|<span data-ttu-id="cf558-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf558-122">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf558-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf558-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{id}
DELETE /print/printers/{id}/share
```
## <a name="request-headers"></a><span data-ttu-id="cf558-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf558-124">Request headers</span></span>
| <span data-ttu-id="cf558-125">Nome</span><span class="sxs-lookup"><span data-stu-id="cf558-125">Name</span></span>          | <span data-ttu-id="cf558-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf558-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cf558-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf558-127">Authorization</span></span> | <span data-ttu-id="cf558-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf558-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf558-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf558-130">Request body</span></span>
<span data-ttu-id="cf558-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf558-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf558-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf558-132">Response</span></span>
<span data-ttu-id="cf558-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf558-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf558-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf558-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf558-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf558-136">Request</span></span>
<span data-ttu-id="cf558-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf558-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf558-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf558-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printershare"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/shares/{id}
```
# <a name="c"></a>[<span data-ttu-id="cf558-139">C#</span><span class="sxs-lookup"><span data-stu-id="cf558-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf558-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf558-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf558-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf558-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cf558-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf558-142">Response</span></span>
<span data-ttu-id="cf558-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cf558-143">The following is an example of the response.</span></span>
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
