---
title: Listar allowedUsers for printerShare
description: Recupere uma lista de usuários que tiveram acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: d1f55d9d4ae91d6ae41ee4656fbb1e90b7948304
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771530"
---
# <a name="list-allowedusers"></a><span data-ttu-id="547f8-103">Listar allowedUsers</span><span class="sxs-lookup"><span data-stu-id="547f8-103">List allowedUsers</span></span>
<span data-ttu-id="547f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="547f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="547f8-105">Recupere uma lista de usuários que tiveram acesso para enviar trabalhos de impressão para a [impressora associadaShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="547f8-105">Retrieve a list of users who have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="547f8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="547f8-106">Permissions</span></span>
<span data-ttu-id="547f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="547f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="547f8-109">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda acesso aos usuários [de](user-list.md) lista.</span><span class="sxs-lookup"><span data-stu-id="547f8-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [List users](user-list.md) access.</span></span> <span data-ttu-id="547f8-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="547f8-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="547f8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="547f8-111">Permission type</span></span> | <span data-ttu-id="547f8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="547f8-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="547f8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="547f8-113">Delegated (work or school account)</span></span>| <span data-ttu-id="547f8-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="547f8-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="547f8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="547f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="547f8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="547f8-116">Not Supported.</span></span>|
|<span data-ttu-id="547f8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="547f8-117">Application</span></span>|<span data-ttu-id="547f8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="547f8-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="547f8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="547f8-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}/allowedUsers
```

## <a name="request-headers"></a><span data-ttu-id="547f8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="547f8-120">Request headers</span></span>
|<span data-ttu-id="547f8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="547f8-121">Name</span></span>|<span data-ttu-id="547f8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="547f8-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="547f8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="547f8-123">Authorization</span></span>|<span data-ttu-id="547f8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="547f8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="547f8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="547f8-126">Request body</span></span>
<span data-ttu-id="547f8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="547f8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="547f8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="547f8-128">Response</span></span>

<span data-ttu-id="547f8-129">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="547f8-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="547f8-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="547f8-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="547f8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="547f8-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="547f8-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="547f8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_user"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedUsers
```
# <a name="c"></a>[<span data-ttu-id="547f8-133">C#</span><span class="sxs-lookup"><span data-stu-id="547f8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="547f8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="547f8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="547f8-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="547f8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="547f8-136">Java</span><span class="sxs-lookup"><span data-stu-id="547f8-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="547f8-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="547f8-137">Response</span></span>
<span data-ttu-id="547f8-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="547f8-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.user)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.user)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "UserName",
      "userPrincipalName": "username@contoso.com"
    }
  ]
}
```

