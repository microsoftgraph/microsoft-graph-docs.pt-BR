---
title: Listar deviceManagementTroubleshootingEvents
description: Listar propriedades e relações de objetos de deviceManagementTroubleshootingEvent.
author: tfitzmac
ms.openlocfilehash: 7d159e6f851c1e3635a85be2ab123436e267493b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325274"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="c00fe-103">Listar deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="c00fe-103">List deviceManagementTroubleshootingEvents</span></span>

> <span data-ttu-id="c00fe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c00fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c00fe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c00fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c00fe-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c00fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c00fe-107">Listar propriedades e relações de objetos de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="c00fe-107">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c00fe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c00fe-108">Prerequisites</span></span>
<span data-ttu-id="c00fe-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c00fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c00fe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c00fe-111">Permission type</span></span>|<span data-ttu-id="c00fe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c00fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c00fe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c00fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c00fe-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c00fe-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c00fe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c00fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c00fe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c00fe-116">Not supported.</span></span>|
|<span data-ttu-id="c00fe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c00fe-117">Application</span></span>|<span data-ttu-id="c00fe-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c00fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c00fe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c00fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="c00fe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c00fe-120">Request headers</span></span>
|<span data-ttu-id="c00fe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c00fe-121">Header</span></span>|<span data-ttu-id="c00fe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c00fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c00fe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c00fe-123">Authorization</span></span>|<span data-ttu-id="c00fe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c00fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c00fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c00fe-125">Accept</span></span>|<span data-ttu-id="c00fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c00fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c00fe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c00fe-127">Request body</span></span>
<span data-ttu-id="c00fe-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c00fe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c00fe-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c00fe-129">Response</span></span>
<span data-ttu-id="c00fe-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c00fe-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c00fe-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c00fe-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c00fe-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c00fe-132">Request</span></span>
<span data-ttu-id="c00fe-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c00fe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="c00fe-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c00fe-134">Response</span></span>
<span data-ttu-id="c00fe-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c00fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
      "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value"
    }
  ]
}
```





