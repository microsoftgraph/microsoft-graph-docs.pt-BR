---
title: Como trabalhar com ações de execução longa (beta)
description: Este artigo descreve o trabalho com ações de execução longa.
localization_priority: Normal
author: daspek
ms.openlocfilehash: 0403dd8e099a5f21f3b1da7cf74859b664eefa43
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277767"
---
# <a name="working-with-long-running-actions-beta"></a><span data-ttu-id="57cc2-103">Como trabalhar com ações de execução longa (beta)</span><span class="sxs-lookup"><span data-stu-id="57cc2-103">Working with long running actions (beta)</span></span>


<span data-ttu-id="57cc2-104">Algumas respostas de API exigem tempo indeterminado para serem concluídas.</span><span class="sxs-lookup"><span data-stu-id="57cc2-104">Some API responses require indeterminate time to complete.</span></span>
<span data-ttu-id="57cc2-105">Em vez de ter que esperar até que a ação seja concluída antes de retornar uma resposta, o Microsoft Graph pode usar um padrão de ações de execução longa.</span><span class="sxs-lookup"><span data-stu-id="57cc2-105">Instead of waiting until the action is complete before returning a response, Microsoft Graph may use a long running actions pattern.</span></span>
<span data-ttu-id="57cc2-106">Esse padrão fornece ao aplicativo uma espera para sondar se há atualizações de status em uma ação de execução longa, sem que qualquer solicitação aguarde até que a ação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="57cc2-106">This pattern provides your app a wait to poll for status updates on a long running action, without any request waiting for the action to complete.</span></span>

<span data-ttu-id="57cc2-107">O padrão geral segue estas etapas:</span><span class="sxs-lookup"><span data-stu-id="57cc2-107">The general pattern follows these steps:</span></span>

1. <span data-ttu-id="57cc2-108">O aplicativo solicita uma ação de execução longa por meio da API.</span><span class="sxs-lookup"><span data-stu-id="57cc2-108">Your app requests a long running action via the API.</span></span> <span data-ttu-id="57cc2-109">A API aceita a ação e retorna uma resposta `202 Accepted` junto com um cabeçalho de Local para que a URL de API recupere relatórios de status de ação.</span><span class="sxs-lookup"><span data-stu-id="57cc2-109">The API accepts the action and returns a `202 Accepted` response along with a Location header for the API URL to retrieve action status reports.</span></span>
2. <span data-ttu-id="57cc2-110">O aplicativo solicita a URL de relatório de status de ação e recebe uma resposta [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) com o progresso da ação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="57cc2-110">Your app requests the action status report URL and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response with the progress of the long running action.</span></span>
3. <span data-ttu-id="57cc2-111">A ação de execução longa é concluída.</span><span class="sxs-lookup"><span data-stu-id="57cc2-111">The long running action completes.</span></span> 
4. <span data-ttu-id="57cc2-112">O aplicativo solicita a URL de relatório de status da ação novamente e recebe uma resposta [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) que mostra a conclusão da ação.</span><span class="sxs-lookup"><span data-stu-id="57cc2-112">Your app requests the action status report URL again and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response showing the completion of the action.</span></span>

## <a name="initial-action-request"></a><span data-ttu-id="57cc2-113">Solicitação de ação inicial</span><span class="sxs-lookup"><span data-stu-id="57cc2-113">Initial action request</span></span>

<span data-ttu-id="57cc2-114">Vamos percorrer as etapas para obter um cenário de exemplo de [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="57cc2-114">Let's walk through the steps for an example [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta) scenario.</span></span>
<span data-ttu-id="57cc2-115">Neste cenário, o aplicativo solicita a cópia de uma pasta que contém uma grande quantidade de dados.</span><span class="sxs-lookup"><span data-stu-id="57cc2-115">In this scenario, your app requests to copy a folder that contains a large amount of data.</span></span>
<span data-ttu-id="57cc2-116">Essa solicitação provavelmente levará vários segundos para ser concluída, pois a quantidade de dados é grande.</span><span class="sxs-lookup"><span data-stu-id="57cc2-116">This request will likely take several seconds to complete since the amount of data is large.</span></span>

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

<span data-ttu-id="57cc2-117">A API responde que a ação foi aceita e fornece a URL para recuperar o status da ação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="57cc2-117">The API responds that the action was accepted and the URL for retrieving the status of the long running action.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="57cc2-118">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="57cc2-118">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="57cc2-119">C#</span><span class="sxs-lookup"><span data-stu-id="57cc2-119">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57cc2-120">Javascript</span><span class="sxs-lookup"><span data-stu-id="57cc2-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="57cc2-121">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="57cc2-121">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="57cc2-122">**Observação:** o local da URL retornado pode não estar no ponto de extremidade da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="57cc2-122">**Note:** The location URL returned may not be on the Microsoft Graph API endpoint.</span></span>

<span data-ttu-id="57cc2-123">Em muitos casos, esse pode ser o fim da solicitação, pois a ação de cópia será concluída sem que o aplicativo realize tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="57cc2-123">In many cases this may be the end of the request, since the copy action will complete without the app doing any additional work.</span></span>
<span data-ttu-id="57cc2-124">No entanto, se o aplicativo precisar mostrar o status da ação de cópia ou garantir que ela seja concluída sem erros, poderá fazer isso usando a URL de monitor.</span><span class="sxs-lookup"><span data-stu-id="57cc2-124">However, if your app needs to show the status of the copy action or ensure that it completes without error, it can do so using the monitor URL.</span></span>

## <a name="retrieve-a-status-report-from-the-monitor-url"></a><span data-ttu-id="57cc2-125">Recuperar um relatório de status da URL de monitor</span><span class="sxs-lookup"><span data-stu-id="57cc2-125">Retrieve a status report from the monitor URL</span></span>

<span data-ttu-id="57cc2-p105">Para verificar o status da ação de cópia, o aplicativo faz uma solicitação para a URL fornecida na resposta anterior. *Observação:* Essa solicitação não requer autenticação, pois a URL é de curta duração e exclusiva para o chamador original.</span><span class="sxs-lookup"><span data-stu-id="57cc2-p105">To check on the status of the copy action, the app makes a request to the URL provided in the previous response. *Note:* This request does not require authentication, since the URL is short-lived and unique to the original caller.</span></span> 

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="57cc2-128">O serviço responde com a informação de que a ação de execução longa ainda está em andamento:</span><span class="sxs-lookup"><span data-stu-id="57cc2-128">The service responses with information that the long running action is still in progress:</span></span>

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

<span data-ttu-id="57cc2-p106">As informações podem ser usadas para fornecer uma atualização ao usuário sobre o progresso da ação de cópia. O aplicativo pode continuar a sondar a URL de monitor para solicitar atualizações de status e acompanhar o andamento da ação.</span><span class="sxs-lookup"><span data-stu-id="57cc2-p106">This information can be used to provide an update to the user about the progress of the copy action. The app can continue to poll the monitor URL to request status updates and keep track of the progress of the action.</span></span>

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a><span data-ttu-id="57cc2-131">Recuperar um relatório de status concluído da URL de monitor</span><span class="sxs-lookup"><span data-stu-id="57cc2-131">Retrieve a completed status report from the monitor URL</span></span>

<span data-ttu-id="57cc2-p107">Após alguns segundos, a operação de cópia foi concluída. Dessa vez, quando o aplicativo faz uma solicitação para a URL de monitor, a resposta é um redirecionamento para o resultado concluído da ação.</span><span class="sxs-lookup"><span data-stu-id="57cc2-p107">After a few seconds the copy operation has completed. This time when the app makes a request to the monitor URL the response is a redirection to the finished result of the action.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="57cc2-134">Após a conclusão da ação, a resposta do serviço de monitor retornará a resourceId para obter os resultados.</span><span class="sxs-lookup"><span data-stu-id="57cc2-134">When the action has completed, the response from the monitor service will return the resourceId for the results.</span></span>

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

## <a name="retrieve-the-results-of-the-completed-operation"></a><span data-ttu-id="57cc2-135">Recuperar os resultados da operação concluída</span><span class="sxs-lookup"><span data-stu-id="57cc2-135">Retrieve the results of the completed operation</span></span>

<span data-ttu-id="57cc2-136">Depois que o trabalho for concluído, a URL do monitor retornará o resourceId do resultado. Neste caso, trata-se da nova cópia do item original.</span><span class="sxs-lookup"><span data-stu-id="57cc2-136">Once the job has completed, the monitor URL returns the resourceId of the result, in this case the new copy of the original item.</span></span>
<span data-ttu-id="57cc2-137">Você pode resolver esse novo item usando resourceId; por exemplo:</span><span class="sxs-lookup"><span data-stu-id="57cc2-137">You can address this new item using the resourceId, for example:</span></span>

<!-- {
  "blockType": "request",
  "name": "lro-copy-item-example-complete",
  "scopes": "files.readwrite"
} -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}
```

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="57cc2-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="57cc2-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="57cc2-139">C#</span><span class="sxs-lookup"><span data-stu-id="57cc2-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-complete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57cc2-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="57cc2-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-complete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="57cc2-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="57cc2-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-complete-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="supported-resources"></a><span data-ttu-id="57cc2-142">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="57cc2-142">Supported resources</span></span>

<span data-ttu-id="57cc2-143">Ações de execução longa têm suporte nos métodos de API a seguir</span><span class="sxs-lookup"><span data-stu-id="57cc2-143">Long running actions are supported on the following API methods</span></span>

| <span data-ttu-id="57cc2-144">**Recurso**</span><span class="sxs-lookup"><span data-stu-id="57cc2-144">**Resource**</span></span> | <span data-ttu-id="57cc2-145">**API**</span><span class="sxs-lookup"><span data-stu-id="57cc2-145">**API**</span></span> |
|:------ | :------ |
| <span data-ttu-id="57cc2-146">DriveItem</span><span class="sxs-lookup"><span data-stu-id="57cc2-146">DriveItem</span></span> | [<span data-ttu-id="57cc2-147">Copiar</span><span class="sxs-lookup"><span data-stu-id="57cc2-147">Copy</span></span>](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a><span data-ttu-id="57cc2-148">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57cc2-148">Prerequisites</span></span>

<span data-ttu-id="57cc2-149">As mesmas [permissões](./permissions-reference.md) que são necessárias para realizar uma ação de execução longa também são necessárias para consultar o status de uma ação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="57cc2-149">The same [permissions](./permissions-reference.md) that are required to perform a long running action are also required to query the status of a long running action.</span></span>




<!-- {
  "type": "#page.annotation",
  "description": "Monitor the progress of long-running actions in the API.",
  "keywords": "monitor,long,running,operation,action",
  "section": "documentation",
  "suppressions": [
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: lro-check-status:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus",
    "Error: lro-check-status-complete:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus"
  ],
  "tocPath": "Concepts/Long running actions"
} -->
