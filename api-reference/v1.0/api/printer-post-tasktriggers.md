---
title: Criar printTaskTrigger
description: Crie um novo gatilho de tarefas na impressora especificada.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: e02a2b0ce73d11153a0f778f9b0eeb80d505421b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517069"
---
# <a name="create-printtasktrigger"></a><span data-ttu-id="aa101-103">Criar printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="aa101-103">Create printTaskTrigger</span></span>
<span data-ttu-id="aa101-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa101-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="aa101-105">Crie um novo [gatilho de tarefas](../resources/printtasktrigger.md) na impressora [especificada.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="aa101-105">Create a new [task trigger](../resources/printtasktrigger.md) on the specified [printer](../resources/printer.md).</span></span> <span data-ttu-id="aa101-106">Atualmente, apenas **um gatilho** de tarefa pode ser especificado por impressora, mas esse limite pode ser removido no futuro.</span><span class="sxs-lookup"><span data-stu-id="aa101-106">Currently, only **one** task trigger can be specified per printer, but this limit may be removed in the future.</span></span> 

## <a name="permissions"></a><span data-ttu-id="aa101-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa101-107">Permissions</span></span>
<span data-ttu-id="aa101-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa101-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="aa101-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="aa101-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="aa101-111">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="aa101-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="aa101-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa101-112">Permission type</span></span> | <span data-ttu-id="aa101-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa101-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="aa101-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa101-114">Delegated (work or school account)</span></span>| <span data-ttu-id="aa101-115">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="aa101-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="aa101-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa101-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa101-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa101-117">Not Supported.</span></span>|
|<span data-ttu-id="aa101-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa101-118">Application</span></span>|<span data-ttu-id="aa101-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa101-119">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa101-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa101-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/taskTriggers
```

## <a name="request-headers"></a><span data-ttu-id="aa101-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa101-121">Request headers</span></span>
|<span data-ttu-id="aa101-122">Nome</span><span class="sxs-lookup"><span data-stu-id="aa101-122">Name</span></span>|<span data-ttu-id="aa101-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa101-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="aa101-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa101-124">Authorization</span></span>|<span data-ttu-id="aa101-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa101-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="aa101-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aa101-127">Content-Type</span></span>|<span data-ttu-id="aa101-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa101-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa101-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa101-130">Request body</span></span>
<span data-ttu-id="aa101-131">No corpo da solicitação, fornece uma representação JSON de um [objeto printTaskTrigger.](../resources/printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="aa101-131">In the request body, supply a JSON representation of a [printTaskTrigger](../resources/printtasktrigger.md) object.</span></span> <span data-ttu-id="aa101-132">Fornecer uma referência a [uma printTaskDefinition](../resources/printtaskdefinition.md) usando o formato, conforme `@odata.bind` mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="aa101-132">Supply a reference to a [printTaskDefinition](../resources/printtaskdefinition.md) by using the `@odata.bind` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="aa101-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa101-133">Response</span></span>
<span data-ttu-id="aa101-134">Se tiver êxito, este método retornará um código `201 Created` de resposta e um [printTaskTrigger](../resources/printtasktrigger.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa101-134">If successful, this method returns a `201 Created` response code and a [printTaskTrigger](../resources/printtasktrigger.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aa101-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="aa101-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aa101-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa101-136">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="aa101-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa101-137">Response</span></span>
<span data-ttu-id="aa101-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="aa101-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

