---
title: Listar deviceConfigurationUserStatuses
description: Listar propriedades e relações dos objetos deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: acbf3c3c064ce2dc6a426374e3309362a591fe70
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467868"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="effa7-103">Listar deviceConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="effa7-103">List deviceConfigurationUserStatuses</span></span>

> <span data-ttu-id="effa7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="effa7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="effa7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="effa7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="effa7-106">Listar propriedades e relações dos objetos [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="effa7-106">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="effa7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="effa7-107">Prerequisites</span></span>
<span data-ttu-id="effa7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="effa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="effa7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="effa7-110">Permission type</span></span>|<span data-ttu-id="effa7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="effa7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="effa7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="effa7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="effa7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="effa7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="effa7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="effa7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="effa7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="effa7-115">Not supported.</span></span>|
|<span data-ttu-id="effa7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="effa7-116">Application</span></span>|<span data-ttu-id="effa7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="effa7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="effa7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="effa7-118">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="effa7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="effa7-119">Request headers</span></span>
|<span data-ttu-id="effa7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="effa7-120">Header</span></span>|<span data-ttu-id="effa7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="effa7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="effa7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="effa7-122">Authorization</span></span>|<span data-ttu-id="effa7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="effa7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="effa7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="effa7-124">Accept</span></span>|<span data-ttu-id="effa7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="effa7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="effa7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="effa7-126">Request body</span></span>
<span data-ttu-id="effa7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="effa7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="effa7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="effa7-128">Response</span></span>
<span data-ttu-id="effa7-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="effa7-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="effa7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="effa7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="effa7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="effa7-131">Request</span></span>
<span data-ttu-id="effa7-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="effa7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="effa7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="effa7-133">Response</span></span>
<span data-ttu-id="effa7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="effa7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





