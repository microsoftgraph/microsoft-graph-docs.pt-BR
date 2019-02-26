---
title: Obter localizedNotificationMessage
description: Ler propriedades e relações do objeto localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d4bc7f70c5c8b5cf0ccd8e4c0780af980bd3172
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255868"
---
# <a name="get-localizednotificationmessage"></a><span data-ttu-id="e3643-103">Obter localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="e3643-103">Get localizedNotificationMessage</span></span>

> <span data-ttu-id="e3643-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3643-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3643-105">Ler propriedades e relações do objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="e3643-105">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3643-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3643-106">Prerequisites</span></span>
<span data-ttu-id="e3643-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3643-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e3643-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3643-109">Permission type</span></span>|<span data-ttu-id="e3643-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3643-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3643-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3643-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3643-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3643-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e3643-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3643-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3643-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3643-114">Not supported.</span></span>|
|<span data-ttu-id="e3643-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3643-115">Application</span></span>|<span data-ttu-id="e3643-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3643-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3643-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3643-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3643-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e3643-118">Optional query parameters</span></span>
<span data-ttu-id="e3643-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e3643-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3643-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3643-120">Request headers</span></span>
|<span data-ttu-id="e3643-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3643-121">Header</span></span>|<span data-ttu-id="e3643-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e3643-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3643-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3643-123">Authorization</span></span>|<span data-ttu-id="e3643-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3643-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3643-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3643-125">Accept</span></span>|<span data-ttu-id="e3643-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3643-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3643-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3643-127">Request body</span></span>
<span data-ttu-id="e3643-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3643-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3643-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3643-129">Response</span></span>
<span data-ttu-id="e3643-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3643-130">If successful, this method returns a `200 OK` response code and [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3643-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3643-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3643-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3643-132">Request</span></span>
<span data-ttu-id="e3643-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3643-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="e3643-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3643-134">Response</span></span>
<span data-ttu-id="e3643-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3643-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.localizedNotificationMessage",
    "id": "7a777708-7708-7a77-0877-777a0877777a",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "locale": "Locale value",
    "subject": "Subject value",
    "messageTemplate": "Message Template value",
    "isDefault": true
  }
}
```



