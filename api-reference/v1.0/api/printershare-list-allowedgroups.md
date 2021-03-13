---
title: Listar allowedGroups para printerShare
description: Recupere uma lista de grupos que tiveram acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 49555364c6ff923d746718ef37650130d85e7c30
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771565"
---
# <a name="list-allowedgroups"></a><span data-ttu-id="7b519-103">Listar allowedGroups</span><span class="sxs-lookup"><span data-stu-id="7b519-103">List allowedGroups</span></span>
<span data-ttu-id="7b519-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b519-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="7b519-105">Recupere uma lista de grupos que tiveram acesso para enviar trabalhos de impressão para a [impressora associadaShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="7b519-105">Retrieve a list of groups that have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b519-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b519-106">Permissions</span></span>
<span data-ttu-id="7b519-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b519-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7b519-109">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda acesso a [grupos de](group-list.md) lista.</span><span class="sxs-lookup"><span data-stu-id="7b519-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [List groups](group-list.md) access.</span></span> <span data-ttu-id="7b519-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="7b519-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="7b519-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b519-111">Permission type</span></span> | <span data-ttu-id="7b519-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b519-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7b519-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b519-113">Delegated (work or school account)</span></span>| <span data-ttu-id="7b519-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b519-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="7b519-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b519-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b519-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b519-116">Not Supported.</span></span>|
|<span data-ttu-id="7b519-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b519-117">Application</span></span>|<span data-ttu-id="7b519-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b519-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b519-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b519-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}/allowedGroups
```

## <a name="request-headers"></a><span data-ttu-id="7b519-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b519-120">Request headers</span></span>
|<span data-ttu-id="7b519-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7b519-121">Name</span></span>|<span data-ttu-id="7b519-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b519-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7b519-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b519-123">Authorization</span></span>|<span data-ttu-id="7b519-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b519-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b519-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b519-126">Request body</span></span>
<span data-ttu-id="7b519-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b519-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b519-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b519-128">Response</span></span>

<span data-ttu-id="7b519-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [de](../resources/group.md) grupo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b519-129">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b519-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7b519-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7b519-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b519-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7b519-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b519-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedGroups
```
# <a name="c"></a>[<span data-ttu-id="7b519-133">C#</span><span class="sxs-lookup"><span data-stu-id="7b519-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b519-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b519-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b519-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b519-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b519-136">Java</span><span class="sxs-lookup"><span data-stu-id="7b519-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7b519-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b519-137">Response</span></span>
<span data-ttu-id="7b519-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7b519-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.group)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.group)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "GroupName"
    }
  ]
}
```

