---
title: Create taskTrigger
description: Criar um novo disparador de tarefas na impressora especificada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f3a3673e098c67ac3bf7b01a3d607e38afe95add
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035626"
---
# <a name="create-tasktrigger"></a><span data-ttu-id="07709-103">Create taskTrigger</span><span class="sxs-lookup"><span data-stu-id="07709-103">Create taskTrigger</span></span>

<span data-ttu-id="07709-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07709-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07709-105">Criar um novo [disparador de tarefas](../resources/printtasktrigger.md) na [impressora](../resources/printer.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="07709-105">Create a new [task trigger](../resources/printtasktrigger.md) on the specified [printer](../resources/printer.md).</span></span> <span data-ttu-id="07709-106">No momento, apenas **um** gatilho de tarefa pode ser especificado por impressora, mas esse limite pode ser removido no futuro.</span><span class="sxs-lookup"><span data-stu-id="07709-106">Currently, only **one** task trigger can be specified per printer, but this limit may be removed in the future.</span></span> <span data-ttu-id="07709-107">Além disso, somente o aplicativo que registrou a impressora pode gerenciar seus gatilhos de tarefa.</span><span class="sxs-lookup"><span data-stu-id="07709-107">Additionally, only the application that registered the printer can manage its task triggers.</span></span>

## <a name="permissions"></a><span data-ttu-id="07709-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="07709-108">Permissions</span></span>
<span data-ttu-id="07709-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07709-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="07709-111">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="07709-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="07709-112">O usuário conectado deve ser um [administrador da impressora](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="07709-112">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="07709-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07709-113">Permission type</span></span> | <span data-ttu-id="07709-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07709-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="07709-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07709-115">Delegated (work or school account)</span></span>| <span data-ttu-id="07709-116">Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="07709-116">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="07709-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07709-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07709-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07709-118">Not Supported.</span></span>|
|<span data-ttu-id="07709-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07709-119">Application</span></span>|<span data-ttu-id="07709-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07709-120">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07709-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07709-121">HTTP request</span></span>

```http
POST /print/printers/{id}/taskTriggers
```

## <a name="request-headers"></a><span data-ttu-id="07709-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07709-122">Request headers</span></span>
| <span data-ttu-id="07709-123">Nome</span><span class="sxs-lookup"><span data-stu-id="07709-123">Name</span></span>      |<span data-ttu-id="07709-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="07709-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="07709-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="07709-125">Authorization</span></span> | <span data-ttu-id="07709-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07709-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="07709-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="07709-128">Content-type</span></span>  | <span data-ttu-id="07709-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07709-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="07709-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07709-131">Request body</span></span>
<span data-ttu-id="07709-132">No corpo da solicitação, forneça uma representação JSON de um objeto [printTaskTrigger](../resources/printtasktrigger.md) .</span><span class="sxs-lookup"><span data-stu-id="07709-132">In the request body, supply a JSON representation of a [printTaskTrigger](../resources/printtasktrigger.md) object.</span></span> <span data-ttu-id="07709-133">Forneça uma referência a um [printTaskDefinition](../resources/printtaskdefinition.md) usando o `@odata.bind` formato, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="07709-133">Supply a reference to a [printTaskDefinition](../resources/printtaskdefinition.md) by using the `@odata.bind` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="07709-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="07709-134">Response</span></span>
<span data-ttu-id="07709-135">Se tiver êxito, este método retornará um `201 Created` código de resposta e um [printTaskTrigger](../resources/printtasktrigger.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07709-135">If successful, this method returns a `201 Created` response code and a [printTaskTrigger](../resources/printtasktrigger.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07709-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07709-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="07709-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07709-137">Request</span></span>
<span data-ttu-id="07709-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="07709-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="07709-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="07709-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="07709-140">C#</span><span class="sxs-lookup"><span data-stu-id="07709-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printer-tasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07709-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07709-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printer-tasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07709-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07709-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printer-tasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="07709-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="07709-143">Response</span></span>
<span data-ttu-id="07709-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="07709-144">The following is an example of the response.</span></span>
><span data-ttu-id="07709-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07709-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


