---
title: Obter iosDerivedCredentialAuthenticationConfiguration
description: Leia as propriedades e as relações do objeto iosDerivedCredentialAuthenticationConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e8494c8b0571bbc736c19af5e9fe6807f3e8bdd7
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949086"
---
# <a name="get-iosderivedcredentialauthenticationconfiguration"></a><span data-ttu-id="c7e66-103">Obter iosDerivedCredentialAuthenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7e66-103">Get iosDerivedCredentialAuthenticationConfiguration</span></span>

> <span data-ttu-id="c7e66-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7e66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7e66-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7e66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7e66-106">Leia as propriedades e as relações do objeto [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c7e66-106">Read properties and relationships of the [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7e66-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7e66-107">Prerequisites</span></span>
<span data-ttu-id="c7e66-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7e66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7e66-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7e66-110">Permission type</span></span>|<span data-ttu-id="c7e66-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7e66-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7e66-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7e66-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7e66-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7e66-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c7e66-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7e66-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7e66-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7e66-115">Not supported.</span></span>|
|<span data-ttu-id="c7e66-116">Application</span><span class="sxs-lookup"><span data-stu-id="c7e66-116">Application</span></span>|<span data-ttu-id="c7e66-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7e66-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7e66-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7e66-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7e66-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c7e66-119">Optional query parameters</span></span>
<span data-ttu-id="c7e66-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c7e66-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7e66-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7e66-121">Request headers</span></span>
|<span data-ttu-id="c7e66-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7e66-122">Header</span></span>|<span data-ttu-id="c7e66-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c7e66-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7e66-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7e66-124">Authorization</span></span>|<span data-ttu-id="c7e66-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7e66-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7e66-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7e66-126">Accept</span></span>|<span data-ttu-id="c7e66-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c7e66-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7e66-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7e66-128">Request body</span></span>
<span data-ttu-id="c7e66-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7e66-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7e66-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7e66-130">Response</span></span>
<span data-ttu-id="c7e66-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7e66-131">If successful, this method returns a `200 OK` response code and [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7e66-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7e66-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7e66-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7e66-133">Request</span></span>
<span data-ttu-id="c7e66-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7e66-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c7e66-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7e66-135">Response</span></span>
<span data-ttu-id="c7e66-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7e66-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1305

{
  "value": {
    "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
    "id": "01713f58-3f58-0171-583f-7101583f7101",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "deviceManagementApplicabilityRuleOsEdition": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
      "osEditionTypes": [
        "windows10EnterpriseN"
      ],
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleOsVersion": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
      "minOSVersion": "Min OSVersion value",
      "maxOSVersion": "Max OSVersion value",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleDeviceMode": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
      "deviceMode": "sModeConfiguration",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```





