---
title: Criar allowedGroup para printerShare
description: Conceda ao grupo especificado acesso para enviar trabalhos de impressão à impressora associada.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: a6a5e2cb69c2ee9ee65ef012108d001312666a74
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787783"
---
# <a name="create-allowedgroup-for-printershare"></a><span data-ttu-id="5e2e3-103">Criar allowedGroup para printerShare</span><span class="sxs-lookup"><span data-stu-id="5e2e3-103">Create allowedGroup for printerShare</span></span>
<span data-ttu-id="5e2e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e2e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="5e2e3-105">Conceda ao grupo especificado acesso para enviar trabalhos de impressão para a [impressora associadaShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="5e2e3-105">Grant the specified group access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5e2e3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e2e3-106">Permissions</span></span>
<span data-ttu-id="5e2e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e2e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5e2e3-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="5e2e3-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="5e2e3-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="5e2e3-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="5e2e3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e2e3-111">Permission type</span></span> | <span data-ttu-id="5e2e3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e2e3-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5e2e3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e2e3-113">Delegated (work or school account)</span></span>| <span data-ttu-id="5e2e3-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e2e3-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="5e2e3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e2e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e2e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e2e3-116">Not Supported.</span></span>|
|<span data-ttu-id="5e2e3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e2e3-117">Application</span></span>|<span data-ttu-id="5e2e3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e2e3-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e2e3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e2e3-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/shares/{printerShareId}/allowedGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5e2e3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e2e3-120">Request headers</span></span>
|<span data-ttu-id="5e2e3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5e2e3-121">Name</span></span>|<span data-ttu-id="5e2e3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e2e3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5e2e3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e2e3-123">Authorization</span></span>|<span data-ttu-id="5e2e3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e2e3-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5e2e3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e2e3-126">Content-Type</span></span>|<span data-ttu-id="5e2e3-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e2e3-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e2e3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e2e3-129">Request body</span></span>
<span data-ttu-id="5e2e3-130">No corpo da solicitação, fornece uma referência a uma entidade de grupo usando o formato, conforme `@odata.id` mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="5e2e3-130">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="5e2e3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e2e3-131">Response</span></span>

<span data-ttu-id="5e2e3-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5e2e3-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5e2e3-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5e2e3-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5e2e3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e2e3-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5e2e3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e2e3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_group_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedGroups/$ref
Content-Type: application/json
Content-length: 47

{
  "@odata.id": "https://graph.microsoft.com/v1.0/groups/{groupId}"
}
```
# <a name="c"></a>[<span data-ttu-id="5e2e3-136">C#</span><span class="sxs-lookup"><span data-stu-id="5e2e3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e2e3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e2e3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e2e3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e2e3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e2e3-139">Java</span><span class="sxs-lookup"><span data-stu-id="5e2e3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5e2e3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e2e3-140">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

