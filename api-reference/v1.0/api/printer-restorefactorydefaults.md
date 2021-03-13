---
title: 'printer: restoreFactoryDefaults'
description: Redefinir as configurações padrão de uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 68bf2f96336e6156a28cab9d42e9e5ee5971a659
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771789"
---
# <a name="printer-restorefactorydefaults"></a><span data-ttu-id="51608-103">printer: restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="51608-103">printer: restoreFactoryDefaults</span></span>
<span data-ttu-id="51608-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51608-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="51608-105">Restaure [as configurações](../resources/printer.md)padrão de uma impressora para os valores especificados pelo fabricante.</span><span class="sxs-lookup"><span data-stu-id="51608-105">Restore a [printer](../resources/printer.md)'s default settings to the values specified by the manufacturer.</span></span>

## <a name="permissions"></a><span data-ttu-id="51608-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="51608-106">Permissions</span></span>
<span data-ttu-id="51608-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51608-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="51608-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="51608-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="51608-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="51608-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="51608-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51608-111">Permission type</span></span> | <span data-ttu-id="51608-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51608-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="51608-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51608-113">Delegated (work or school account)</span></span>| <span data-ttu-id="51608-114">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="51608-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="51608-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51608-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51608-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51608-116">Not Supported.</span></span>|
|<span data-ttu-id="51608-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51608-117">Application</span></span>| <span data-ttu-id="51608-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51608-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51608-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51608-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/restoreFactoryDefaults
```

## <a name="request-headers"></a><span data-ttu-id="51608-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51608-120">Request headers</span></span>
|<span data-ttu-id="51608-121">Nome</span><span class="sxs-lookup"><span data-stu-id="51608-121">Name</span></span>|<span data-ttu-id="51608-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="51608-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="51608-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="51608-123">Authorization</span></span>|<span data-ttu-id="51608-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51608-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="51608-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51608-126">Request body</span></span>
<span data-ttu-id="51608-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51608-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51608-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="51608-128">Response</span></span>

<span data-ttu-id="51608-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51608-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51608-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="51608-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="51608-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51608-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="51608-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="51608-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer_restorefactorydefaults"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/restoreFactoryDefaults
```
# <a name="c"></a>[<span data-ttu-id="51608-134">C#</span><span class="sxs-lookup"><span data-stu-id="51608-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-restorefactorydefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51608-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51608-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-restorefactorydefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51608-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51608-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-restorefactorydefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51608-137">Java</span><span class="sxs-lookup"><span data-stu-id="51608-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-restorefactorydefaults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="51608-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="51608-138">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

