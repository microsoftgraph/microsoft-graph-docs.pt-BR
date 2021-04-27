---
title: Create taskTrigger
description: Crie um novo gatilho de tarefas na impressora especificada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: cd654963b8aa5dc5ce30c2fadc644fb3aaa03568
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052023"
---
# <a name="create-tasktrigger"></a><span data-ttu-id="01851-103">Create taskTrigger</span><span class="sxs-lookup"><span data-stu-id="01851-103">Create taskTrigger</span></span>

<span data-ttu-id="01851-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01851-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01851-105">Crie um novo [gatilho de tarefas](../resources/printtasktrigger.md) na impressora [especificada.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="01851-105">Create a new [task trigger](../resources/printtasktrigger.md) on the specified [printer](../resources/printer.md).</span></span> <span data-ttu-id="01851-106">Atualmente, apenas **um gatilho** de tarefa pode ser especificado por impressora, mas esse limite pode ser removido no futuro.</span><span class="sxs-lookup"><span data-stu-id="01851-106">Currently, only **one** task trigger can be specified per printer, but this limit may be removed in the future.</span></span> 

## <a name="permissions"></a><span data-ttu-id="01851-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="01851-107">Permissions</span></span>
<span data-ttu-id="01851-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01851-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="01851-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="01851-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="01851-111">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="01851-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="01851-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01851-112">Permission type</span></span> | <span data-ttu-id="01851-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01851-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="01851-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01851-114">Delegated (work or school account)</span></span>| <span data-ttu-id="01851-115">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="01851-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="01851-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01851-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01851-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01851-117">Not Supported.</span></span>|
|<span data-ttu-id="01851-118">Application</span><span class="sxs-lookup"><span data-stu-id="01851-118">Application</span></span>|<span data-ttu-id="01851-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01851-119">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01851-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01851-120">HTTP request</span></span>

```http
POST /print/printers/{id}/taskTriggers
```

## <a name="request-headers"></a><span data-ttu-id="01851-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01851-121">Request headers</span></span>
| <span data-ttu-id="01851-122">Nome</span><span class="sxs-lookup"><span data-stu-id="01851-122">Name</span></span>      |<span data-ttu-id="01851-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="01851-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="01851-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="01851-124">Authorization</span></span> | <span data-ttu-id="01851-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01851-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01851-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="01851-127">Content-type</span></span>  | <span data-ttu-id="01851-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01851-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01851-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01851-130">Request body</span></span>
<span data-ttu-id="01851-131">No corpo da solicitação, fornece uma representação JSON de um [objeto printTaskTrigger.](../resources/printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="01851-131">In the request body, supply a JSON representation of a [printTaskTrigger](../resources/printtasktrigger.md) object.</span></span> <span data-ttu-id="01851-132">Fornecer uma referência a [uma printTaskDefinition](../resources/printtaskdefinition.md) usando o formato, conforme `@odata.bind` mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="01851-132">Supply a reference to a [printTaskDefinition](../resources/printtaskdefinition.md) by using the `@odata.bind` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="01851-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="01851-133">Response</span></span>
<span data-ttu-id="01851-134">Se tiver êxito, este método retornará um código `201 Created` de resposta e um [printTaskTrigger](../resources/printtasktrigger.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01851-134">If successful, this method returns a `201 Created` response code and a [printTaskTrigger](../resources/printtasktrigger.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01851-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01851-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="01851-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01851-136">Request</span></span>
<span data-ttu-id="01851-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01851-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="01851-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="01851-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printer_tasktrigger"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/ae63f617-4856-4b45-8ea9-69dfbeea230e/taskTriggers

{
  "event": "jobStarted",
  "definition@odata.bind": "https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c"
}
```
# <a name="c"></a>[<span data-ttu-id="01851-139">C#</span><span class="sxs-lookup"><span data-stu-id="01851-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printer-tasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01851-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01851-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printer-tasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01851-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01851-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printer-tasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01851-142">Java</span><span class="sxs-lookup"><span data-stu-id="01851-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printer-tasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="01851-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="01851-143">Response</span></span>
<span data-ttu-id="01851-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01851-144">The following is an example of the response.</span></span>
><span data-ttu-id="01851-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="01851-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 196

{
  "@odata.context": "https://graph.print.microsoft.com/v1.0/$metadata#Collection(Microsoft.Graph.PrintTaskTrigger)",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```
