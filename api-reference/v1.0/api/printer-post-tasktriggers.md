---
title: Criar printTaskTrigger
description: Crie um novo gatilho de tarefas na impressora especificada.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 3ed74256934310df5f5ea99217f8f0956e109eda
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771831"
---
# <a name="create-printtasktrigger"></a><span data-ttu-id="8f800-103">Criar printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="8f800-103">Create printTaskTrigger</span></span>
<span data-ttu-id="8f800-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f800-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="8f800-105">Crie um novo [gatilho de tarefas](../resources/printtasktrigger.md) na impressora [especificada.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="8f800-105">Create a new [task trigger](../resources/printtasktrigger.md) on the specified [printer](../resources/printer.md).</span></span> <span data-ttu-id="8f800-106">Atualmente, apenas **um gatilho** de tarefa pode ser especificado por impressora, mas esse limite pode ser removido no futuro.</span><span class="sxs-lookup"><span data-stu-id="8f800-106">Currently, only **one** task trigger can be specified per printer, but this limit may be removed in the future.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8f800-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8f800-107">Permissions</span></span>
<span data-ttu-id="8f800-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f800-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8f800-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="8f800-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="8f800-111">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="8f800-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="8f800-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f800-112">Permission type</span></span> | <span data-ttu-id="8f800-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f800-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8f800-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f800-114">Delegated (work or school account)</span></span>| <span data-ttu-id="8f800-115">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="8f800-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="8f800-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f800-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f800-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f800-117">Not Supported.</span></span>|
|<span data-ttu-id="8f800-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f800-118">Application</span></span>|<span data-ttu-id="8f800-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f800-119">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f800-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f800-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/taskTriggers
```

## <a name="request-headers"></a><span data-ttu-id="8f800-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f800-121">Request headers</span></span>
|<span data-ttu-id="8f800-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8f800-122">Name</span></span>|<span data-ttu-id="8f800-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f800-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8f800-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f800-124">Authorization</span></span>|<span data-ttu-id="8f800-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f800-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8f800-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f800-127">Content-Type</span></span>|<span data-ttu-id="8f800-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f800-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f800-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f800-130">Request body</span></span>
<span data-ttu-id="8f800-131">No corpo da solicitação, fornece uma representação JSON de um [objeto printTaskTrigger.](../resources/printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="8f800-131">In the request body, supply a JSON representation of a [printTaskTrigger](../resources/printtasktrigger.md) object.</span></span> <span data-ttu-id="8f800-132">Fornecer uma referência a [uma printTaskDefinition](../resources/printtaskdefinition.md) usando o formato, conforme `@odata.bind` mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="8f800-132">Supply a reference to a [printTaskDefinition](../resources/printtaskdefinition.md) by using the `@odata.bind` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="8f800-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f800-133">Response</span></span>
<span data-ttu-id="8f800-134">Se tiver êxito, este método retornará um código `201 Created` de resposta e um [printTaskTrigger](../resources/printtasktrigger.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f800-134">If successful, this method returns a `201 Created` response code and a [printTaskTrigger](../resources/printtasktrigger.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f800-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8f800-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f800-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f800-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8f800-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f800-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printtasktrigger_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers
Content-Type: application/json
Content-length: 80

{
  "event": "jobStarted",
  "definition@odata.bind": "https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}"
}
```
# <a name="c"></a>[<span data-ttu-id="8f800-138">C#</span><span class="sxs-lookup"><span data-stu-id="8f800-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printtasktrigger-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f800-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f800-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printtasktrigger-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f800-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f800-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printtasktrigger-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f800-141">Java</span><span class="sxs-lookup"><span data-stu-id="8f800-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printtasktrigger-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8f800-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f800-142">Response</span></span>
<span data-ttu-id="8f800-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8f800-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.print.microsoft.com/v1.0/$metadata#Collection(Microsoft.Graph.PrintTaskTrigger)",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```

