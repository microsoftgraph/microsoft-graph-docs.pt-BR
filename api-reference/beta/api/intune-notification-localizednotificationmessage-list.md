---
title: Listar localizedNotificationMessages
description: Listar propriedades e relações de objetos de localizedNotificationMessage.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1d04f62f995f486f161045162ab68599ab799d06
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727770"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="ae384-103">Listar localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="ae384-103">List localizedNotificationMessages</span></span>

<span data-ttu-id="ae384-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae384-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae384-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae384-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae384-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae384-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae384-107">Listar propriedades e relações de objetos de [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="ae384-107">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae384-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae384-108">Prerequisites</span></span>
<span data-ttu-id="ae384-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae384-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae384-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae384-111">Permission type</span></span>|<span data-ttu-id="ae384-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae384-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae384-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae384-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae384-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae384-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ae384-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae384-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae384-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae384-116">Not supported.</span></span>|
|<span data-ttu-id="ae384-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae384-117">Application</span></span>|<span data-ttu-id="ae384-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae384-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae384-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae384-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="ae384-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae384-120">Request headers</span></span>
|<span data-ttu-id="ae384-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae384-121">Header</span></span>|<span data-ttu-id="ae384-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ae384-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae384-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae384-123">Authorization</span></span>|<span data-ttu-id="ae384-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae384-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae384-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae384-125">Accept</span></span>|<span data-ttu-id="ae384-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae384-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae384-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae384-127">Request body</span></span>
<span data-ttu-id="ae384-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae384-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae384-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae384-129">Response</span></span>
<span data-ttu-id="ae384-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae384-130">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae384-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae384-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae384-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae384-132">Request</span></span>
<span data-ttu-id="ae384-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae384-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="ae384-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae384-134">Response</span></span>
<span data-ttu-id="ae384-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae384-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





