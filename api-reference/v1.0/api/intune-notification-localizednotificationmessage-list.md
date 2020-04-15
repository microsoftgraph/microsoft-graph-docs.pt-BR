---
title: Listar localizedNotificationMessages
description: Listar propriedades e relações de objetos de localizedNotificationMessage.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8f56a7871a01316045f4d86ff1b440792cb7db35
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453018"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="60bfe-103">Listar localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="60bfe-103">List localizedNotificationMessages</span></span>

<span data-ttu-id="60bfe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60bfe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60bfe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60bfe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60bfe-106">Listar propriedades e relações de objetos de [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="60bfe-106">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60bfe-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60bfe-107">Prerequisites</span></span>
<span data-ttu-id="60bfe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60bfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60bfe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60bfe-110">Permission type</span></span>|<span data-ttu-id="60bfe-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60bfe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60bfe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60bfe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60bfe-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="60bfe-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="60bfe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60bfe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60bfe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60bfe-115">Not supported.</span></span>|
|<span data-ttu-id="60bfe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60bfe-116">Application</span></span>|<span data-ttu-id="60bfe-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60bfe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60bfe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60bfe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="60bfe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60bfe-119">Request headers</span></span>
|<span data-ttu-id="60bfe-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60bfe-120">Header</span></span>|<span data-ttu-id="60bfe-121">Valor</span><span class="sxs-lookup"><span data-stu-id="60bfe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60bfe-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="60bfe-122">Authorization</span></span>|<span data-ttu-id="60bfe-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60bfe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60bfe-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60bfe-124">Accept</span></span>|<span data-ttu-id="60bfe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60bfe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60bfe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60bfe-126">Request body</span></span>
<span data-ttu-id="60bfe-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60bfe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60bfe-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="60bfe-128">Response</span></span>
<span data-ttu-id="60bfe-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60bfe-129">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60bfe-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60bfe-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="60bfe-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60bfe-131">Request</span></span>
<span data-ttu-id="60bfe-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60bfe-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="60bfe-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="60bfe-133">Response</span></span>
<span data-ttu-id="60bfe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60bfe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






