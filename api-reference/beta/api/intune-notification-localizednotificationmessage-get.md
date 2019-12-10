---
title: Obter localizedNotificationMessage
description: Ler propriedades e relações do objeto localizedNotificationMessage.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 15a572721cc07931d8213581feed5a05233d7fe2
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942013"
---
# <a name="get-localizednotificationmessage"></a><span data-ttu-id="fabca-103">Obter localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="fabca-103">Get localizedNotificationMessage</span></span>

> <span data-ttu-id="fabca-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fabca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fabca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fabca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fabca-106">Ler propriedades e relações do objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="fabca-106">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fabca-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fabca-107">Prerequisites</span></span>
<span data-ttu-id="fabca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fabca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fabca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fabca-110">Permission type</span></span>|<span data-ttu-id="fabca-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fabca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fabca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fabca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fabca-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fabca-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fabca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fabca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fabca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fabca-115">Not supported.</span></span>|
|<span data-ttu-id="fabca-116">Application</span><span class="sxs-lookup"><span data-stu-id="fabca-116">Application</span></span>|<span data-ttu-id="fabca-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fabca-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fabca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fabca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fabca-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fabca-119">Optional query parameters</span></span>
<span data-ttu-id="fabca-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fabca-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fabca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fabca-121">Request headers</span></span>
|<span data-ttu-id="fabca-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fabca-122">Header</span></span>|<span data-ttu-id="fabca-123">Valor</span><span class="sxs-lookup"><span data-stu-id="fabca-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fabca-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fabca-124">Authorization</span></span>|<span data-ttu-id="fabca-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fabca-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fabca-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fabca-126">Accept</span></span>|<span data-ttu-id="fabca-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fabca-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fabca-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fabca-128">Request body</span></span>
<span data-ttu-id="fabca-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fabca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fabca-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fabca-130">Response</span></span>
<span data-ttu-id="fabca-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fabca-131">If successful, this method returns a `200 OK` response code and [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fabca-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fabca-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fabca-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fabca-133">Request</span></span>
<span data-ttu-id="fabca-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fabca-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="fabca-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fabca-135">Response</span></span>
<span data-ttu-id="fabca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fabca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





