---
title: Listar localizedNotificationMessages
description: Listar propriedades e relações de objetos de localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ffccd0f496c8096e06371f14cdadf7a1a12e08a5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963679"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="fb30d-103">Listar localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="fb30d-103">List localizedNotificationMessages</span></span>

> <span data-ttu-id="fb30d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fb30d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb30d-105">Listar propriedades e relações de objetos de [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="fb30d-105">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb30d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb30d-106">Prerequisites</span></span>
<span data-ttu-id="fb30d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb30d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb30d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb30d-109">Permission type</span></span>|<span data-ttu-id="fb30d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb30d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb30d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb30d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb30d-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb30d-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fb30d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb30d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb30d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb30d-114">Not supported.</span></span>|
|<span data-ttu-id="fb30d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb30d-115">Application</span></span>|<span data-ttu-id="fb30d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb30d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb30d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb30d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="fb30d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb30d-118">Request headers</span></span>
|<span data-ttu-id="fb30d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb30d-119">Header</span></span>|<span data-ttu-id="fb30d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fb30d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb30d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb30d-121">Authorization</span></span>|<span data-ttu-id="fb30d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb30d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb30d-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb30d-123">Accept</span></span>|<span data-ttu-id="fb30d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fb30d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb30d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb30d-125">Request body</span></span>
<span data-ttu-id="fb30d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb30d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb30d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb30d-127">Response</span></span>
<span data-ttu-id="fb30d-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb30d-128">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb30d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb30d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb30d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb30d-130">Request</span></span>
<span data-ttu-id="fb30d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb30d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="fb30d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb30d-132">Response</span></span>
<span data-ttu-id="fb30d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb30d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.localizedNotificationMessage",
      "id": "7a777708-7708-7a77-0877-777a0877777a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "locale": "Locale value",
      "subject": "Subject value",
      "messageTemplate": "Message Template value",
      "isDefault": true
    }
  ]
}
```



