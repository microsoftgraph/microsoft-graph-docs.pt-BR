---
title: Como trabalhar com ações de execução longa (beta)
description: Este artigo descreve o trabalho com ações de execução longa.
localization_priority: Normal
author: daspek
ms.openlocfilehash: 9623dce367514d86e7dc84df672578cd2a77fad3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331998"
---
# <a name="working-with-long-running-actions-beta"></a><span data-ttu-id="8c2e4-103">Como trabalhar com ações de execução longa (beta)</span><span class="sxs-lookup"><span data-stu-id="8c2e4-103">Working with long running actions (beta)</span></span>


<span data-ttu-id="8c2e4-104">Algumas respostas de API exigem tempo indeterminado para serem concluídas.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-104">Some API responses require indeterminate time to complete.</span></span>
<span data-ttu-id="8c2e4-105">Em vez de ter que esperar até que a ação seja concluída antes de retornar uma resposta, o Microsoft Graph pode usar um padrão de ações de execução longa.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-105">Instead of waiting until the action is complete before returning a response, Microsoft Graph may use a long running actions pattern.</span></span>
<span data-ttu-id="8c2e4-106">Esse padrão fornece ao aplicativo uma espera para sondar se há atualizações de status em uma ação de execução longa, sem que qualquer solicitação aguarde até que a ação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-106">This pattern provides your app a wait to poll for status updates on a long running action, without any request waiting for the action to complete.</span></span>

<span data-ttu-id="8c2e4-107">O padrão geral segue estas etapas:</span><span class="sxs-lookup"><span data-stu-id="8c2e4-107">The general pattern follows these steps:</span></span>

1. <span data-ttu-id="8c2e4-108">O aplicativo solicita uma ação de execução longa por meio da API.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-108">Your app requests a long running action via the API.</span></span> <span data-ttu-id="8c2e4-109">A API aceita a ação e retorna uma resposta `202 Accepted` junto com um cabeçalho de Local para que a URL de API recupere relatórios de status de ação.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-109">The API accepts the action and returns a `202 Accepted` response along with a Location header for the API URL to retrieve action status reports.</span></span>
2. <span data-ttu-id="8c2e4-110">O aplicativo solicita a URL de relatório de status de ação e recebe uma resposta [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) com o progresso da ação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-110">Your app requests the action status report URL and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response with the progress of the long running action.</span></span>
3. <span data-ttu-id="8c2e4-111">A ação de execução longa é concluída.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-111">The long running action completes.</span></span> 
4. <span data-ttu-id="8c2e4-112">O aplicativo solicita a URL de relatório de status da ação novamente e recebe uma resposta [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) que mostra a conclusão da ação.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-112">Your app requests the action status report URL again and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response showing the completion of the action.</span></span>

## <a name="initial-action-request"></a><span data-ttu-id="8c2e4-113">Solicitação de ação inicial</span><span class="sxs-lookup"><span data-stu-id="8c2e4-113">Initial action request</span></span>

<span data-ttu-id="8c2e4-114">Vamos percorrer as etapas para obter um cenário de exemplo de [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="8c2e4-114">Let's walk through the steps for an example [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta) scenario.</span></span>
<span data-ttu-id="8c2e4-115">Neste cenário, o aplicativo solicita a cópia de uma pasta que contém uma grande quantidade de dados.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-115">In this scenario, your app requests to copy a folder that contains a large amount of data.</span></span>
<span data-ttu-id="8c2e4-116">Essa solicitação provavelmente levará vários segundos para ser concluída, pois a quantidade de dados é grande.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-116">This request will likely take several seconds to complete since the amount of data is large.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8c2e4-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c2e4-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "lro-copy-item-example", "scopes": "files.readwrite" } -->

```http
POST https://graph.microsoft.com/beta/me/drive/items/{folder-item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "Copy of LargeFolder1"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c2e4-118">C#</span><span class="sxs-lookup"><span data-stu-id="8c2e4-118">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/lro-copy-item-example-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c2e4-119">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c2e4-119">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/lro-copy-item-example-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c2e4-120">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8c2e4-120">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/lro-copy-item-example-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8c2e4-121">Java</span><span class="sxs-lookup"><span data-stu-id="8c2e4-121">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/lro-copy-item-example-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="8c2e4-122">A API responde que a ação foi aceita e fornece a URL para recuperar o status da ação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-122">The API responds that the action was accepted and the URL for retrieving the status of the long running action.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="8c2e4-123">**Observação:** o local da URL retornado pode não estar no ponto de extremidade da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-123">**Note:** The location URL returned may not be on the Microsoft Graph API endpoint.</span></span>

<span data-ttu-id="8c2e4-124">Em muitos casos, esse pode ser o fim da solicitação, pois a ação de cópia será concluída sem que o aplicativo realize tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-124">In many cases this may be the end of the request, since the copy action will complete without the app doing any additional work.</span></span>
<span data-ttu-id="8c2e4-125">No entanto, se o aplicativo precisar mostrar o status da ação de cópia ou garantir que ela seja concluída sem erros, poderá fazer isso usando a URL de monitor.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-125">However, if your app needs to show the status of the copy action or ensure that it completes without error, it can do so using the monitor URL.</span></span>

## <a name="retrieve-a-status-report-from-the-monitor-url"></a><span data-ttu-id="8c2e4-126">Recuperar um relatório de status da URL de monitor</span><span class="sxs-lookup"><span data-stu-id="8c2e4-126">Retrieve a status report from the monitor URL</span></span>

<span data-ttu-id="8c2e4-p105">Para verificar o status da ação de cópia, o aplicativo faz uma solicitação para a URL fornecida na resposta anterior. *Observação:* Essa solicitação não requer autenticação, pois a URL é de curta duração e exclusiva para o chamador original.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-p105">To check on the status of the copy action, the app makes a request to the URL provided in the previous response. *Note:* This request does not require authentication, since the URL is short-lived and unique to the original caller.</span></span> 

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="8c2e4-129">O serviço responde com a informação de que a ação de execução longa ainda está em andamento:</span><span class="sxs-lookup"><span data-stu-id="8c2e4-129">The service responses with information that the long running action is still in progress:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
  "operation": "ItemCopy",
  "percentageComplete": 27.8,
  "status": "inProgress"
}
```

<span data-ttu-id="8c2e4-p106">As informações podem ser usadas para fornecer uma atualização ao usuário sobre o progresso da ação de cópia. O aplicativo pode continuar a sondar a URL de monitor para solicitar atualizações de status e acompanhar o andamento da ação.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-p106">This information can be used to provide an update to the user about the progress of the copy action. The app can continue to poll the monitor URL to request status updates and keep track of the progress of the action.</span></span>

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a><span data-ttu-id="8c2e4-132">Recuperar um relatório de status concluído da URL de monitor</span><span class="sxs-lookup"><span data-stu-id="8c2e4-132">Retrieve a completed status report from the monitor URL</span></span>

<span data-ttu-id="8c2e4-p107">Após alguns segundos, a operação de cópia foi concluída. Dessa vez, quando o aplicativo faz uma solicitação para a URL de monitor, a resposta é um redirecionamento para o resultado concluído da ação.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-p107">After a few seconds the copy operation has completed. This time when the app makes a request to the monitor URL the response is a redirection to the finished result of the action.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="8c2e4-135">Após a conclusão da ação, a resposta do serviço de monitor retornará a resourceId para obter os resultados.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-135">When the action has completed, the response from the monitor service will return the resourceId for the results.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "percentageComplete": 100.0,
    "resourceId": "01MOWKYVJML57KN2ANMBA3JZJS2MBGC7KM",
    "status": "completed"
}
```

## <a name="retrieve-the-results-of-the-completed-operation"></a><span data-ttu-id="8c2e4-136">Recuperar os resultados da operação concluída</span><span class="sxs-lookup"><span data-stu-id="8c2e4-136">Retrieve the results of the completed operation</span></span>

<span data-ttu-id="8c2e4-137">Depois que o trabalho for concluído, a URL do monitor retornará o resourceId do resultado. Neste caso, trata-se da nova cópia do item original.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-137">Once the job has completed, the monitor URL returns the resourceId of the result, in this case the new copy of the original item.</span></span>
<span data-ttu-id="8c2e4-138">Você pode resolver esse novo item usando resourceId; por exemplo:</span><span class="sxs-lookup"><span data-stu-id="8c2e4-138">You can address this new item using the resourceId, for example:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8c2e4-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c2e4-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "lro-copy-item-example-complete",
  "scopes": "files.readwrite"
} -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c2e4-140">C#</span><span class="sxs-lookup"><span data-stu-id="8c2e4-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/lro-copy-item-example-complete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c2e4-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c2e4-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/lro-copy-item-example-complete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c2e4-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8c2e4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/lro-copy-item-example-complete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8c2e4-143">Java</span><span class="sxs-lookup"><span data-stu-id="8c2e4-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/lro-copy-item-example-complete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "",
    "name": "Copy of LargeFolder1",
    "folder": { },
    "size": 12019
}
```

## <a name="supported-resources"></a><span data-ttu-id="8c2e4-144">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="8c2e4-144">Supported resources</span></span>

<span data-ttu-id="8c2e4-145">Ações de execução longa têm suporte nos métodos de API a seguir</span><span class="sxs-lookup"><span data-stu-id="8c2e4-145">Long running actions are supported on the following API methods</span></span>

| <span data-ttu-id="8c2e4-146">**Recurso**</span><span class="sxs-lookup"><span data-stu-id="8c2e4-146">**Resource**</span></span> | <span data-ttu-id="8c2e4-147">**API**</span><span class="sxs-lookup"><span data-stu-id="8c2e4-147">**API**</span></span> |
|:------ | :------ |
| <span data-ttu-id="8c2e4-148">DriveItem</span><span class="sxs-lookup"><span data-stu-id="8c2e4-148">DriveItem</span></span> | [<span data-ttu-id="8c2e4-149">Copiar</span><span class="sxs-lookup"><span data-stu-id="8c2e4-149">Copy</span></span>](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a><span data-ttu-id="8c2e4-150">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c2e4-150">Prerequisites</span></span>

<span data-ttu-id="8c2e4-151">As mesmas [permissões](./permissions-reference.md) que são necessárias para realizar uma ação de execução longa também são necessárias para consultar o status de uma ação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="8c2e4-151">The same [permissions](./permissions-reference.md) that are required to perform a long running action are also required to query the status of a long running action.</span></span>




<!-- {
  "type": "#page.annotation",
  "description": "Monitor the progress of long-running actions in the API.",
  "keywords": "monitor,long,running,operation,action",
  "section": "documentation",
  "suppressions": [
    "Error: lro-check-status:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus",
    "Error: lro-check-status-complete:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus"
  ],
  "tocPath": "Concepts/Long running actions"
} -->
