---
title: Listar localizedNotificationMessages
description: Listar propriedades e relações de objetos de localizedNotificationMessage.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 343b1b42f892ef80d549ff801aa5bea73330a2ad
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191199"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="08973-103">Listar localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="08973-103">List localizedNotificationMessages</span></span>

> <span data-ttu-id="08973-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="08973-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08973-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08973-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08973-106">Listar propriedades e relações de objetos de [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="08973-106">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08973-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="08973-107">Prerequisites</span></span>
<span data-ttu-id="08973-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08973-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08973-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08973-110">Permission type</span></span>|<span data-ttu-id="08973-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="08973-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08973-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08973-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08973-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="08973-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="08973-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08973-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08973-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08973-115">Not supported.</span></span>|
|<span data-ttu-id="08973-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08973-116">Application</span></span>|<span data-ttu-id="08973-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="08973-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08973-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08973-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="08973-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08973-119">Request headers</span></span>
|<span data-ttu-id="08973-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="08973-120">Header</span></span>|<span data-ttu-id="08973-121">Valor</span><span class="sxs-lookup"><span data-stu-id="08973-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08973-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="08973-122">Authorization</span></span>|<span data-ttu-id="08973-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08973-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08973-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="08973-124">Accept</span></span>|<span data-ttu-id="08973-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08973-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08973-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08973-126">Request body</span></span>
<span data-ttu-id="08973-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="08973-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08973-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="08973-128">Response</span></span>
<span data-ttu-id="08973-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08973-129">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08973-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08973-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="08973-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08973-131">Request</span></span>
<span data-ttu-id="08973-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08973-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="08973-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="08973-133">Response</span></span>
<span data-ttu-id="08973-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08973-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




