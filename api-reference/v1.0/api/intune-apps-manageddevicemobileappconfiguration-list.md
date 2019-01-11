---
title: Listar managedDeviceMobileAppConfigurations
description: Listar propriedades e relações dos objetos managedDeviceMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 070ef484155083b61701999d79e986fe4b180a4e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822530"
---
# <a name="list-manageddevicemobileappconfigurations"></a><span data-ttu-id="c635b-103">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="c635b-103">List managedDeviceMobileAppConfigurations</span></span>

> <span data-ttu-id="c635b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c635b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c635b-105">Listar propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c635b-105">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c635b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c635b-106">Prerequisites</span></span>
<span data-ttu-id="c635b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c635b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c635b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c635b-109">Permission type</span></span>|<span data-ttu-id="c635b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c635b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c635b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c635b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c635b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c635b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c635b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c635b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c635b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c635b-114">Not supported.</span></span>|
|<span data-ttu-id="c635b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c635b-115">Application</span></span>|<span data-ttu-id="c635b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c635b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c635b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c635b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c635b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c635b-118">Request headers</span></span>
|<span data-ttu-id="c635b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c635b-119">Header</span></span>|<span data-ttu-id="c635b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c635b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c635b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c635b-121">Authorization</span></span>|<span data-ttu-id="c635b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c635b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c635b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c635b-123">Accept</span></span>|<span data-ttu-id="c635b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c635b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c635b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c635b-125">Request body</span></span>
<span data-ttu-id="c635b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c635b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c635b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c635b-127">Response</span></span>
<span data-ttu-id="c635b-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c635b-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c635b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c635b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c635b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c635b-130">Request</span></span>
<span data-ttu-id="c635b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c635b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="c635b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c635b-132">Response</span></span>
<span data-ttu-id="c635b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c635b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 485

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
      "id": "c60e7591-7591-c60e-9175-0ec691750ec6",
      "targetedMobileApps": [
        "Targeted Mobile Apps value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```



