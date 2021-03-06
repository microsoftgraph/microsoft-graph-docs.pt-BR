---
title: Assine para alterar notificações de APIs de impressão na nuvem usando o Microsoft Graph
description: Saiba como assinar para alterar as notificações de eventos de trabalho de impressão usando a API do Microsoft Graph.
author: jahsu
localization_priority: Priority
ms.prod: cloud-printing
ms.custom: scenarios:getting-started
ms.openlocfilehash: 0d4cbaabb6fc05df3d9a58d1ced467bee0b8ef04
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515727"
---
# <a name="subscribe-to-change-notifications-from-cloud-printing-apis-using-microsoft-graph"></a><span data-ttu-id="fed63-103">Assine para alterar notificações de APIs de impressão na nuvem usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fed63-103">Subscribe to change notifications from cloud printing APIs using Microsoft Graph</span></span>

<span data-ttu-id="fed63-104">A Impressão Universal ajuda os clientes a mover a infraestrutura de impressão para a nuvem, e faz parte de um ecossistema robusto de soluções de parceiros que oferecem funcionalidade de impressão avançada.</span><span class="sxs-lookup"><span data-stu-id="fed63-104">Universal Print helps customers move their print infrastructure to the cloud, and is part of a robust ecosystem of partner solutions that offer advanced print functionality.</span></span> <span data-ttu-id="fed63-105">Essas soluções podem se tornar ainda mais poderosas quando você usa as APIs de impressão na nuvem do Microsoft Graph para integração com a Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="fed63-105">These solutions can become even more powerful when you use the cloud printing APIs in Microsoft Graph to integrate with Universal Print.</span></span>

<span data-ttu-id="fed63-106">Muitas soluções parceiras precisam processar trabalhos de impressão em tempo real à medida que são enviados dos dispositivos dos usuários para as impressoras, o que significa que eles precisam ser notificados quando os trabalhos de impressão estiverem disponíveis para processamento.</span><span class="sxs-lookup"><span data-stu-id="fed63-106">Many partner solutions need to process print jobs in real time as they're sent from users' devices to printers, which means they need to be notified when print jobs are available for processing.</span></span> <span data-ttu-id="fed63-107">A Impressão Universal fornece ganchos para que as soluções de fornecedores de impressão sejam notificadas conforme as tarefas se movem pela nuvem, e APIs que permitem o gerenciamento de impressoras e trabalhos de impressão.</span><span class="sxs-lookup"><span data-stu-id="fed63-107">Universal Print provides hooks for print vendor solutions to be notified as jobs move through the cloud, and APIs that enable management of printers and print jobs.</span></span>

<span data-ttu-id="fed63-108">Este artigo descreve como assinar notificações para vários eventos de trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="fed63-108">This article describes how to subscribe to notifications for various print job events.</span></span>


## <a name="get-started-with-change-notifications"></a><span data-ttu-id="fed63-109">Obtenha notificações de alterações</span><span class="sxs-lookup"><span data-stu-id="fed63-109">Get started with change notifications</span></span>

<span data-ttu-id="fed63-110">Antes de aproveitar as vantagens das notificações de alteração por meio do Microsoft Graph, você deve [registrar seu aplicativo no Azure](/azure/active-directory/develop/howto-create-service-principal-portal#register-an-application-with-azure-ad-and-create-a-service-principal) e provisionar o aplicativo no locatário do Azure Active Directory (Azure AD) do cliente.</span><span class="sxs-lookup"><span data-stu-id="fed63-110">Before you can take advantage of change notifications via Microsoft Graph, you must [register your application in Azure](/azure/active-directory/develop/howto-create-service-principal-portal#register-an-application-with-azure-ad-and-create-a-service-principal) and provision your application in the customers Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="fed63-111">Certifique-se de que o aplicativo tenha os escopos de permissão necessários habilitados, conforme descrito mais adiante neste artigo.</span><span class="sxs-lookup"><span data-stu-id="fed63-111">Make sure that the application has the required permission scopes enabled, as described later in this article.</span></span>


### <a name="notifications-and-subscriptions"></a><span data-ttu-id="fed63-112">Notificações e assinaturas</span><span class="sxs-lookup"><span data-stu-id="fed63-112">Notifications and subscriptions</span></span>

<span data-ttu-id="fed63-113">A Impressão Universal atualmente oferece suporte a notificações para dois cenários relacionados a trabalhos de impressão:</span><span class="sxs-lookup"><span data-stu-id="fed63-113">Universal Print currently supports notifications for two scenarios related to print jobs:</span></span>

* <span data-ttu-id="fed63-114">PrintTask é acionado (JobStarted): um aplicativo pode se inscrever para receber notificações quando o printTask(gancho) é acionado.</span><span class="sxs-lookup"><span data-stu-id="fed63-114">PrintTask is triggered (JobStarted): An application can subscribe to receive notifications when their printTask(hook) is triggered.</span></span>
<span data-ttu-id="fed63-115">Para obter detalhes sobre como acionar uma tarefa, confira [Estendendo a Impressão Universal para oferecer suporte ao pull de impressão](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="fed63-115">For details about how to trigger a task, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span> <span data-ttu-id="fed63-116">Atualmente, um printTask pode ser acionado apenas para um evento JobStarted.</span><span class="sxs-lookup"><span data-stu-id="fed63-116">Currently, a printTask can be triggered only for a JobStarted event.</span></span> <span data-ttu-id="fed63-117">Um evento JobStarted é gerado quando um trabalho de impressão é criado com sucesso, seu conteúdo é carregado e o processamento de trabalho é iniciado.</span><span class="sxs-lookup"><span data-stu-id="fed63-117">A JobStarted event is raised when a print job has been successfully created, its payload has been uploaded, and job processing has started.</span></span>  

* <span data-ttu-id="fed63-118">Jobfetchable: após o início do trabalho, aplicativos de impressão de terceiros ou a Impressão Universal podem fazer algum processamento (como converter o conteúdo XPS em PDF para uma impressora PDF).</span><span class="sxs-lookup"><span data-stu-id="fed63-118">JobFetchable: After the job has started, third-party print applications or Universal Print might do some processing (like converting XPS payload to PDF for a PDF printer).</span></span> <span data-ttu-id="fed63-119">Depois que o processamento for concluído e a conteúdo estiver pronto para ser baixado por uma impressora, um evento JobFetchable é gerado para o trabalho de impressão correspondente.</span><span class="sxs-lookup"><span data-stu-id="fed63-119">After processing is complete and the payload is ready to be downloaded by a printer, a JobFetchable event is raised for the corresponding print job.</span></span>

>[!NOTE]
><span data-ttu-id="fed63-120">Para ouvir as notificações de alteração do evento Jobfetchable, não é necessário um recurso **printTaskDefinition**.</span><span class="sxs-lookup"><span data-stu-id="fed63-120">For listening to the change notifications for JobFetchable event, a **printTaskDefinition** resource is not required.</span></span>

### <a name="create-an-application-to-listen-to-notifications"></a><span data-ttu-id="fed63-121">Crie um aplicativo para ouvir as notificações</span><span class="sxs-lookup"><span data-stu-id="fed63-121">Create an application to listen to notifications</span></span>

<span data-ttu-id="fed63-122">Para obter informações sobre como ouvir as notificações do Microsoft Graph, confira [Usar notificações de alteração e controlar alterações com o Microsoft Graph](https://docs.microsoft.com/learn/modules/msgraph-changenotifications-trackchanges/) e [Configurar notificações para alterações nos dados do usuário – Exemplos de código](/graph/webhooks#code-samples).</span><span class="sxs-lookup"><span data-stu-id="fed63-122">For information about how to listen for Microsoft Graph notifications, see [Use change notifications and track changes with Microsoft Graph](https://docs.microsoft.com/learn/modules/msgraph-changenotifications-trackchanges/) and [Set up notifications for changes in user data – Code Samples](/graph/webhooks#code-samples).</span></span>


### <a name="scopes"></a><span data-ttu-id="fed63-123">Escopos</span><span class="sxs-lookup"><span data-stu-id="fed63-123">Scopes</span></span>

<span data-ttu-id="fed63-124">Para assinar as notificações de trabalhos de impressão, os aplicativos devem ter os seguintes escopos de permissão aprovados no locatário do Azure AD do cliente:</span><span class="sxs-lookup"><span data-stu-id="fed63-124">To subscribe to notifications for print jobs, applications must have the following permission scopes approved in the customer’s Azure AD tenant:</span></span> 

* <span data-ttu-id="fed63-125">Para evento printTask acionado (JobStarted), as permissões listadas em [Obter taskDefinition](/graph/api/printtaskdefinition-get?view=graph-rest-beta&tabs=http%22%20%5Cl%20%22permissions%22%20%5C).</span><span class="sxs-lookup"><span data-stu-id="fed63-125">For printTask triggered (JobStarted) event, the permissions listed in [Get taskDefinition](/graph/api/printtaskdefinition-get?view=graph-rest-beta&tabs=http%22%20%5Cl%20%22permissions%22%20%5C).</span></span> 

* <span data-ttu-id="fed63-126">Para evento JobFetchable, as permissões listadas em [Criar assinatura](/graph/api/subscription-post-subscriptions?view=graph-rest-beta&tabs=http).</span><span class="sxs-lookup"><span data-stu-id="fed63-126">For JobFetchable event, the permissions listed in [Create subscription](/graph/api/subscription-post-subscriptions?view=graph-rest-beta&tabs=http).</span></span>

<span data-ttu-id="fed63-127">Os aplicativos devem [gerar e usar o token de segurança do Azure AD](/graph/auth-v2-service?context=graph%2Fapi%2Fbeta&view=graph-rest-beta) no cabeçalho de solicitação da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fed63-127">Applications must [generate and use the Azure AD security token](/graph/auth-v2-service?context=graph%2Fapi%2Fbeta&view=graph-rest-beta) in the Microsoft Graph API request header.</span></span> <span data-ttu-id="fed63-128">O token de segurança contém as declarações de acordo com os escopos aprovados para o locatário do Azure AD do cliente por seu administrador.</span><span class="sxs-lookup"><span data-stu-id="fed63-128">The security token contains the claims as per the scopes approved for the customer’s Azure AD tenant by its administrator.</span></span>  


## <a name="create-subscription-printtask-triggered-jobstarted-event"></a><span data-ttu-id="fed63-129">Criar assinatura: evento printTask acionado (JobStarted)</span><span class="sxs-lookup"><span data-stu-id="fed63-129">Create subscription: printTask triggered (JobStarted) event</span></span> 

<span data-ttu-id="fed63-130">Alguns aplicativos monitoram as filas de impressão em busca de trabalhos recebidos e para serem notificados assim que houver um trabalho válido na fila.</span><span class="sxs-lookup"><span data-stu-id="fed63-130">Some applications monitor print queues for incoming jobs and want to be notified as soon as there is a valid job in the queue.</span></span> <span data-ttu-id="fed63-131">Após serem notificados, eles podem coletar os metadados relevantes do trabalho ou até mesmo realizar modificações no trabalho de impressão – incluindo abortar o trabalho ou redirecionar o trabalho da fila de impressão atual para outra fila após modificar os atributos do trabalho corretamente.</span><span class="sxs-lookup"><span data-stu-id="fed63-131">After theyt're notified, they can collect the relevant job metadata or even perform modifications in the print job – including aborting the job or redirecting the job from the current print queue to another queue after modifying the job attributes accordingly.</span></span> 

<span data-ttu-id="fed63-132">Antes de criar uma notificação para um evento **printTask**-acionado, certifique-se de que o aplicativo criou o seguinte:</span><span class="sxs-lookup"><span data-stu-id="fed63-132">Before creating a notification for a **printTask**-triggered event, ensure that application has created the following:</span></span> 

- <span data-ttu-id="fed63-133">Um [printTaskDefinition](/graph/api/print-post-taskdefinitions?view=graph-rest-beta&tabs=http)  para o locatário do Azure AD do cliente.</span><span class="sxs-lookup"><span data-stu-id="fed63-133">A [printTaskDefinition](/graph/api/print-post-taskdefinitions?view=graph-rest-beta&tabs=http) for the customer’s Azure AD tenant.</span></span> <span data-ttu-id="fed63-134">Uma única definição de tarefa pode ser associada a uma ou mais impressoras no mesmo locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fed63-134">A single task definition can be associated with one or more printers within the same Azure AD tenant.</span></span> 

- <span data-ttu-id="fed63-135">Um [printTaskTrigger](/graph/api/printer-post-tasktriggers?view=graph-rest-beta&tabs=http) de cada uma das filas de impressão para as quais o parceiro quer receber uma notificação quando um novo trabalho de impressão for iniciado.</span><span class="sxs-lookup"><span data-stu-id="fed63-135">A [printTaskTrigger](/graph/api/printer-post-tasktriggers?view=graph-rest-beta&tabs=http) for each of the printer queues for which the partner wants to receive a notification when a new print job starts.</span></span> <span data-ttu-id="fed63-136">O **printTaskTrigger** precisa ser vinculado ao **printTaskDefinition**.</span><span class="sxs-lookup"><span data-stu-id="fed63-136">The **printTaskTrigger** needs to be bound to the **printTaskDefinition**.</span></span> 

>[!NOTE]
><span data-ttu-id="fed63-137">Uma impressora pode ser associada a apenas um **printTaskTrigger** e um **printTaskTrigger** pode ser associado a apenas um **printTaskDefinition**.</span><span class="sxs-lookup"><span data-stu-id="fed63-137">One printer can be associated with only one **printTaskTrigger** and one **printTaskTrigger** can be associated with only one **printTaskDefinition**.</span></span> <span data-ttu-id="fed63-138">No entanto, um **printTaskDefinition** pode ter um ou mais **printTaskTriggers** associados a ele.</span><span class="sxs-lookup"><span data-stu-id="fed63-138">However, one **printTaskDefinition** can have one or more **printTaskTriggers** associated with it.</span></span> 

<span data-ttu-id="fed63-139">Com o **printTaskDefinition** existente para o locatário do Azure AD do cliente, o aplicativo pode [criar uma assinatura para um evento printTask acionado (JobStarted) usando o printTaskDefinition](/graph/api/subscription-post-subscriptions?view=graph-rest-beta&tabs=http).</span><span class="sxs-lookup"><span data-stu-id="fed63-139">With the **printTaskDefinition** that exists for customer’s Azure AD tenant, the application can [create a subscription for a printTask triggered (JobStarted) event using the printTaskDefinition](/graph/api/subscription-post-subscriptions?view=graph-rest-beta&tabs=http).</span></span> <span data-ttu-id="fed63-140">Ao criar a assinatura:</span><span class="sxs-lookup"><span data-stu-id="fed63-140">While creating the subscription:</span></span>  

* <span data-ttu-id="fed63-141">O campo `resource` precisa ser definido como `print/taskDefinitions/{printTaskDefinition ID}/tasks`.</span><span class="sxs-lookup"><span data-stu-id="fed63-141">The `resource` field needs to be set as `print/taskDefinitions/{printTaskDefinition ID}/tasks`.</span></span> 
* <span data-ttu-id="fed63-142">O campo `changeType` precisa ser definido como `created`.</span><span class="sxs-lookup"><span data-stu-id="fed63-142">The `changeType` field needs to be set as `created`.</span></span> 
* <span data-ttu-id="fed63-143">O campo `expirationDateTime` precisa ser menor que o [tempo máximo de expiração](/graph/api/resources/subscription?view=graph-rest-beta#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="fed63-143">The `expirationDateTime` field needs to be less than the [maximum expiration time](/graph/api/resources/subscription?view=graph-rest-beta#maximum-length-of-subscription-per-resource-type).</span></span> 

<span data-ttu-id="fed63-144">Para obter mais detalhes, confira [Propriedades do tipo de recurso da assinatura.](/graph/api/resources/subscription?view=graph-rest-beta#properties).</span><span class="sxs-lookup"><span data-stu-id="fed63-144">For more details, see [Subscription resource type properties](/graph/api/resources/subscription?view=graph-rest-beta#properties).</span></span>

<span data-ttu-id="fed63-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fed63-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription"
}--> 
```http
POST https://graph.microsoft.com/beta/subscriptions 
Content-Type: application/json
{ 
    "changeType":"created", 
    "resource":"print/taskDefinitions/{printTaskDefinition ID}/tasks", 
    "clientState":"secret", 
    "notificationUrl":"{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "expirationDateTime":"2020-01-30T22:42:09Z" 
} 
```

### <a name="response"></a><span data-ttu-id="fed63-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="fed63-146">Response</span></span>

<span data-ttu-id="fed63-147">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="fed63-147">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
{ 
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity", 
    "id": "{Subscription ID}", 
    "resource": "print/taskDefinitions/{printTaskDefinition ID}/tasks", 
    "applicationId": "{application ID}", 
    "changeType": "created", 
    "clientState": "secret", 
    "notificationUrl": "{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "notificationQueryOptions": null, 
    "lifecycleNotificationUrl": null, 
    "expirationDateTime": "2020-12-30T22:42:09Z", 
    "creatorId": "{Creator ID}", 
    "includeResourceData": null, 
    "latestSupportedTlsVersion": "v1_2", 
    "encryptionCertificate": null, 
    "encryptionCertificateId": null 
}
```


## <a name="create-subscription-jobfetchable-event"></a><span data-ttu-id="fed63-148">Criar assinatura: evento JobFetchable</span><span class="sxs-lookup"><span data-stu-id="fed63-148">Create subscription: JobFetchable event</span></span> 
<span data-ttu-id="fed63-149">Alguns aplicativos de nuvem precisam baixar os trabalhos de impressão da Impressão Universal quando estiverem prontos.</span><span class="sxs-lookup"><span data-stu-id="fed63-149">Some cloud applications need to download print jobs from Universal Print when they are ready.</span></span> <span data-ttu-id="fed63-150">Como esses aplicativos em execução na nuvem não estão protegidos pelo firewall do cliente, eles podem usar as notificações de alteração do Microsoft Graph para serem notificados quando um trabalho de impressão estiver pronto para ser baixado.</span><span class="sxs-lookup"><span data-stu-id="fed63-150">Because these applications running in the cloud are not behind the customer's firewall, they can use Microsoft Graph change notifications to be notified when a print job is ready to be downloaded.</span></span>

>[!NOTE]
><span data-ttu-id="fed63-151">Trabalhos de impressão não podem ser modificados quando entram no estado JobFetchable.</span><span class="sxs-lookup"><span data-stu-id="fed63-151">Print jobs can't be modified when they enter the JobFetchable state.</span></span>
<span data-ttu-id="fed63-152">Uma notificação JobFetchable precisa ser criada para cada fila da impressora.</span><span class="sxs-lookup"><span data-stu-id="fed63-152">A JobFetchable notification needs to be created for each printer queue.</span></span> <span data-ttu-id="fed63-153">Ao criar a assinatura:</span><span class="sxs-lookup"><span data-stu-id="fed63-153">While creating the subscription:</span></span>
* <span data-ttu-id="fed63-154">O campo `resource` precisa ser definido como 'print/printers/{printer id}/jobs'.</span><span class="sxs-lookup"><span data-stu-id="fed63-154">The `resource` field needs to be set as 'print/printers/{printer id}/jobs'.</span></span> 
* <span data-ttu-id="fed63-155">O campo `changeType` precisa ser definido como `updated`.</span><span class="sxs-lookup"><span data-stu-id="fed63-155">The `changeType` field needs to be set as `updated`.</span></span> 
* <span data-ttu-id="fed63-156">O campo `notificationQueryOptions` precisa ser definido como `$filter = isFetchable eq true`.</span><span class="sxs-lookup"><span data-stu-id="fed63-156">The `notificationQueryOptions` field needs to be set as `$filter = isFetchable eq true`.</span></span> 
* <span data-ttu-id="fed63-157">O campo `expirationDateTime` precisa ser menor que o [tempo máximo de expiração](/graph/api/resources/subscription?view=graph-rest-beta#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="fed63-157">The `expirationDateTime` field needs to be less than the [maximum expiration time](/graph/api/resources/subscription?view=graph-rest-beta#maximum-length-of-subscription-per-resource-type).</span></span> 

<span data-ttu-id="fed63-158">Para obter mais detalhes, confira [Propriedades do tipo de recurso da assinatura.](/graph/api/resources/subscription?view=graph-rest-beta#properties).</span><span class="sxs-lookup"><span data-stu-id="fed63-158">For more details, see [Subscription resource type properties](/graph/api/resources/subscription?view=graph-rest-beta#properties).</span></span>

<span data-ttu-id="fed63-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fed63-159">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription"
}--> 
```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
    "changeType":"updated",
    "resource":"print/printers/{printer id}/jobs",
    "notificationQueryOptions": "$filter = isFetchable eq true", 
    "notificationUrl":"{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}",
    "expirationDateTime":"2020-12-30T22:42:09Z",
    "clientState":"mysecret"
} 
```

### <a name="response"></a><span data-ttu-id="fed63-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="fed63-160">Response</span></span>

<span data-ttu-id="fed63-161">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="fed63-161">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
{ 
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity", 
    "id": "{Subscription ID}", 
    "resource": "print/printers/{printer ID}/jobs", 
    "applicationId": "{Application ID}", 
    "changeType": "updated", 
    "clientState": "mysecret", 
    "notificationUrl": "{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "notificationQueryOptions": "$filter = isFetchable eq true", 
    "lifecycleNotificationUrl": null, 
    "expirationDateTime": "2020-12-30T22:42:09Z", 
    "creatorId": "{Creator ID}", 
    "includeResourceData": null, 
    "latestSupportedTlsVersion": "v1_2", 
    "encryptionCertificate": null, 
    "encryptionCertificateId": null
}
```


## <a name="renewing-a-notification-subscription"></a><span data-ttu-id="fed63-162">Renovando uma assinatura de notificação</span><span class="sxs-lookup"><span data-stu-id="fed63-162">Renewing a notification subscription</span></span>

<span data-ttu-id="fed63-163">O Microsoft Graph tem um limite de tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="fed63-163">Microsoft Graph has a limit on the expiration time.</span></span> <span data-ttu-id="fed63-164">Para obter detalhes, confira [tempo máximo de expiração](/graph/api/resources/subscription?view=graph-rest-beta#maximum-length-of-subscription-per-resource-type).</span><span class="sxs-lookup"><span data-stu-id="fed63-164">For details, see [maximum expiration time](/graph/api/resources/subscription?view=graph-rest-beta#maximum-length-of-subscription-per-resource-type).</span></span> <span data-ttu-id="fed63-165">Para continuar recebendo notificações, é necessário que a assinatura seja renovada periodicamente, usando a [API de atualização da assinatura](/graph/api/subscription-update?view=graph-rest-beta&tabs=http).</span><span class="sxs-lookup"><span data-stu-id="fed63-165">To continue receiving notifications, the subscription needs to be renewed periodically by using the [Update subscription API](/graph/api/subscription-update?view=graph-rest-beta&tabs=http).</span></span> 

## <a name="other-operations-on-notification-subscriptions"></a><span data-ttu-id="fed63-166">Outras operações sobre assinaturas de notificação</span><span class="sxs-lookup"><span data-stu-id="fed63-166">Other operations on notification subscriptions</span></span> 

<span data-ttu-id="fed63-167">Os aplicativos podem [obter](/graph/api/subscription-get?view=graph-rest-beta&tabs=http) detalhes da assinatura ou podem [excluir](/graph/api/subscription-delete?view=graph-rest-beta&tabs=http) uma assinatura quando necessário.</span><span class="sxs-lookup"><span data-stu-id="fed63-167">Applications can [get](/graph/api/subscription-get?view=graph-rest-beta&tabs=http) details of the subscription or can [delete](/graph/api/subscription-delete?view=graph-rest-beta&tabs=http) a subscription when required.</span></span> <span data-ttu-id="fed63-168">Para obter detalhes, confira [Usar a API do Microsoft Graph para receber notificações de alteração](/graph/api/resources/webhooks?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="fed63-168">For details, see [Use the Microsoft Graph API to get change notifications](/graph/api/resources/webhooks?view=graph-rest-beta).</span></span>


## <a name="faqs"></a><span data-ttu-id="fed63-169">Perguntas frequentes</span><span class="sxs-lookup"><span data-stu-id="fed63-169">FAQs</span></span>
### <a name="how-does-microsoft-graph-validate-notification-urls"></a><span data-ttu-id="fed63-170">Como o Microsoft Graph valida as URLs de notificação?</span><span class="sxs-lookup"><span data-stu-id="fed63-170">How does Microsoft Graph validate notification URLs?</span></span>
<span data-ttu-id="fed63-171">O Microsoft Graph valida o ponto de extremidade da notificação fornecido na propriedade **notificationUrl** da solicitação da assinatura antes de criá-la.</span><span class="sxs-lookup"><span data-stu-id="fed63-171">Microsoft Graph validates the notification endpoint provided in the **notificationUrl** property of the subscription request before creating the subscription.</span></span>
<span data-ttu-id="fed63-172">Para obter detalhes, confira [Validação do ponto de extremidade da notificação](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="fed63-172">For details, see [Notification endpoint validation](/graph/webhooks#notification-endpoint-validation).</span></span>

### <a name="what-are-applications-expected-to-do-after-receiving-a-change-notification"></a><span data-ttu-id="fed63-173">O que os aplicativos devem fazer após receber uma notificação de alteração?</span><span class="sxs-lookup"><span data-stu-id="fed63-173">What are applications expected to do after receiving a change notification?</span></span>
<span data-ttu-id="fed63-174">Os aplicativos devem processar e reconhecer todas as notificações de alteração recebidas.</span><span class="sxs-lookup"><span data-stu-id="fed63-174">Applications should process and acknowledge every change notification they receive.</span></span> <span data-ttu-id="fed63-175">Para obter detalhes, confira [Processando a notificação de alteração](/graph/webhooks#processing-the-change-notification).</span><span class="sxs-lookup"><span data-stu-id="fed63-175">For details, see [Processing the change notification](/graph/webhooks#processing-the-change-notification).</span></span>

### <a name="how-can-i-get-a-list-of-active-subscriptions"></a><span data-ttu-id="fed63-176">Como posso obter uma lista de assinaturas ativas?</span><span class="sxs-lookup"><span data-stu-id="fed63-176">How can I get a list of active subscriptions?</span></span>
<span data-ttu-id="fed63-177">Para obter detalhes sobre como recuperar uma lista de assinaturas de webhook, confira [Listar assinaturas](/graph/api/subscription-list?view=graph-rest-beta&tabs=http).</span><span class="sxs-lookup"><span data-stu-id="fed63-177">For details about how to retrieve a list of webhook subscriptions, see [List subscriptions](/graph/api/subscription-list?view=graph-rest-beta&tabs=http).</span></span>


## <a name="see-also"></a><span data-ttu-id="fed63-178">Confira também</span><span class="sxs-lookup"><span data-stu-id="fed63-178">See also</span></span>

- <span data-ttu-id="fed63-179">Para saber mais sobre a API de impressão na nuvem do Microsoft Graph, confira [Visão geral da API de impressão na nuvem da Impressão Universal](/graph/universal-print-concept-overview).</span><span class="sxs-lookup"><span data-stu-id="fed63-179">To learn more about the cloud printing API in Microsoft Graph, see [Universal Print cloud printing API overview](/graph/universal-print-concept-overview).</span></span> 
- <span data-ttu-id="fed63-180">Para ver sugestões ou comentários sobre a API de impressão na nuvem do Microsoft Graph, visite a [Comunidade de tecnologia da Impressão Universal](https://aka.ms/community/UniversalPrint).</span><span class="sxs-lookup"><span data-stu-id="fed63-180">For suggestions or feedback about the cloud printing API in Microsoft Graph, visit the [Universal Print tech community](https://aka.ms/community/UniversalPrint).</span></span>