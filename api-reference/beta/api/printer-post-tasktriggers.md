---
title: Criar taskTrigger
description: Criar um novo disparador de tarefas na impressora especificada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 453759faf24ac5c116e3f1d9bf73aa7771aae595
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091591"
---
# <a name="create-tasktrigger"></a><span data-ttu-id="20213-103">Criar taskTrigger</span><span class="sxs-lookup"><span data-stu-id="20213-103">Create taskTrigger</span></span>

<span data-ttu-id="20213-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20213-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20213-105">Criar um novo [disparador de tarefas](../resources/printtasktrigger.md) na [impressora](../resources/printer.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="20213-105">Create a new [task trigger](../resources/printtasktrigger.md) on the specified [printer](../resources/printer.md).</span></span> <span data-ttu-id="20213-106">No momento, apenas **um** gatilho de tarefa pode ser especificado por impressora, mas esse limite pode ser removido no futuro.</span><span class="sxs-lookup"><span data-stu-id="20213-106">Currently, only **one** task trigger can be specified per printer, but this limit may be removed in the future.</span></span> <span data-ttu-id="20213-107">Além disso, somente o aplicativo que registrou a impressora pode gerenciar seus gatilhos de tarefa.</span><span class="sxs-lookup"><span data-stu-id="20213-107">Additionally, only the application that registered the printer can manage its task triggers.</span></span>

## <a name="permissions"></a><span data-ttu-id="20213-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="20213-108">Permissions</span></span>
<span data-ttu-id="20213-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20213-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="20213-111">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="20213-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="20213-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20213-112">Permission type</span></span> | <span data-ttu-id="20213-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20213-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="20213-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20213-114">Delegated (work or school account)</span></span>| <span data-ttu-id="20213-115">Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="20213-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="20213-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20213-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20213-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20213-117">Not Supported.</span></span>|
|<span data-ttu-id="20213-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20213-118">Application</span></span>|<span data-ttu-id="20213-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20213-119">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20213-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20213-120">HTTP request</span></span>

```http
POST /print/printers/{id}/taskTriggers
```

## <a name="request-headers"></a><span data-ttu-id="20213-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20213-121">Request headers</span></span>
| <span data-ttu-id="20213-122">Nome</span><span class="sxs-lookup"><span data-stu-id="20213-122">Name</span></span>      |<span data-ttu-id="20213-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="20213-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20213-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="20213-124">Authorization</span></span> | <span data-ttu-id="20213-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20213-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20213-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="20213-127">Content-type</span></span>  | <span data-ttu-id="20213-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20213-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20213-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20213-130">Request body</span></span>
<span data-ttu-id="20213-131">No corpo da solicitação, forneça uma representação JSON de um objeto [printTaskTrigger](../resources/printtasktrigger.md) .</span><span class="sxs-lookup"><span data-stu-id="20213-131">In the request body, supply a JSON representation of a [printTaskTrigger](../resources/printtasktrigger.md) object.</span></span> <span data-ttu-id="20213-132">Forneça uma referência a um [printTaskDefinition](../resources/printtaskdefinition.md) usando o `@odata.bind` formato, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="20213-132">Supply a reference to a [printTaskDefinition](../resources/printtaskdefinition.md) by using the `@odata.bind` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="20213-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="20213-133">Response</span></span>
<span data-ttu-id="20213-134">Se tiver êxito, este método retornará um `201 Created` código de resposta e um [printTaskTrigger](../resources/printtasktrigger.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20213-134">If successful, this method returns a `201 Created` response code and a [printTaskTrigger](../resources/printtasktrigger.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20213-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20213-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="20213-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20213-136">Request</span></span>
<span data-ttu-id="20213-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="20213-137">The following is an example of the request.</span></span>

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

---

### <a name="response"></a><span data-ttu-id="20213-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="20213-138">Response</span></span>
<span data-ttu-id="20213-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20213-139">The following is an example of the response.</span></span>
><span data-ttu-id="20213-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20213-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
