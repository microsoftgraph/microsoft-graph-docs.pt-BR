---
title: Excluir allowedUser de printerShare
description: Revogar o acesso do usuário especificado para enviar trabalhos de impressão para o compartilhamento de impressora associado.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 453fd853c7631ccb84c8b5709a33a787fc859444
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771740"
---
# <a name="delete-alloweduser-from-printershare"></a><span data-ttu-id="1f0d8-103">Excluir allowedUser de printerShare</span><span class="sxs-lookup"><span data-stu-id="1f0d8-103">Delete allowedUser from printerShare</span></span>

<span data-ttu-id="1f0d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f0d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="1f0d8-105">Revogar o acesso do usuário especificado para enviar trabalhos de impressão para a impressora [associadaShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="1f0d8-105">Revoke the specified user's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1f0d8-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1f0d8-106">Permissions</span></span>
<span data-ttu-id="1f0d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f0d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1f0d8-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="1f0d8-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="1f0d8-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="1f0d8-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="1f0d8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f0d8-111">Permission type</span></span> | <span data-ttu-id="1f0d8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f0d8-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1f0d8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f0d8-113">Delegated (work or school account)</span></span>| <span data-ttu-id="1f0d8-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f0d8-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="1f0d8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f0d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f0d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f0d8-116">Not Supported.</span></span>|
|<span data-ttu-id="1f0d8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f0d8-117">Application</span></span>|<span data-ttu-id="1f0d8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f0d8-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f0d8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f0d8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{printerShareId}/allowedUsers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="1f0d8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f0d8-120">Request headers</span></span>
| <span data-ttu-id="1f0d8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1f0d8-121">Name</span></span>          | <span data-ttu-id="1f0d8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f0d8-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1f0d8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f0d8-123">Authorization</span></span> | <span data-ttu-id="1f0d8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f0d8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f0d8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f0d8-126">Request body</span></span>
<span data-ttu-id="1f0d8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f0d8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f0d8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f0d8-128">Response</span></span>
<span data-ttu-id="1f0d8-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f0d8-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f0d8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f0d8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f0d8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f0d8-132">Request</span></span>
<span data-ttu-id="1f0d8-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f0d8-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1f0d8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f0d8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_alloweduser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedUsers/{userId}/$ref
```
# <a name="c"></a>[<span data-ttu-id="1f0d8-135">C#</span><span class="sxs-lookup"><span data-stu-id="1f0d8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-alloweduser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f0d8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f0d8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-alloweduser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f0d8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f0d8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-alloweduser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f0d8-138">Java</span><span class="sxs-lookup"><span data-stu-id="1f0d8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-alloweduser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f0d8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f0d8-139">Response</span></span>
<span data-ttu-id="1f0d8-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1f0d8-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
