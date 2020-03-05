---
title: Excluir settingStateDeviceSummary
description: Exclui settingStateDeviceSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01487beef97e568fc351368eacf1f7996d69a096
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42483466"
---
# <a name="delete-settingstatedevicesummary"></a><span data-ttu-id="c4a19-103">Excluir settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="c4a19-103">Delete settingStateDeviceSummary</span></span>

<span data-ttu-id="c4a19-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c4a19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4a19-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4a19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4a19-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4a19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4a19-107">Exclui [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c4a19-107">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4a19-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4a19-108">Prerequisites</span></span>
<span data-ttu-id="c4a19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4a19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4a19-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4a19-111">Permission type</span></span>|<span data-ttu-id="c4a19-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4a19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4a19-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4a19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4a19-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4a19-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4a19-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4a19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4a19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4a19-116">Not supported.</span></span>|
|<span data-ttu-id="c4a19-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4a19-117">Application</span></span>|<span data-ttu-id="c4a19-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4a19-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4a19-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4a19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="c4a19-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a19-120">Request headers</span></span>
|<span data-ttu-id="c4a19-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4a19-121">Header</span></span>|<span data-ttu-id="c4a19-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c4a19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4a19-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4a19-123">Authorization</span></span>|<span data-ttu-id="c4a19-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4a19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4a19-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4a19-125">Accept</span></span>|<span data-ttu-id="c4a19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4a19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4a19-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a19-127">Request body</span></span>
<span data-ttu-id="c4a19-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4a19-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4a19-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4a19-129">Response</span></span>
<span data-ttu-id="c4a19-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c4a19-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c4a19-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4a19-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4a19-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a19-132">Request</span></span>
<span data-ttu-id="c4a19-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4a19-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="c4a19-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4a19-134">Response</span></span>
<span data-ttu-id="c4a19-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4a19-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





