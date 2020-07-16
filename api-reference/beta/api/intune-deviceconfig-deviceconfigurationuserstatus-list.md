---
title: Listar deviceConfigurationUserStatuses
description: Listar propriedades e relações dos objetos deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2bd4b6ac70f4d5cf4408bd4d424b98df2a90cfa8
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792846"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="63a5b-103">Listar deviceConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="63a5b-103">List deviceConfigurationUserStatuses</span></span>

<span data-ttu-id="63a5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63a5b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63a5b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63a5b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63a5b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63a5b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63a5b-107">Listar propriedades e relações dos objetos [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="63a5b-107">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63a5b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63a5b-108">Prerequisites</span></span>
<span data-ttu-id="63a5b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63a5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63a5b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63a5b-111">Permission type</span></span>|<span data-ttu-id="63a5b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63a5b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63a5b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63a5b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63a5b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63a5b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="63a5b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63a5b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63a5b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63a5b-116">Not supported.</span></span>|
|<span data-ttu-id="63a5b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63a5b-117">Application</span></span>|<span data-ttu-id="63a5b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63a5b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63a5b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63a5b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="63a5b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63a5b-120">Request headers</span></span>
|<span data-ttu-id="63a5b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63a5b-121">Header</span></span>|<span data-ttu-id="63a5b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="63a5b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63a5b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="63a5b-123">Authorization</span></span>|<span data-ttu-id="63a5b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63a5b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63a5b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63a5b-125">Accept</span></span>|<span data-ttu-id="63a5b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63a5b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63a5b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63a5b-127">Request body</span></span>
<span data-ttu-id="63a5b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63a5b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63a5b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="63a5b-129">Response</span></span>
<span data-ttu-id="63a5b-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63a5b-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63a5b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63a5b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="63a5b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63a5b-132">Request</span></span>
<span data-ttu-id="63a5b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63a5b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="63a5b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="63a5b-134">Response</span></span>
<span data-ttu-id="63a5b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63a5b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
      "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



