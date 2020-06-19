---
title: Excluir deviceConfigurationUserStatus
description: Exclui deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6d8b73b0763822a2a4e22315febc34000225f1db
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792860"
---
# <a name="delete-deviceconfigurationuserstatus"></a><span data-ttu-id="1971c-103">Excluir deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="1971c-103">Delete deviceConfigurationUserStatus</span></span>

<span data-ttu-id="1971c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1971c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1971c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1971c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1971c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1971c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1971c-107">Exclui [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="1971c-107">Deletes a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1971c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1971c-108">Prerequisites</span></span>
<span data-ttu-id="1971c-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1971c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1971c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1971c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1971c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1971c-111">Permission type</span></span>|<span data-ttu-id="1971c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1971c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1971c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1971c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1971c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1971c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1971c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1971c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1971c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1971c-116">Not supported.</span></span>|
|<span data-ttu-id="1971c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1971c-117">Application</span></span>|<span data-ttu-id="1971c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1971c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1971c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1971c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="1971c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1971c-120">Request headers</span></span>
|<span data-ttu-id="1971c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1971c-121">Header</span></span>|<span data-ttu-id="1971c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1971c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1971c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1971c-123">Authorization</span></span>|<span data-ttu-id="1971c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1971c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1971c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1971c-125">Accept</span></span>|<span data-ttu-id="1971c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1971c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1971c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1971c-127">Request body</span></span>
<span data-ttu-id="1971c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1971c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1971c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1971c-129">Response</span></span>
<span data-ttu-id="1971c-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1971c-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1971c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1971c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1971c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1971c-132">Request</span></span>
<span data-ttu-id="1971c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1971c-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="1971c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1971c-134">Response</span></span>
<span data-ttu-id="1971c-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1971c-135">Here is an example of the response.</span></span> <span data-ttu-id="1971c-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1971c-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1971c-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1971c-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



