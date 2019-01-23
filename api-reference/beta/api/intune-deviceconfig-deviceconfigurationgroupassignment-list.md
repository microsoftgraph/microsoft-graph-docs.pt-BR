---
title: Lista deviceConfigurationGroupAssignments
description: Lista as propriedades e os relacionamentos dos objetos deviceConfigurationGroupAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a55cdea2c27c56ee0fe5c61eef4a694f446d4e7c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424382"
---
# <a name="list-deviceconfigurationgroupassignments"></a><span data-ttu-id="e7b95-103">Lista deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="e7b95-103">List deviceConfigurationGroupAssignments</span></span>

> <span data-ttu-id="e7b95-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e7b95-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e7b95-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e7b95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7b95-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e7b95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7b95-107">Lista as propriedades e os relacionamentos dos objetos [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e7b95-107">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7b95-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7b95-108">Prerequisites</span></span>
<span data-ttu-id="e7b95-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7b95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e7b95-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7b95-111">Permission type</span></span>|<span data-ttu-id="e7b95-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7b95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7b95-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7b95-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7b95-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7b95-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e7b95-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7b95-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7b95-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7b95-116">Not supported.</span></span>|
|<span data-ttu-id="e7b95-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7b95-117">Application</span></span>|<span data-ttu-id="e7b95-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7b95-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7b95-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7b95-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="e7b95-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7b95-120">Request headers</span></span>
|<span data-ttu-id="e7b95-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7b95-121">Header</span></span>|<span data-ttu-id="e7b95-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e7b95-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7b95-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7b95-123">Authorization</span></span>|<span data-ttu-id="e7b95-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7b95-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7b95-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7b95-125">Accept</span></span>|<span data-ttu-id="e7b95-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7b95-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7b95-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7b95-127">Request body</span></span>
<span data-ttu-id="e7b95-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7b95-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7b95-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7b95-129">Response</span></span>
<span data-ttu-id="e7b95-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7b95-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7b95-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7b95-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7b95-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7b95-132">Request</span></span>
<span data-ttu-id="e7b95-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7b95-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="e7b95-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7b95-134">Response</span></span>
<span data-ttu-id="e7b95-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7b95-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 244

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ]
}
```




