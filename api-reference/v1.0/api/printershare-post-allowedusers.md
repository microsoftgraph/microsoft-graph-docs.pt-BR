---
title: Criar allowedUser para printerShare
description: Conceda ao usuário especificado acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 9a3d198c225633ebeecf7de8d5c069e49c014eeb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771425"
---
# <a name="create-alloweduser-for-printershare"></a><span data-ttu-id="b365d-103">Criar allowedUser para printerShare</span><span class="sxs-lookup"><span data-stu-id="b365d-103">Create allowedUser for printerShare</span></span>
<span data-ttu-id="b365d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b365d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="b365d-105">Conceda ao usuário especificado acesso para enviar trabalhos de impressão para a [impressora associadaShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="b365d-105">Grant the specified user access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b365d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b365d-106">Permissions</span></span>
<span data-ttu-id="b365d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b365d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b365d-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="b365d-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="b365d-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="b365d-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="b365d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b365d-111">Permission type</span></span> | <span data-ttu-id="b365d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b365d-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b365d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b365d-113">Delegated (work or school account)</span></span>| <span data-ttu-id="b365d-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b365d-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="b365d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b365d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b365d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b365d-116">Not Supported.</span></span>|
|<span data-ttu-id="b365d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b365d-117">Application</span></span>|<span data-ttu-id="b365d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b365d-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b365d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b365d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares/{printerShareId}/allowedUsers/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b365d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b365d-120">Request headers</span></span>
|<span data-ttu-id="b365d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b365d-121">Name</span></span>|<span data-ttu-id="b365d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b365d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b365d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b365d-123">Authorization</span></span>|<span data-ttu-id="b365d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b365d-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b365d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b365d-126">Content-Type</span></span>|<span data-ttu-id="b365d-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b365d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b365d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b365d-129">Request body</span></span>
<span data-ttu-id="b365d-130">No corpo da solicitação, fornece uma referência a uma entidade de usuário usando o formato, conforme `@odata.id` mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="b365d-130">In the request body, supply a reference to a user entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="b365d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b365d-131">Response</span></span>

<span data-ttu-id="b365d-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b365d-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b365d-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b365d-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b365d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b365d-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b365d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b365d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_user_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedUsers/$ref
Content-Type: application/json
Content-length: 46

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{userId}"
}
```
# <a name="c"></a>[<span data-ttu-id="b365d-136">C#</span><span class="sxs-lookup"><span data-stu-id="b365d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b365d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b365d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b365d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b365d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b365d-139">Java</span><span class="sxs-lookup"><span data-stu-id="b365d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b365d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b365d-140">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
}
-->
```http
HTTP/1.1 204 No Content
```

