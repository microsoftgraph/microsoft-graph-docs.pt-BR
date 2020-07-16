---
title: Excluir deviceConfigurationDeviceStatus
description: Exclui deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5cb807d186408d6cd76a701b5b19bdf6a94338db
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792944"
---
# <a name="delete-deviceconfigurationdevicestatus"></a><span data-ttu-id="8fec6-103">Excluir deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8fec6-103">Delete deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="8fec6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fec6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8fec6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8fec6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fec6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8fec6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fec6-107">Exclui [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8fec6-107">Deletes a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fec6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8fec6-108">Prerequisites</span></span>
<span data-ttu-id="8fec6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fec6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fec6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fec6-111">Permission type</span></span>|<span data-ttu-id="8fec6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8fec6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fec6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fec6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8fec6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fec6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8fec6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fec6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fec6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fec6-116">Not supported.</span></span>|
|<span data-ttu-id="8fec6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fec6-117">Application</span></span>|<span data-ttu-id="8fec6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fec6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fec6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fec6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="8fec6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8fec6-120">Request headers</span></span>
|<span data-ttu-id="8fec6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8fec6-121">Header</span></span>|<span data-ttu-id="8fec6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8fec6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fec6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fec6-123">Authorization</span></span>|<span data-ttu-id="8fec6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8fec6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fec6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8fec6-125">Accept</span></span>|<span data-ttu-id="8fec6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8fec6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fec6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fec6-127">Request body</span></span>
<span data-ttu-id="8fec6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8fec6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fec6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fec6-129">Response</span></span>
<span data-ttu-id="8fec6-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8fec6-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8fec6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8fec6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fec6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fec6-132">Request</span></span>
<span data-ttu-id="8fec6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8fec6-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="8fec6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fec6-134">Response</span></span>
<span data-ttu-id="8fec6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8fec6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



