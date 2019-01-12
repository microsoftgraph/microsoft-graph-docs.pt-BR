---
title: Como trabalhar com ações de execução longa (beta)
description: Este artigo descreve o trabalho com ações de execução longa.
localization_priority: Normal
ms.openlocfilehash: d7ee9631e9e18ae1972e2b156366c66d3d3dd455
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868051"
---
# <a name="working-with-long-running-actions-beta"></a><span data-ttu-id="b44b8-103">Como trabalhar com ações de execução longa (beta)</span><span class="sxs-lookup"><span data-stu-id="b44b8-103">Working with long running actions (beta)</span></span>

> <span data-ttu-id="b44b8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b44b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b44b8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b44b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b44b8-106">Algumas respostas de API exigem tempo indeterminado para serem concluídas.</span><span class="sxs-lookup"><span data-stu-id="b44b8-106">Some API responses require indeterminate time to complete.</span></span>
<span data-ttu-id="b44b8-107">Em vez de ter que esperar até que a ação seja concluída antes de retornar uma resposta, o Microsoft Graph pode usar um padrão de ações de execução longa.</span><span class="sxs-lookup"><span data-stu-id="b44b8-107">Instead of waiting until the action is complete before returning a response, Microsoft Graph may use a long running actions pattern.</span></span>
<span data-ttu-id="b44b8-108">Esse padrão fornece ao aplicativo uma espera para sondar se há atualizações de status em uma ação de execução longa, sem que qualquer solicitação aguarde até que a ação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="b44b8-108">This pattern provides your app a wait to poll for status updates on a long running action, without any request waiting for the action to complete.</span></span>

<span data-ttu-id="b44b8-109">O padrão geral segue estas etapas:</span><span class="sxs-lookup"><span data-stu-id="b44b8-109">The general pattern follows these steps:</span></span>

1. <span data-ttu-id="b44b8-110">O aplicativo solicita uma ação de execução longa por meio da API.</span><span class="sxs-lookup"><span data-stu-id="b44b8-110">Your app requests a long running action via the API.</span></span> <span data-ttu-id="b44b8-111">A API aceita a ação e retorna uma resposta `202 Accepted` junto com um cabeçalho de Local para que a URL de API recupere relatórios de status de ação.</span><span class="sxs-lookup"><span data-stu-id="b44b8-111">The API accepts the action and returns a `202 Accepted` response along with a Location header for the API URL to retrieve action status reports.</span></span>
2. <span data-ttu-id="b44b8-112">O aplicativo solicita a URL de relatório de status de ação e recebe uma resposta [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) com o progresso da ação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="b44b8-112">Your app requests the action status report URL and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response with the progress of the long running action.</span></span>
3. <span data-ttu-id="b44b8-113">A ação de execução longa é concluída.</span><span class="sxs-lookup"><span data-stu-id="b44b8-113">The long running action completes.</span></span> 
4. <span data-ttu-id="b44b8-114">O aplicativo solicita a URL de relatório de status da ação novamente e recebe uma resposta [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) que mostra a conclusão da ação.</span><span class="sxs-lookup"><span data-stu-id="b44b8-114">Your app requests the action status report URL again and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response showing the completion of the action.</span></span>

## <a name="initial-action-request"></a><span data-ttu-id="b44b8-115">Solicitação de ação inicial</span><span class="sxs-lookup"><span data-stu-id="b44b8-115">Initial action request</span></span>

<span data-ttu-id="b44b8-116">Vamos percorrer as etapas para obter um cenário de exemplo de [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="b44b8-116">Let's walk through the steps for an example [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta) scenario.</span></span>
<span data-ttu-id="b44b8-117">Neste cenário, o aplicativo solicita a cópia de uma pasta que contém uma grande quantidade de dados.</span><span class="sxs-lookup"><span data-stu-id="b44b8-117">In this scenario, your app requests to copy a folder that contains a large amount of data.</span></span>
<span data-ttu-id="b44b8-118">Essa solicitação provavelmente levará vários segundos para ser concluída, pois a quantidade de dados é grande.</span><span class="sxs-lookup"><span data-stu-id="b44b8-118">This request will likely take several seconds to complete since the amount of data is large.</span></span>

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

<span data-ttu-id="b44b8-119">A API responde que a ação foi aceita e fornece a URL para recuperar o status da ação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="b44b8-119">The API responds that the action was accepted and the URL for retrieving the status of the long running action.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="b44b8-120">**Observação:** o local da URL retornado pode não estar no ponto de extremidade da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b44b8-120">**Note:** The location URL returned may not be on the Microsoft Graph API endpoint.</span></span>

<span data-ttu-id="b44b8-121">Em muitos casos, esse pode ser o fim da solicitação, pois a ação de cópia será concluída sem que o aplicativo realize tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="b44b8-121">In many cases this may be the end of the request, since the copy action will complete without the app doing any additional work.</span></span>
<span data-ttu-id="b44b8-122">No entanto, se o aplicativo precisar mostrar o status da ação de cópia ou garantir que ela seja concluída sem erros, poderá fazer isso usando a URL de monitor.</span><span class="sxs-lookup"><span data-stu-id="b44b8-122">However, if your app needs to show the status of the copy action or ensure that it completes without error, it can do so using the monitor URL.</span></span>

## <a name="retrieve-a-status-report-from-the-monitor-url"></a><span data-ttu-id="b44b8-123">Recuperar um relatório de status da URL de monitor</span><span class="sxs-lookup"><span data-stu-id="b44b8-123">Retrieve a status report from the monitor URL</span></span>

<span data-ttu-id="b44b8-124">Para verificar o status da ação de cópia, o aplicativo faz uma solicitação para a URL fornecida na resposta anterior.</span><span class="sxs-lookup"><span data-stu-id="b44b8-124">To check on the status of the copy action, the app makes a request to the URL provided in the previous response.</span></span>
<span data-ttu-id="b44b8-125">*Observação:* Essa solicitação não requer autenticação, pois a URL é de curta duração e exclusiva para o chamador original.</span><span class="sxs-lookup"><span data-stu-id="b44b8-125">*Note:* This request does not require authentication, since the URL is short-lived and unique to the original caller.</span></span> 

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="b44b8-126">O serviço responde com a informação de que a ação de execução longa ainda está em andamento:</span><span class="sxs-lookup"><span data-stu-id="b44b8-126">The service responses with information that the long running action is still in progress:</span></span>

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

<span data-ttu-id="b44b8-127">As informações podem ser usadas para fornecer uma atualização ao usuário sobre o progresso da ação de cópia.</span><span class="sxs-lookup"><span data-stu-id="b44b8-127">This information can be used to provide an update to the user about the progress of the copy action.</span></span>
<span data-ttu-id="b44b8-128">O aplicativo pode continuar a sondar a URL de monitor para solicitar atualizações de status e acompanhar o andamento da ação.</span><span class="sxs-lookup"><span data-stu-id="b44b8-128">The app can continue to poll the monitor URL to request status updates and keep track of the progress of the action.</span></span>

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a><span data-ttu-id="b44b8-129">Recuperar um relatório de status concluído da URL de monitor</span><span class="sxs-lookup"><span data-stu-id="b44b8-129">Retrieve a completed status report from the monitor URL</span></span>

<span data-ttu-id="b44b8-130">Após alguns segundos, a operação de cópia foi concluída.</span><span class="sxs-lookup"><span data-stu-id="b44b8-130">After a few seconds the copy operation has completed.</span></span>
<span data-ttu-id="b44b8-131">Dessa vez, quando o aplicativo faz uma solicitação para a URL de monitor, a resposta é um redirecionamento para o resultado concluído da ação.</span><span class="sxs-lookup"><span data-stu-id="b44b8-131">This time when the app makes a request to the monitor URL the response is a redirection to the finished result of the action.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="b44b8-132">Após a conclusão da ação, a resposta do serviço de monitor retornará a resourceId para obter os resultados.</span><span class="sxs-lookup"><span data-stu-id="b44b8-132">When the action has completed, the response from the monitor service will return the resourceId for the results.</span></span>

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

## <a name="retrieve-the-results-of-the-completed-operation"></a><span data-ttu-id="b44b8-133">Recuperar os resultados da operação concluída</span><span class="sxs-lookup"><span data-stu-id="b44b8-133">Retrieve the results of the completed operation</span></span>

<span data-ttu-id="b44b8-134">Depois que o trabalho for concluído, a URL do monitor retornará o resourceId do resultado. Neste caso, trata-se da nova cópia do item original.</span><span class="sxs-lookup"><span data-stu-id="b44b8-134">Once the job has completed, the monitor URL returns the resourceId of the result, in this case the new copy of the original item.</span></span>
<span data-ttu-id="b44b8-135">Você pode resolver esse novo item usando resourceId; por exemplo:</span><span class="sxs-lookup"><span data-stu-id="b44b8-135">You can address this new item using the resourceId, for example:</span></span>

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

## <a name="supported-resources"></a><span data-ttu-id="b44b8-136">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="b44b8-136">Supported resources</span></span>

<span data-ttu-id="b44b8-137">Ações de execução longa têm suporte nos métodos de API a seguir</span><span class="sxs-lookup"><span data-stu-id="b44b8-137">Long running actions are supported on the following API methods</span></span>

| <span data-ttu-id="b44b8-138">**Recurso**</span><span class="sxs-lookup"><span data-stu-id="b44b8-138">**Resource**</span></span> | <span data-ttu-id="b44b8-139">**API**</span><span class="sxs-lookup"><span data-stu-id="b44b8-139">**API**</span></span> |
|:------ | :------ |
| <span data-ttu-id="b44b8-140">DriveItem</span><span class="sxs-lookup"><span data-stu-id="b44b8-140">DriveItem</span></span> | [<span data-ttu-id="b44b8-141">Copiar</span><span class="sxs-lookup"><span data-stu-id="b44b8-141">Copy</span></span>](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a><span data-ttu-id="b44b8-142">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b44b8-142">Prerequisites</span></span>

<span data-ttu-id="b44b8-143">As mesmas [permissões](./permissions-reference.md) que são necessárias para realizar uma ação de execução longa também são necessárias para consultar o status de uma ação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="b44b8-143">The same [permissions](./permissions-reference.md) that are required to perform a long running action are also required to query the status of a long running action.</span></span>




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
