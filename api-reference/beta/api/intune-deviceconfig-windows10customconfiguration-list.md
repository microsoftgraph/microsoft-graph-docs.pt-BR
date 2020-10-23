---
title: Listar windows10CustomConfigurations
description: Listar propriedades e relações dos objetos windows10CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e8185277788eb65742935669c72e779056b1f0b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691971"
---
# <a name="list-windows10customconfigurations"></a><span data-ttu-id="b7ca7-103">Listar windows10CustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="b7ca7-103">List windows10CustomConfigurations</span></span>

<span data-ttu-id="b7ca7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7ca7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7ca7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b7ca7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7ca7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7ca7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7ca7-107">Listar propriedades e relações dos objetos [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7ca7-107">List properties and relationships of the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7ca7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7ca7-108">Prerequisites</span></span>
<span data-ttu-id="b7ca7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7ca7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7ca7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7ca7-111">Permission type</span></span>|<span data-ttu-id="b7ca7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b7ca7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7ca7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7ca7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7ca7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7ca7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b7ca7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7ca7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7ca7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7ca7-116">Not supported.</span></span>|
|<span data-ttu-id="b7ca7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7ca7-117">Application</span></span>|<span data-ttu-id="b7ca7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7ca7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7ca7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7ca7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b7ca7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7ca7-120">Request headers</span></span>
|<span data-ttu-id="b7ca7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7ca7-121">Header</span></span>|<span data-ttu-id="b7ca7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b7ca7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7ca7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7ca7-123">Authorization</span></span>|<span data-ttu-id="b7ca7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7ca7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7ca7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7ca7-125">Accept</span></span>|<span data-ttu-id="b7ca7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7ca7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7ca7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7ca7-127">Request body</span></span>
<span data-ttu-id="b7ca7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7ca7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7ca7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7ca7-129">Response</span></span>
<span data-ttu-id="b7ca7-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7ca7-130">If successful, this method returns a `200 OK` response code and a collection of [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7ca7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7ca7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7ca7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7ca7-132">Request</span></span>
<span data-ttu-id="b7ca7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7ca7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b7ca7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7ca7-134">Response</span></span>
<span data-ttu-id="b7ca7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7ca7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1608

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
      "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSetting",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value"
        }
      ]
    }
  ]
}
```





