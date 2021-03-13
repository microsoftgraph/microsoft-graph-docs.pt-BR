---
title: Eliminar impressora
description: Excluir (não registro) uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 94841d1668363ffeb98d8416527c06d53bb7c517
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776925"
---
# <a name="delete-printer"></a><span data-ttu-id="8e855-103">Eliminar impressora</span><span class="sxs-lookup"><span data-stu-id="8e855-103">Delete printer</span></span>
<span data-ttu-id="8e855-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e855-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="8e855-105">Excluir (não registro) uma [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="8e855-105">Delete (unregister) a [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e855-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8e855-106">Permissions</span></span>
<span data-ttu-id="8e855-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e855-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8e855-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="8e855-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="8e855-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="8e855-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="8e855-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e855-111">Permission type</span></span> | <span data-ttu-id="8e855-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e855-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8e855-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e855-113">Delegated (work or school account)</span></span>| <span data-ttu-id="8e855-114">Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="8e855-114">Printer.FullControl.All</span></span> |
|<span data-ttu-id="8e855-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e855-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e855-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e855-116">Not Supported.</span></span>|
|<span data-ttu-id="8e855-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e855-117">Application</span></span>|<span data-ttu-id="8e855-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e855-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e855-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e855-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/printers/{printerId}
```

## <a name="request-headers"></a><span data-ttu-id="8e855-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e855-120">Request headers</span></span>
|<span data-ttu-id="8e855-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8e855-121">Name</span></span>|<span data-ttu-id="8e855-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e855-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8e855-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e855-123">Authorization</span></span>|<span data-ttu-id="8e855-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e855-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e855-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e855-126">Request body</span></span>
<span data-ttu-id="8e855-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e855-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e855-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e855-128">Response</span></span>

<span data-ttu-id="8e855-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8e855-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8e855-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8e855-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8e855-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e855-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8e855-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e855-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printer"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/printers/{printerId}
```
# <a name="c"></a>[<span data-ttu-id="8e855-133">C#</span><span class="sxs-lookup"><span data-stu-id="8e855-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e855-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e855-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e855-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e855-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e855-136">Java</span><span class="sxs-lookup"><span data-stu-id="8e855-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8e855-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e855-137">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

