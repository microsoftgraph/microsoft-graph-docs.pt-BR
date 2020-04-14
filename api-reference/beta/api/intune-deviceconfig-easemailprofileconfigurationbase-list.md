---
title: Listar easEmailProfileConfigurationBases
description: Listar Propriedades e relações dos objetos easEmailProfileConfigurationBase.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f79777a9514524ade5e7c5832d9d7f34c87779b9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433156"
---
# <a name="list-easemailprofileconfigurationbases"></a><span data-ttu-id="18234-103">Listar easEmailProfileConfigurationBases</span><span class="sxs-lookup"><span data-stu-id="18234-103">List easEmailProfileConfigurationBases</span></span>

<span data-ttu-id="18234-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18234-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18234-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="18234-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18234-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18234-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18234-107">Listar Propriedades e relações dos objetos [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) .</span><span class="sxs-lookup"><span data-stu-id="18234-107">List properties and relationships of the [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18234-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="18234-108">Prerequisites</span></span>
<span data-ttu-id="18234-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18234-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18234-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18234-111">Permission type</span></span>|<span data-ttu-id="18234-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="18234-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18234-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18234-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18234-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18234-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="18234-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18234-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18234-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18234-116">Not supported.</span></span>|
|<span data-ttu-id="18234-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18234-117">Application</span></span>|<span data-ttu-id="18234-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18234-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18234-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18234-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="18234-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18234-120">Request headers</span></span>
|<span data-ttu-id="18234-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18234-121">Header</span></span>|<span data-ttu-id="18234-122">Valor</span><span class="sxs-lookup"><span data-stu-id="18234-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18234-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="18234-123">Authorization</span></span>|<span data-ttu-id="18234-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18234-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18234-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="18234-125">Accept</span></span>|<span data-ttu-id="18234-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18234-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18234-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18234-127">Request body</span></span>
<span data-ttu-id="18234-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="18234-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18234-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="18234-129">Response</span></span>
<span data-ttu-id="18234-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18234-130">If successful, this method returns a `200 OK` response code and a collection of [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18234-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18234-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="18234-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18234-132">Request</span></span>
<span data-ttu-id="18234-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18234-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="18234-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="18234-134">Response</span></span>
<span data-ttu-id="18234-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18234-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1572

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.easEmailProfileConfigurationBase",
      "id": "a3f96310-6310-a3f9-1063-f9a31063f9a3",
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
      "version": 7,
      "usernameSource": "primarySmtpAddress",
      "usernameAADSource": "primarySmtpAddress",
      "userDomainNameSource": "netBiosDomainName",
      "customDomainName": "Custom Domain Name value"
    }
  ]
}
```



