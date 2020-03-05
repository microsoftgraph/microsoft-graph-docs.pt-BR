---
title: Acessar deviceConfigurationUserOverview
description: Leia as propriedades e as relações do objeto deviceConfigurationUserOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 12a34f8c0a4d1369f47b1006796217067a8faf7a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442996"
---
# <a name="get-deviceconfigurationuseroverview"></a><span data-ttu-id="a2853-103">Acessar deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="a2853-103">Get deviceConfigurationUserOverview</span></span>

<span data-ttu-id="a2853-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a2853-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2853-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a2853-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2853-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2853-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2853-107">Leia as propriedades e as relações do objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="a2853-107">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2853-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2853-108">Prerequisites</span></span>
<span data-ttu-id="a2853-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2853-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2853-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2853-111">Permission type</span></span>|<span data-ttu-id="a2853-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a2853-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2853-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2853-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2853-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2853-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a2853-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2853-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2853-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2853-116">Not supported.</span></span>|
|<span data-ttu-id="a2853-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2853-117">Application</span></span>|<span data-ttu-id="a2853-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2853-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2853-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2853-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2853-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a2853-120">Optional query parameters</span></span>
<span data-ttu-id="a2853-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a2853-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2853-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2853-122">Request headers</span></span>
|<span data-ttu-id="a2853-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2853-123">Header</span></span>|<span data-ttu-id="a2853-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a2853-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2853-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2853-125">Authorization</span></span>|<span data-ttu-id="a2853-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2853-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2853-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a2853-127">Accept</span></span>|<span data-ttu-id="a2853-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a2853-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2853-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2853-129">Request body</span></span>
<span data-ttu-id="a2853-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2853-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2853-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2853-131">Response</span></span>
<span data-ttu-id="a2853-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2853-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2853-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2853-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2853-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2853-134">Request</span></span>
<span data-ttu-id="a2853-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2853-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="a2853-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2853-136">Response</span></span>
<span data-ttu-id="a2853-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2853-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
    "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





