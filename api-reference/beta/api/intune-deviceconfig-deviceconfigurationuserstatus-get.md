---
title: Acessar deviceConfigurationUserStatus
description: Leia as propriedades e as relações do objeto deviceConfigurationUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f83f7027b194ca0cdd24d02ca831e484d3166e8f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967493"
---
# <a name="get-deviceconfigurationuserstatus"></a><span data-ttu-id="17a9c-103">Acessar deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="17a9c-103">Get deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="17a9c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17a9c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17a9c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17a9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17a9c-106">Leia as propriedades e as relações do objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="17a9c-106">Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17a9c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17a9c-107">Prerequisites</span></span>
<span data-ttu-id="17a9c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17a9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17a9c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17a9c-110">Permission type</span></span>|<span data-ttu-id="17a9c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17a9c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17a9c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17a9c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17a9c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="17a9c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="17a9c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17a9c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17a9c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17a9c-115">Not supported.</span></span>|
|<span data-ttu-id="17a9c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17a9c-116">Application</span></span>|<span data-ttu-id="17a9c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17a9c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17a9c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17a9c-118">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17a9c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="17a9c-119">Optional query parameters</span></span>
<span data-ttu-id="17a9c-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="17a9c-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17a9c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17a9c-121">Request headers</span></span>
|<span data-ttu-id="17a9c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17a9c-122">Header</span></span>|<span data-ttu-id="17a9c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="17a9c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17a9c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="17a9c-124">Authorization</span></span>|<span data-ttu-id="17a9c-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17a9c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17a9c-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17a9c-126">Accept</span></span>|<span data-ttu-id="17a9c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="17a9c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17a9c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17a9c-128">Request body</span></span>
<span data-ttu-id="17a9c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17a9c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17a9c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="17a9c-130">Response</span></span>
<span data-ttu-id="17a9c-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17a9c-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17a9c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17a9c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="17a9c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17a9c-133">Request</span></span>
<span data-ttu-id="17a9c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17a9c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="17a9c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="17a9c-135">Response</span></span>
<span data-ttu-id="17a9c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17a9c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





