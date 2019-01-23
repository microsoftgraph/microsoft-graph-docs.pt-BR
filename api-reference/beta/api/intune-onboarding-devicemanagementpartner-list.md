---
title: Listar deviceManagementPartners
description: Listar propriedades e relações de objetos de deviceManagementPartner.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cc57c455ae4464ee94e82b0b8ab51b026fdfa129
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418320"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="369a4-103">Listar deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="369a4-103">List deviceManagementPartners</span></span>

> <span data-ttu-id="369a4-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="369a4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="369a4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="369a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="369a4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="369a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="369a4-107">Listar propriedades e relações de objetos de [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="369a4-107">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="369a4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="369a4-108">Prerequisites</span></span>
<span data-ttu-id="369a4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="369a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="369a4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="369a4-111">Permission type</span></span>|<span data-ttu-id="369a4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="369a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="369a4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="369a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="369a4-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="369a4-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="369a4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="369a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="369a4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="369a4-116">Not supported.</span></span>|
|<span data-ttu-id="369a4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="369a4-117">Application</span></span>|<span data-ttu-id="369a4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="369a4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="369a4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="369a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="369a4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="369a4-120">Request headers</span></span>
|<span data-ttu-id="369a4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="369a4-121">Header</span></span>|<span data-ttu-id="369a4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="369a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="369a4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="369a4-123">Authorization</span></span>|<span data-ttu-id="369a4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="369a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="369a4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="369a4-125">Accept</span></span>|<span data-ttu-id="369a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="369a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="369a4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="369a4-127">Request body</span></span>
<span data-ttu-id="369a4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="369a4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="369a4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="369a4-129">Response</span></span>
<span data-ttu-id="369a4-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="369a4-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="369a4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="369a4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="369a4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="369a4-132">Request</span></span>
<span data-ttu-id="369a4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="369a4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="369a4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="369a4-134">Response</span></span>
<span data-ttu-id="369a4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="369a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




