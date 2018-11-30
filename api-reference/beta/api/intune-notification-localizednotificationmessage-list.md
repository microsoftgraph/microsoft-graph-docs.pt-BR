---
title: Listar localizedNotificationMessages
description: Listar propriedades e relações de objetos de localizedNotificationMessage.
ms.openlocfilehash: 649864ae18c48ec86090c18cf4f50a9ac1801f86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033222"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="33f06-103">Listar localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="33f06-103">List localizedNotificationMessages</span></span>

> <span data-ttu-id="33f06-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="33f06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33f06-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="33f06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33f06-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="33f06-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33f06-107">Listar propriedades e relações de objetos de [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="33f06-107">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33f06-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33f06-108">Prerequisites</span></span>
<span data-ttu-id="33f06-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33f06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33f06-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33f06-111">Permission type</span></span>|<span data-ttu-id="33f06-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="33f06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33f06-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33f06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33f06-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="33f06-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="33f06-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33f06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33f06-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33f06-116">Not supported.</span></span>|
|<span data-ttu-id="33f06-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33f06-117">Application</span></span>|<span data-ttu-id="33f06-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33f06-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33f06-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33f06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="33f06-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33f06-120">Request headers</span></span>
|<span data-ttu-id="33f06-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33f06-121">Header</span></span>|<span data-ttu-id="33f06-122">Valor</span><span class="sxs-lookup"><span data-stu-id="33f06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33f06-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33f06-123">Authorization</span></span>|<span data-ttu-id="33f06-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33f06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33f06-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33f06-125">Accept</span></span>|<span data-ttu-id="33f06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33f06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33f06-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33f06-127">Request body</span></span>
<span data-ttu-id="33f06-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="33f06-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33f06-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="33f06-129">Response</span></span>
<span data-ttu-id="33f06-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33f06-130">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33f06-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33f06-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="33f06-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33f06-132">Request</span></span>
<span data-ttu-id="33f06-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33f06-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="33f06-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="33f06-134">Response</span></span>
<span data-ttu-id="33f06-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33f06-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





