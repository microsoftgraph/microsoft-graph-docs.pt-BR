---
title: Listar deviceManagementPartners
description: Listar propriedades e relações de objetos de deviceManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8b208cefcc2fa19a82447138bdc7022b5fa62613
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941034"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="39eae-103">Listar deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="39eae-103">List deviceManagementPartners</span></span>

> <span data-ttu-id="39eae-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="39eae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39eae-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="39eae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39eae-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="39eae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39eae-107">Listar propriedades e relações de objetos de [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="39eae-107">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39eae-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="39eae-108">Prerequisites</span></span>
<span data-ttu-id="39eae-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39eae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39eae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39eae-111">Permission type</span></span>|<span data-ttu-id="39eae-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="39eae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39eae-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39eae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39eae-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="39eae-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="39eae-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39eae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39eae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39eae-116">Not supported.</span></span>|
|<span data-ttu-id="39eae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39eae-117">Application</span></span>|<span data-ttu-id="39eae-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39eae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39eae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39eae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="39eae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39eae-120">Request headers</span></span>
|<span data-ttu-id="39eae-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39eae-121">Header</span></span>|<span data-ttu-id="39eae-122">Valor</span><span class="sxs-lookup"><span data-stu-id="39eae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39eae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="39eae-123">Authorization</span></span>|<span data-ttu-id="39eae-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39eae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39eae-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="39eae-125">Accept</span></span>|<span data-ttu-id="39eae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39eae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39eae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39eae-127">Request body</span></span>
<span data-ttu-id="39eae-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="39eae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39eae-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="39eae-129">Response</span></span>
<span data-ttu-id="39eae-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39eae-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39eae-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39eae-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="39eae-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39eae-132">Request</span></span>
<span data-ttu-id="39eae-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39eae-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="39eae-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="39eae-134">Response</span></span>
<span data-ttu-id="39eae-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39eae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 794

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementPartner",
      "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "unavailable",
      "partnerAppType": "singleTenantApp",
      "singleTenantAppId": "Single Tenant App Id value",
      "displayName": "Display Name value",
      "isConfigured": true,
      "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
      "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
    }
  ]
}
```





