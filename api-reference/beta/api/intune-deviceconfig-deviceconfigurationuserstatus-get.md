---
title: Acessar deviceConfigurationUserStatus
description: Leia as propriedades e as relações do objeto deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fac5576e6dc5f037f7517b2623a58c6f1ba895cb
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792853"
---
# <a name="get-deviceconfigurationuserstatus"></a><span data-ttu-id="c5efb-103">Acessar deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="c5efb-103">Get deviceConfigurationUserStatus</span></span>

<span data-ttu-id="c5efb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5efb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5efb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5efb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5efb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5efb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5efb-107">Leia as propriedades e as relações do objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="c5efb-107">Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5efb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5efb-108">Prerequisites</span></span>
<span data-ttu-id="c5efb-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c5efb-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c5efb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5efb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5efb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5efb-111">Permission type</span></span>|<span data-ttu-id="c5efb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5efb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5efb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5efb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5efb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5efb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c5efb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5efb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5efb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5efb-116">Not supported.</span></span>|
|<span data-ttu-id="c5efb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5efb-117">Application</span></span>|<span data-ttu-id="c5efb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5efb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5efb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5efb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5efb-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5efb-120">Optional query parameters</span></span>
<span data-ttu-id="c5efb-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5efb-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5efb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5efb-122">Request headers</span></span>
|<span data-ttu-id="c5efb-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5efb-123">Header</span></span>|<span data-ttu-id="c5efb-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c5efb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5efb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5efb-125">Authorization</span></span>|<span data-ttu-id="c5efb-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5efb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5efb-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5efb-127">Accept</span></span>|<span data-ttu-id="c5efb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c5efb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5efb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5efb-129">Request body</span></span>
<span data-ttu-id="c5efb-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5efb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5efb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5efb-131">Response</span></span>
<span data-ttu-id="c5efb-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5efb-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5efb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5efb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5efb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5efb-134">Request</span></span>
<span data-ttu-id="c5efb-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5efb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="c5efb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5efb-136">Response</span></span>
<span data-ttu-id="c5efb-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="c5efb-137">Here is an example of the response.</span></span> <span data-ttu-id="c5efb-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="c5efb-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c5efb-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c5efb-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
    "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



