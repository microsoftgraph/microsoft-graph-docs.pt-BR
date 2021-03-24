---
title: Listar deviceConfigurationUserStatuses
description: Listar propriedades e relações dos objetos deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e69ce1d68d675db4a010a3d6ef17c857d7ffeb80
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137473"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="7dc3f-103">Listar deviceConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="7dc3f-103">List deviceConfigurationUserStatuses</span></span>

<span data-ttu-id="7dc3f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dc3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7dc3f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7dc3f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dc3f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7dc3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dc3f-107">Listar propriedades e relações dos objetos [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="7dc3f-107">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dc3f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7dc3f-108">Prerequisites</span></span>
<span data-ttu-id="7dc3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dc3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dc3f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dc3f-111">Permission type</span></span>|<span data-ttu-id="7dc3f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7dc3f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dc3f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dc3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7dc3f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dc3f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7dc3f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dc3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dc3f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dc3f-116">Not supported.</span></span>|
|<span data-ttu-id="7dc3f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7dc3f-117">Application</span></span>|<span data-ttu-id="7dc3f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dc3f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dc3f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dc3f-119">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="7dc3f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7dc3f-120">Request headers</span></span>
|<span data-ttu-id="7dc3f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7dc3f-121">Header</span></span>|<span data-ttu-id="7dc3f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7dc3f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dc3f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7dc3f-123">Authorization</span></span>|<span data-ttu-id="7dc3f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7dc3f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dc3f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7dc3f-125">Accept</span></span>|<span data-ttu-id="7dc3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7dc3f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dc3f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7dc3f-127">Request body</span></span>
<span data-ttu-id="7dc3f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7dc3f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dc3f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dc3f-129">Response</span></span>
<span data-ttu-id="7dc3f-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dc3f-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dc3f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dc3f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dc3f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dc3f-132">Request</span></span>
<span data-ttu-id="7dc3f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7dc3f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="7dc3f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dc3f-134">Response</span></span>
<span data-ttu-id="7dc3f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7dc3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




