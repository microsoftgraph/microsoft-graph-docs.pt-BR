---
title: Excluir deviceConfigurationDeviceStatus
description: Exclui deviceConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 65d2febcf24a501daa21d11aaa08af6e99c4ecac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32469450"
---
# <a name="delete-deviceconfigurationdevicestatus"></a><span data-ttu-id="f103c-103">Excluir deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="f103c-103">Delete deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="f103c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f103c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f103c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f103c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f103c-106">Exclui [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="f103c-106">Deletes a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f103c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f103c-107">Prerequisites</span></span>
<span data-ttu-id="f103c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f103c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f103c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f103c-110">Permission type</span></span>|<span data-ttu-id="f103c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f103c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f103c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f103c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f103c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f103c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f103c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f103c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f103c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f103c-115">Not supported.</span></span>|
|<span data-ttu-id="f103c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f103c-116">Application</span></span>|<span data-ttu-id="f103c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f103c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f103c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f103c-118">HTTP Request</span></span>
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
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="f103c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f103c-119">Request headers</span></span>
|<span data-ttu-id="f103c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f103c-120">Header</span></span>|<span data-ttu-id="f103c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f103c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f103c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f103c-122">Authorization</span></span>|<span data-ttu-id="f103c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f103c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f103c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f103c-124">Accept</span></span>|<span data-ttu-id="f103c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f103c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f103c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f103c-126">Request body</span></span>
<span data-ttu-id="f103c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f103c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f103c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f103c-128">Response</span></span>
<span data-ttu-id="f103c-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f103c-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f103c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f103c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f103c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f103c-131">Request</span></span>
<span data-ttu-id="f103c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f103c-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="f103c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f103c-133">Response</span></span>
<span data-ttu-id="f103c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f103c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





