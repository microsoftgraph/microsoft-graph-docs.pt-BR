---
title: Assine para alterar notificações de APIs de impressão na nuvem usando o Microsoft Graph
description: Saiba como assinar para alterar as notificações de eventos de trabalho de impressão usando a API do Microsoft Graph.
author: jahsu
ms.localizationpriority: high
ms.prod: cloud-printing
ms.custom: scenarios:getting-started
ms.openlocfilehash: df511878bfebba02bd68ede445a26b66233caeae
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143455"
---
# <a name="subscribe-to-change-notifications-from-cloud-printing-apis-using-microsoft-graph"></a>Assine para alterar notificações de APIs de impressão na nuvem usando o Microsoft Graph

A Impressão Universal ajuda os clientes a mover a infraestrutura de impressão para a nuvem, e faz parte de um ecossistema robusto de soluções de parceiros que oferecem funcionalidade de impressão avançada. Essas soluções podem se tornar ainda mais poderosas quando você usa as APIs de impressão na nuvem do Microsoft Graph para integração com a Impressão Universal.

Muitas soluções parceiras precisam processar trabalhos de impressão em tempo real à medida que são enviados dos dispositivos dos usuários para as impressoras, o que significa que eles precisam ser notificados quando os trabalhos de impressão estiverem disponíveis para processamento. A Impressão Universal fornece ganchos para que as soluções de fornecedores de impressão sejam notificadas conforme as tarefas se movem pela nuvem, e APIs que permitem o gerenciamento de impressoras e trabalhos de impressão.

Este artigo descreve como assinar notificações para vários eventos de trabalho de impressão.


## <a name="get-started-with-change-notifications"></a>Obtenha notificações de alterações

Antes de aproveitar as vantagens das notificações de alteração por meio do Microsoft Graph, você deve [registrar seu aplicativo no Azure](/azure/active-directory/develop/howto-create-service-principal-portal#register-an-application-with-azure-ad-and-create-a-service-principal) e provisionar o aplicativo no locatário do Azure Active Directory (Azure AD) do cliente. Certifique-se de que o aplicativo tenha os escopos de permissão necessários habilitados, conforme descrito mais adiante neste artigo.


### <a name="notifications-and-subscriptions"></a>Notificações e assinaturas

A Impressão Universal atualmente oferece suporte a notificações para dois cenários relacionados a trabalhos de impressão:

* PrintTask é acionado (JobStarted): um aplicativo pode se inscrever para receber notificações quando o printTask(gancho) é acionado.
Para obter detalhes sobre como acionar uma tarefa, confira [Estendendo a Impressão Universal para oferecer suporte ao pull de impressão](./universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing). Atualmente, um printTask pode ser acionado apenas para um evento JobStarted. Um evento JobStarted é gerado quando um trabalho de impressão é criado com sucesso, seu conteúdo é carregado e o processamento de trabalho é iniciado.  

* Jobfetchable: após o início do trabalho, aplicativos de impressão de terceiros ou a Impressão Universal podem fazer algum processamento (como converter o conteúdo XPS em PDF para uma impressora PDF). Depois que o processamento for concluído e a conteúdo estiver pronto para ser baixado por uma impressora, um evento JobFetchable é gerado para o trabalho de impressão correspondente.

>[!NOTE]
>Para ouvir as notificações de alteração do evento Jobfetchable, não é necessário um recurso **printTaskDefinition**.

### <a name="create-an-application-to-listen-to-notifications"></a>Crie um aplicativo para ouvir as notificações

Para obter informações sobre como ouvir as notificações do Microsoft Graph, confira [Usar notificações de alteração e controlar alterações com o Microsoft Graph](/learn/modules/msgraph-changenotifications-trackchanges/) e [Configurar notificações para alterações nos dados do usuário – Exemplos de código](./webhooks.md#code-samples).


### <a name="scopes"></a>Escopos

Para assinar as notificações de trabalhos de impressão, os aplicativos devem ter os seguintes escopos de permissão aprovados no locatário do Azure AD do cliente: 

* Para evento printTask acionado (JobStarted), as permissões listadas em [Obter taskDefinition](/graph/api/printtaskdefinition-get?view=graph-rest-v1.0&tabs=http%22%20%5Cl%20%22permissions%22%20%5C). 

* Para evento JobFetchable, as permissões listadas em [Criar assinatura](/graph/api/subscription-post-subscriptions?view=graph-rest-v1.0&tabs=http).

Os aplicativos devem [gerar e usar o token de segurança do Azure AD](/graph/auth-v2-service?context=graph%2Fapi%2F1.0) no cabeçalho de solicitação da API do Microsoft Graph. O token de segurança contém as declarações de acordo com os escopos aprovados para o locatário do Azure AD do cliente por seu administrador.  


## <a name="create-subscription-printtask-triggered-jobstarted-event"></a>Criar assinatura: evento printTask acionado (JobStarted) 

Alguns aplicativos monitoram as filas de impressão em busca de trabalhos recebidos e para serem notificados assim que houver um trabalho válido na fila. Após serem notificados, eles podem coletar os metadados relevantes do trabalho ou até mesmo realizar modificações no trabalho de impressão – incluindo abortar o trabalho ou redirecionar o trabalho da fila de impressão atual para outra fila após modificar os atributos do trabalho corretamente. 

Antes de criar uma notificação para um evento **printTask**-acionado, certifique-se de que o aplicativo criou o seguinte: 

- Um [printTaskDefinition](/graph/api/print-post-taskdefinitions?view=graph-rest-v1.0&tabs=http)  para o locatário do Azure AD do cliente. Uma única definição de tarefa pode ser associada a uma ou mais impressoras no mesmo locatário do Azure AD. 

- Um [printTaskTrigger](/graph/api/printer-post-tasktriggers?view=graph-rest-v1.0&tabs=http) de cada uma das filas de impressão para as quais o parceiro quer receber uma notificação quando um novo trabalho de impressão for iniciado. O **printTaskTrigger** precisa ser vinculado ao **printTaskDefinition**. 

>[!NOTE]
>Uma impressora pode ser associada a apenas um **printTaskTrigger** e um **printTaskTrigger** pode ser associado a apenas um **printTaskDefinition**. No entanto, um **printTaskDefinition** pode ter um ou mais **printTaskTriggers** associados a ele. 

Com o **printTaskDefinition** existente para o locatário do Azure AD do cliente, o aplicativo pode [criar uma assinatura para um evento printTask acionado (JobStarted) usando o printTaskDefinition](/graph/api/subscription-post-subscriptions?view=graph-rest-v1.0&tabs=http). Ao criar a assinatura:  

* O campo `resource` precisa ser definido como `print/taskDefinitions/{printTaskDefinition ID}/tasks`. 
* O campo `changeType` precisa ser definido como `created`. 
* O campo `expirationDateTime` precisa ser menor que o [tempo máximo de expiração](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type). 

Para obter mais detalhes, confira [Propriedades do tipo de recurso da assinatura.](/graph/api/resources/subscription?view=graph-rest-v1.0#properties).

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "create_subscription"
}--> 
```http
POST https://graph.microsoft.com/v1.0/subscriptions 
Content-Type: application/json
{ 
    "changeType":"created", 
    "resource":"print/taskDefinitions/{printTaskDefinition ID}/tasks", 
    "clientState":"secret", 
    "notificationUrl":"{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "expirationDateTime":"2020-01-30T22:42:09Z" 
} 
```

### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
{ 
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity", 
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


## <a name="create-subscription-jobfetchable-event"></a>Criar assinatura: evento JobFetchable 
Alguns aplicativos de nuvem precisam baixar os trabalhos de impressão da Impressão Universal quando estiverem prontos. Como esses aplicativos em execução na nuvem não estão protegidos pelo firewall do cliente, eles podem usar as notificações de alteração do Microsoft Graph para serem notificados quando um trabalho de impressão estiver pronto para ser baixado.

>[!NOTE]
>Trabalhos de impressão não podem ser modificados quando entram no estado JobFetchable.
Uma notificação JobFetchable precisa ser criada para cada fila da impressora. Ao criar a assinatura:
* O campo `resource` precisa ser definido como 'print/printers/{printer id}/jobs'. 
* O campo `changeType` precisa ser definido como `updated`. 
* O campo `notificationQueryOptions` precisa ser definido como `$filter = isFetchable eq true`. 
* O campo `expirationDateTime` precisa ser menor que o [tempo máximo de expiração](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type). 

Para obter mais detalhes, confira [Propriedades do tipo de recurso da assinatura.](/graph/api/resources/subscription?view=graph-rest-v1.0#properties).

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "create_subscription"
}--> 
```http
POST https://graph.microsoft.com/v1.0/subscriptions
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

### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
{ 
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity", 
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


## <a name="renewing-a-notification-subscription"></a>Renovando uma assinatura de notificação

O Microsoft Graph tem um limite de tempo de expiração. Para obter detalhes, confira [tempo máximo de expiração](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type). Para continuar recebendo notificações, é necessário que a assinatura seja renovada periodicamente, usando a [API de atualização da assinatura](/graph/api/subscription-update?view=graph-rest-v1.0&tabs=http). 

## <a name="other-operations-on-notification-subscriptions"></a>Outras operações sobre assinaturas de notificação 

Os aplicativos podem [obter](/graph/api/subscription-get?view=graph-rest-v1.0&tabs=http) detalhes da assinatura ou podem [excluir](/graph/api/subscription-delete?view=graph-rest-v1.0&tabs=http) uma assinatura quando necessário. Para obter detalhes, confira [Usar a API do Microsoft Graph para receber notificações de alteração](/graph/api/resources/webhooks?view=graph-rest-v1.0).


## <a name="faqs"></a>Perguntas frequentes
### <a name="how-does-microsoft-graph-validate-notification-urls"></a>Como o Microsoft Graph valida as URLs de notificação?
O Microsoft Graph valida o ponto de extremidade da notificação fornecido na propriedade **notificationUrl** da solicitação da assinatura antes de criá-la.
Para obter detalhes, confira [Validação do ponto de extremidade da notificação](./webhooks.md#notification-endpoint-validation).

### <a name="what-are-applications-expected-to-do-after-receiving-a-change-notification"></a>O que os aplicativos devem fazer após receber uma notificação de alteração?
Os aplicativos devem processar e reconhecer todas as notificações de alteração recebidas. Para obter detalhes, confira [Processando a notificação de alteração](./webhooks.md#processing-the-change-notification).

### <a name="how-can-i-get-a-list-of-active-subscriptions"></a>Como posso obter uma lista de assinaturas ativas?
Para obter detalhes sobre como recuperar uma lista de assinaturas de webhook, confira [Listar assinaturas](/graph/api/subscription-list?view=graph-rest-v1.0&tabs=http).


## <a name="see-also"></a>Confira também

- Para saber mais sobre a API de impressão na nuvem do Microsoft Graph, confira [Visão geral da API de impressão na nuvem da Impressão Universal](/graph/universal-print-concept-overview). 
- Para ver sugestões ou comentários sobre a API de impressão na nuvem do Microsoft Graph, visite a [Comunidade de tecnologia da Impressão Universal](https://aka.ms/community/UniversalPrint).
