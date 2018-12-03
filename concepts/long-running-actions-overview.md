---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
ms.topic: conceptual
ms.openlocfilehash: 687ed04d3ddcede391e9f16a2046cb186a093323
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091592"
---
# <a name="working-with-long-running-actions-beta"></a><span data-ttu-id="0d517-101">Como trabalhar com ações de execução longa (beta)</span><span class="sxs-lookup"><span data-stu-id="0d517-101">Working with long running actions (beta)</span></span>

> <span data-ttu-id="0d517-102">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0d517-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d517-103">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0d517-103">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d517-104">Algumas respostas de API exigem tempo indeterminado para serem concluídas.</span><span class="sxs-lookup"><span data-stu-id="0d517-104">Some API responses require indeterminate time to complete.</span></span>
<span data-ttu-id="0d517-105">Em vez de ter que esperar até que a ação seja concluída antes de retornar uma resposta, o Microsoft Graph pode usar um padrão de ações de execução longa.</span><span class="sxs-lookup"><span data-stu-id="0d517-105">Instead of waiting until the action is complete before returning a response, Microsoft Graph may use a long running actions pattern.</span></span>
<span data-ttu-id="0d517-106">Esse padrão fornece ao aplicativo uma espera para sondar se há atualizações de status em uma ação de execução longa, sem que qualquer solicitação aguarde até que a ação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="0d517-106">This pattern provides your app a wait to poll for status updates on a long running action, without any request waiting for the action to complete.</span></span>

<span data-ttu-id="0d517-107">O padrão geral segue estas etapas:</span><span class="sxs-lookup"><span data-stu-id="0d517-107">The general pattern follows these steps:</span></span>

1. <span data-ttu-id="0d517-108">O aplicativo solicita uma ação de execução longa por meio da API.</span><span class="sxs-lookup"><span data-stu-id="0d517-108">Your app requests a long running action via the API.</span></span> <span data-ttu-id="0d517-109">A API aceita a ação e retorna uma resposta `202 Accepted` junto com um cabeçalho de Local para que a URL de API recupere relatórios de status de ação.</span><span class="sxs-lookup"><span data-stu-id="0d517-109">The API accepts the action and returns a `202 Accepted` response along with a Location header for the API URL to retrieve action status reports.</span></span>
2. <span data-ttu-id="0d517-110">O aplicativo solicita a URL de relatório de status de ação e recebe uma resposta [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) com o progresso da ação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="0d517-110">Your app requests the action status report URL and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response with the progress of the long running action.</span></span>
3. <span data-ttu-id="0d517-111">A ação de execução longa é concluída.</span><span class="sxs-lookup"><span data-stu-id="0d517-111">The long running action completes.</span></span> 
4. <span data-ttu-id="0d517-112">O aplicativo solicita a URL de relatório de status da ação novamente e recebe uma resposta [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) que mostra a conclusão da ação.</span><span class="sxs-lookup"><span data-stu-id="0d517-112">Your app requests the action status report URL again and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response showing the completion of the action.</span></span>

## <a name="initial-action-request"></a><span data-ttu-id="0d517-113">Solicitação de ação inicial</span><span class="sxs-lookup"><span data-stu-id="0d517-113">Initial action request</span></span>

<span data-ttu-id="0d517-114">Vamos percorrer as etapas para obter um cenário de exemplo de [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="0d517-114">Let's walk through the steps for an example [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta) scenario.</span></span>
<span data-ttu-id="0d517-115">Neste cenário, o aplicativo solicita a cópia de uma pasta que contém uma grande quantidade de dados.</span><span class="sxs-lookup"><span data-stu-id="0d517-115">In this scenario, your app requests to copy a folder that contains a large amount of data.</span></span>
<span data-ttu-id="0d517-116">Essa solicitação provavelmente levará vários segundos para ser concluída, pois a quantidade de dados é grande.</span><span class="sxs-lookup"><span data-stu-id="0d517-116">This request will likely take several seconds to complete since the amount of data is large.</span></span>

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

<span data-ttu-id="0d517-117">A API responde que a ação foi aceita e fornece a URL para recuperar o status da ação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="0d517-117">The API responds that the action was accepted and the URL for retrieving the status of the long running action.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="0d517-118">**Observação:** o local da URL retornado pode não estar no ponto de extremidade da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0d517-118">**Note:** The location URL returned may not be on the Microsoft Graph API endpoint.</span></span>

<span data-ttu-id="0d517-119">Em muitos casos, esse pode ser o fim da solicitação, pois a ação de cópia será concluída sem que o aplicativo realize tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="0d517-119">In many cases this may be the end of the request, since the copy action will complete without the app doing any additional work.</span></span>
<span data-ttu-id="0d517-120">No entanto, se o aplicativo precisar mostrar o status da ação de cópia ou garantir que ela seja concluída sem erros, poderá fazer isso usando a URL de monitor.</span><span class="sxs-lookup"><span data-stu-id="0d517-120">However, if your app needs to show the status of the copy action or ensure that it completes without error, it can do so using the monitor URL.</span></span>

## <a name="retrieve-a-status-report-from-the-monitor-url"></a><span data-ttu-id="0d517-121">Recuperar um relatório de status da URL de monitor</span><span class="sxs-lookup"><span data-stu-id="0d517-121">Retrieve a status report from the monitor URL</span></span>

<span data-ttu-id="0d517-122">Para verificar o status da ação de cópia, o aplicativo faz uma solicitação para a URL fornecida na resposta anterior.</span><span class="sxs-lookup"><span data-stu-id="0d517-122">To check on the status of the copy action, the app makes a request to the URL provided in the previous response.</span></span>
<span data-ttu-id="0d517-123">*Observação:* Essa solicitação não requer autenticação, pois a URL é de curta duração e exclusiva para o chamador original.</span><span class="sxs-lookup"><span data-stu-id="0d517-123">*Note:* This request does not require authentication, since the URL is short-lived and unique to the original caller.</span></span> 

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="0d517-124">O serviço responde com a informação de que a ação de execução longa ainda está em andamento:</span><span class="sxs-lookup"><span data-stu-id="0d517-124">The service responses with information that the long running action is still in progress:</span></span>

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

<span data-ttu-id="0d517-125">As informações podem ser usadas para fornecer uma atualização ao usuário sobre o progresso da ação de cópia.</span><span class="sxs-lookup"><span data-stu-id="0d517-125">This information can be used to provide an update to the user about the progress of the copy action.</span></span>
<span data-ttu-id="0d517-126">O aplicativo pode continuar a sondar a URL de monitor para solicitar atualizações de status e acompanhar o andamento da ação.</span><span class="sxs-lookup"><span data-stu-id="0d517-126">The app can continue to poll the monitor URL to request status updates and keep track of the progress of the action.</span></span>

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a><span data-ttu-id="0d517-127">Recuperar um relatório de status concluído da URL de monitor</span><span class="sxs-lookup"><span data-stu-id="0d517-127">Retrieve a completed status report from the monitor URL</span></span>

<span data-ttu-id="0d517-128">Após alguns segundos, a operação de cópia foi concluída.</span><span class="sxs-lookup"><span data-stu-id="0d517-128">After a few seconds the copy operation has completed.</span></span>
<span data-ttu-id="0d517-129">Dessa vez, quando o aplicativo faz uma solicitação para a URL de monitor, a resposta é um redirecionamento para o resultado concluído da ação.</span><span class="sxs-lookup"><span data-stu-id="0d517-129">This time when the app makes a request to the monitor URL the response is a redirection to the finished result of the action.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="0d517-130">Após a conclusão da ação, a resposta do serviço de monitor retornará a resourceId para obter os resultados.</span><span class="sxs-lookup"><span data-stu-id="0d517-130">When the action has completed, the response from the monitor service will return the resourceId for the results.</span></span>

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

## <a name="retrieve-the-results-of-the-completed-operation"></a><span data-ttu-id="0d517-131">Recuperar os resultados da operação concluída</span><span class="sxs-lookup"><span data-stu-id="0d517-131">Retrieve the results of the completed operation</span></span>

<span data-ttu-id="0d517-132">Depois que o trabalho for concluído, a URL do monitor retornará o resourceId do resultado. Neste caso, trata-se da nova cópia do item original.</span><span class="sxs-lookup"><span data-stu-id="0d517-132">Once the job has completed, the monitor URL returns the resourceId of the result, in this case the new copy of the original item.</span></span>
<span data-ttu-id="0d517-133">Você pode resolver esse novo item usando resourceId; por exemplo:</span><span class="sxs-lookup"><span data-stu-id="0d517-133">You can address this new item using the resourceId, for example:</span></span>

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

## <a name="supported-resources"></a><span data-ttu-id="0d517-134">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="0d517-134">Supported resources</span></span>

<span data-ttu-id="0d517-135">Ações de execução longa têm suporte nos métodos de API a seguir</span><span class="sxs-lookup"><span data-stu-id="0d517-135">Long running actions are supported on the following API methods</span></span>

| <span data-ttu-id="0d517-136">**Recurso**</span><span class="sxs-lookup"><span data-stu-id="0d517-136">**Resource**</span></span> | <span data-ttu-id="0d517-137">**API**</span><span class="sxs-lookup"><span data-stu-id="0d517-137">**API**</span></span> |
|:------ | :------ |
| <span data-ttu-id="0d517-138">DriveItem</span><span class="sxs-lookup"><span data-stu-id="0d517-138">DriveItem</span></span> | [<span data-ttu-id="0d517-139">Copiar</span><span class="sxs-lookup"><span data-stu-id="0d517-139">Copy</span></span>](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a><span data-ttu-id="0d517-140">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0d517-140">Prerequisites</span></span>

<span data-ttu-id="0d517-141">As mesmas [permissões](./permissions-reference.md) que são necessárias para realizar uma ação de execução longa também são necessárias para consultar o status de uma ação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="0d517-141">The same [permissions](./permissions-reference.md) that are required to perform a long running action are also required to query the status of a long running action.</span></span>




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
