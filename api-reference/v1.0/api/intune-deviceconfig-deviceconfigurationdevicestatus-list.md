---
title: Listar deviceConfigurationDeviceStatuses
description: Listar propriedades e relações dos objetos deviceConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0699363257d4733db017aafce251ba531bb321ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566014"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="5c91d-103">Listar deviceConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="5c91d-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="5c91d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c91d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c91d-105">Listar propriedades e relações dos objetos [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="5c91d-105">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c91d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c91d-106">Prerequisites</span></span>
<span data-ttu-id="5c91d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c91d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c91d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c91d-109">Permission type</span></span>|<span data-ttu-id="5c91d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c91d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c91d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c91d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c91d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c91d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5c91d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c91d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c91d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c91d-114">Not supported.</span></span>|
|<span data-ttu-id="5c91d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c91d-115">Application</span></span>|<span data-ttu-id="5c91d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c91d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c91d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c91d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="5c91d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c91d-118">Request headers</span></span>
|<span data-ttu-id="5c91d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c91d-119">Header</span></span>|<span data-ttu-id="5c91d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5c91d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c91d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c91d-121">Authorization</span></span>|<span data-ttu-id="5c91d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c91d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c91d-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5c91d-123">Accept</span></span>|<span data-ttu-id="5c91d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5c91d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c91d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c91d-125">Request body</span></span>
<span data-ttu-id="5c91d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c91d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c91d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c91d-127">Response</span></span>
<span data-ttu-id="5c91d-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c91d-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c91d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c91d-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c91d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c91d-130">Request</span></span>
<span data-ttu-id="5c91d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c91d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="5c91d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c91d-132">Response</span></span>
<span data-ttu-id="5c91d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c91d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
      "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



