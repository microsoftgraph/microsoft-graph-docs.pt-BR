---
title: Listar iosUpdateDeviceStatuses
description: Listar propriedades e relações dos objetos iosUpdateDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 66259147312b0174fc00d95d599984723fec352b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403886"
---
# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="67a85-103">Listar iosUpdateDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="67a85-103">List iosUpdateDeviceStatuses</span></span>

> <span data-ttu-id="67a85-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="67a85-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="67a85-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="67a85-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67a85-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="67a85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67a85-107">Listar propriedades e relações dos objetos [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="67a85-107">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67a85-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67a85-108">Prerequisites</span></span>
<span data-ttu-id="67a85-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="67a85-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="67a85-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67a85-111">Permission type</span></span>|<span data-ttu-id="67a85-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67a85-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67a85-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67a85-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67a85-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="67a85-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="67a85-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67a85-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67a85-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67a85-116">Not supported.</span></span>|
|<span data-ttu-id="67a85-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67a85-117">Application</span></span>|<span data-ttu-id="67a85-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67a85-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67a85-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67a85-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="67a85-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67a85-120">Request headers</span></span>
|<span data-ttu-id="67a85-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67a85-121">Header</span></span>|<span data-ttu-id="67a85-122">Valor</span><span class="sxs-lookup"><span data-stu-id="67a85-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67a85-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="67a85-123">Authorization</span></span>|<span data-ttu-id="67a85-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67a85-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67a85-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67a85-125">Accept</span></span>|<span data-ttu-id="67a85-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67a85-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67a85-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67a85-127">Request body</span></span>
<span data-ttu-id="67a85-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67a85-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67a85-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a85-129">Response</span></span>
<span data-ttu-id="67a85-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67a85-130">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67a85-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67a85-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="67a85-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67a85-132">Request</span></span>
<span data-ttu-id="67a85-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67a85-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="67a85-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a85-134">Response</span></span>
<span data-ttu-id="67a85-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67a85-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 708

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
      "id": "63a79499-9499-63a7-9994-a7639994a763",
      "installStatus": "available",
      "osVersion": "Os Version value",
      "deviceId": "Device Id value",
      "userId": "User Id value",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "platform": 8,
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




