---
title: Eliminar printerShare
description: Exclua um compartilhamento de impressora (desassolhe a impressora associada). Não é possível desfazer a ação. Se a impressora for compartilhada novamente no futuro, todos os usuários do Windows que instalaram anteriormente a impressora precisarão descobrir e instalá-la novamente.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 95a907f18693165304894fab41da36e28b551f35
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771663"
---
# <a name="delete-printershare"></a><span data-ttu-id="27058-105">Eliminar printerShare</span><span class="sxs-lookup"><span data-stu-id="27058-105">Delete printerShare</span></span>
<span data-ttu-id="27058-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27058-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="27058-107">Excluir um compartilhamento de impressora (desatar a impressora [associada](../resources/printer.md)).</span><span class="sxs-lookup"><span data-stu-id="27058-107">Delete a printer share (unshare the associated [printer](../resources/printer.md)).</span></span> <span data-ttu-id="27058-108">Não é possível desfazer a ação.</span><span class="sxs-lookup"><span data-stu-id="27058-108">This action cannot be undone.</span></span> <span data-ttu-id="27058-109">Se a [impressora](../resources/printer.md) for compartilhada novamente no futuro, todos [](../resources/printer.md) os usuários do Windows que instalaram anteriormente a impressora precisarão descobrir e reinstalá-la.</span><span class="sxs-lookup"><span data-stu-id="27058-109">If the [printer](../resources/printer.md) is shared again in the future, any Windows users who had previously installed the [printer](../resources/printer.md) will need to discover and reinstall it.</span></span>

## <a name="permissions"></a><span data-ttu-id="27058-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="27058-110">Permissions</span></span>
<span data-ttu-id="27058-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27058-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="27058-113">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="27058-113">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="27058-114">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="27058-114">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="27058-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27058-115">Permission type</span></span> | <span data-ttu-id="27058-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27058-116">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="27058-117">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27058-117">Delegated (work or school account)</span></span>| <span data-ttu-id="27058-118">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27058-118">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="27058-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27058-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27058-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27058-120">Not Supported.</span></span>|
|<span data-ttu-id="27058-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27058-121">Application</span></span>|<span data-ttu-id="27058-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27058-122">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27058-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27058-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/shares/{printerShareId}
```

## <a name="request-headers"></a><span data-ttu-id="27058-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27058-124">Request headers</span></span>
|<span data-ttu-id="27058-125">Nome</span><span class="sxs-lookup"><span data-stu-id="27058-125">Name</span></span>|<span data-ttu-id="27058-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="27058-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="27058-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="27058-127">Authorization</span></span>|<span data-ttu-id="27058-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27058-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27058-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27058-130">Request body</span></span>
<span data-ttu-id="27058-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27058-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27058-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="27058-132">Response</span></span>

<span data-ttu-id="27058-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27058-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27058-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="27058-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27058-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27058-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="27058-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="27058-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printershare"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/shares/{printerShareId}
```
# <a name="c"></a>[<span data-ttu-id="27058-138">C#</span><span class="sxs-lookup"><span data-stu-id="27058-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27058-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27058-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27058-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27058-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27058-141">Java</span><span class="sxs-lookup"><span data-stu-id="27058-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="27058-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="27058-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

