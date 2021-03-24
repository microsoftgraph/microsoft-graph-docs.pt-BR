---
title: Listar deviceManagementConfigurationPolicies
description: Listar propriedades e relações dos objetos deviceManagementConfigurationPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6e19a3b30212899d6cdf341e14f9627e54fb8742
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127162"
---
# <a name="list-devicemanagementconfigurationpolicies"></a><span data-ttu-id="8444d-103">Listar deviceManagementConfigurationPolicies</span><span class="sxs-lookup"><span data-stu-id="8444d-103">List deviceManagementConfigurationPolicies</span></span>

<span data-ttu-id="8444d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8444d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8444d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8444d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8444d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8444d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8444d-107">Listar propriedades e relações dos [objetos deviceManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8444d-107">List properties and relationships of the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8444d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8444d-108">Prerequisites</span></span>
<span data-ttu-id="8444d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8444d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8444d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8444d-111">Permission type</span></span>|<span data-ttu-id="8444d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8444d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8444d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8444d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8444d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8444d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8444d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8444d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8444d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8444d-116">Not supported.</span></span>|
|<span data-ttu-id="8444d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8444d-117">Application</span></span>|<span data-ttu-id="8444d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8444d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8444d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8444d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationPolicies
```

## <a name="request-headers"></a><span data-ttu-id="8444d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8444d-120">Request headers</span></span>
|<span data-ttu-id="8444d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8444d-121">Header</span></span>|<span data-ttu-id="8444d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8444d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8444d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8444d-123">Authorization</span></span>|<span data-ttu-id="8444d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8444d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8444d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8444d-125">Accept</span></span>|<span data-ttu-id="8444d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8444d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8444d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8444d-127">Request body</span></span>
<span data-ttu-id="8444d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8444d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8444d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8444d-129">Response</span></span>
<span data-ttu-id="8444d-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8444d-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8444d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8444d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8444d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8444d-132">Request</span></span>
<span data-ttu-id="8444d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8444d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicies
```

### <a name="response"></a><span data-ttu-id="8444d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8444d-134">Response</span></span>
<span data-ttu-id="8444d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8444d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 607

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
      "id": "3ffd7cd0-7cd0-3ffd-d07c-fd3fd07cfd3f",
      "name": "Name value",
      "description": "Description value",
      "platforms": "macOS",
      "technologies": "mdm",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "settingCount": 12,
      "creationSource": "Creation Source value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "isAssigned": true
    }
  ]
}
```




