---
title: Lista mobileAppTroubleshootingEvents
description: Lista as propriedades e os relacionamentos dos objetos mobileAppTroubleshootingEvent.
author: tfitzmac
ms.openlocfilehash: cee6872731977fedddced00f3bad678d3b3e42da
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308670"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="0d7ab-103">Lista mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="0d7ab-103">List mobileAppTroubleshootingEvents</span></span>

> <span data-ttu-id="0d7ab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0d7ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d7ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0d7ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d7ab-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0d7ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d7ab-107">Lista as propriedades e os relacionamentos dos objetos [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="0d7ab-107">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0d7ab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0d7ab-108">Prerequisites</span></span>
<span data-ttu-id="0d7ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d7ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d7ab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d7ab-111">Permission type</span></span>|<span data-ttu-id="0d7ab-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0d7ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d7ab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d7ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d7ab-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d7ab-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0d7ab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d7ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d7ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d7ab-116">Not supported.</span></span>|
|<span data-ttu-id="0d7ab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d7ab-117">Application</span></span>|<span data-ttu-id="0d7ab-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d7ab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d7ab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d7ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="0d7ab-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d7ab-120">Request headers</span></span>
|<span data-ttu-id="0d7ab-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0d7ab-121">Header</span></span>|<span data-ttu-id="0d7ab-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0d7ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d7ab-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d7ab-123">Authorization</span></span>|<span data-ttu-id="0d7ab-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d7ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d7ab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0d7ab-125">Accept</span></span>|<span data-ttu-id="0d7ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d7ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d7ab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d7ab-127">Request body</span></span>
<span data-ttu-id="0d7ab-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d7ab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d7ab-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d7ab-129">Response</span></span>
<span data-ttu-id="0d7ab-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d7ab-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d7ab-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d7ab-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0d7ab-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d7ab-132">Request</span></span>
<span data-ttu-id="0d7ab-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d7ab-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="0d7ab-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d7ab-134">Response</span></span>
<span data-ttu-id="0d7ab-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d7ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 623

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
      "id": "77943c10-3c10-7794-103c-9477103c9477",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value",
      "managedDeviceIdentifier": "Managed Device Identifier value",
      "userId": "User Id value",
      "applicationId": "Application Id value",
      "history": [
        {
          "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
          "occurrenceDateTime": "2017-01-01T00:03:20.8380798-08:00"
        }
      ]
    }
  ]
}
```





