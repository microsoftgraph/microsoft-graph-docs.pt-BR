---
title: Listar localizedNotificationMessages
description: Listar propriedades e relações de objetos de localizedNotificationMessage.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f8fa31c7a4b4fc1dbaf18c0b6351b942c709764
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125902"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="f7279-103">Listar localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="f7279-103">List localizedNotificationMessages</span></span>

<span data-ttu-id="f7279-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7279-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7279-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f7279-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7279-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7279-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7279-107">Listar propriedades e relações de objetos de [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="f7279-107">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7279-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7279-108">Prerequisites</span></span>
<span data-ttu-id="f7279-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7279-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7279-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7279-111">Permission type</span></span>|<span data-ttu-id="f7279-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7279-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7279-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7279-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7279-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7279-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f7279-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7279-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7279-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7279-116">Not supported.</span></span>|
|<span data-ttu-id="f7279-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7279-117">Application</span></span>|<span data-ttu-id="f7279-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7279-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7279-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7279-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="f7279-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7279-120">Request headers</span></span>
|<span data-ttu-id="f7279-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7279-121">Header</span></span>|<span data-ttu-id="f7279-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f7279-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7279-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7279-123">Authorization</span></span>|<span data-ttu-id="f7279-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7279-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7279-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f7279-125">Accept</span></span>|<span data-ttu-id="f7279-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7279-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7279-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7279-127">Request body</span></span>
<span data-ttu-id="f7279-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7279-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7279-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7279-129">Response</span></span>
<span data-ttu-id="f7279-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7279-130">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7279-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7279-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7279-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7279-132">Request</span></span>
<span data-ttu-id="f7279-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7279-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="f7279-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7279-134">Response</span></span>
<span data-ttu-id="f7279-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7279-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




