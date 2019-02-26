---
title: Listar editionUpgradeConfigurations
description: Listar propriedades e relações dos objetos editionUpgradeConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c99f110e2e3ff9fbc51f93f977e3f9fd6db9e58
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157887"
---
# <a name="list-editionupgradeconfigurations"></a><span data-ttu-id="50fc3-103">Listar editionUpgradeConfigurations</span><span class="sxs-lookup"><span data-stu-id="50fc3-103">List editionUpgradeConfigurations</span></span>

> <span data-ttu-id="50fc3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50fc3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50fc3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50fc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50fc3-106">Listar propriedades e relações dos objetos [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50fc3-106">List properties and relationships of the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50fc3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50fc3-107">Prerequisites</span></span>
<span data-ttu-id="50fc3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="50fc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="50fc3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50fc3-110">Permission type</span></span>|<span data-ttu-id="50fc3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50fc3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50fc3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50fc3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50fc3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50fc3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="50fc3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50fc3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50fc3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50fc3-115">Not supported.</span></span>|
|<span data-ttu-id="50fc3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50fc3-116">Application</span></span>|<span data-ttu-id="50fc3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50fc3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50fc3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50fc3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="50fc3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50fc3-119">Request headers</span></span>
|<span data-ttu-id="50fc3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50fc3-120">Header</span></span>|<span data-ttu-id="50fc3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="50fc3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50fc3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="50fc3-122">Authorization</span></span>|<span data-ttu-id="50fc3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50fc3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50fc3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50fc3-124">Accept</span></span>|<span data-ttu-id="50fc3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="50fc3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50fc3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50fc3-126">Request body</span></span>
<span data-ttu-id="50fc3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50fc3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50fc3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="50fc3-128">Response</span></span>
<span data-ttu-id="50fc3-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50fc3-129">If successful, this method returns a `200 OK` response code and a collection of [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50fc3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50fc3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="50fc3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50fc3-131">Request</span></span>
<span data-ttu-id="50fc3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50fc3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="50fc3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="50fc3-133">Response</span></span>
<span data-ttu-id="50fc3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50fc3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 700

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
      "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "licenseType": "licenseFile",
      "targetEdition": "windows10EnterpriseN",
      "license": "License value",
      "productKey": "Product Key value",
      "windowsSMode": "block"
    }
  ]
}
```




