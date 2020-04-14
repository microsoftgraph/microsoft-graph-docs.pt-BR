---
title: Listar deviceConfigurationConflictSummaries
description: Listar Propriedades e relações dos objetos Propriedadesdeviceconfigurationconflictsummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8bd58b6bb5f74c73f08948443ce9f2c042320a74
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433553"
---
# <a name="list-deviceconfigurationconflictsummaries"></a><span data-ttu-id="e4e8d-103">Listar deviceConfigurationConflictSummaries</span><span class="sxs-lookup"><span data-stu-id="e4e8d-103">List deviceConfigurationConflictSummaries</span></span>

<span data-ttu-id="e4e8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4e8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4e8d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4e8d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4e8d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4e8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4e8d-107">Listar Propriedades e relações dos objetos [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e4e8d-107">List properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4e8d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4e8d-108">Prerequisites</span></span>
<span data-ttu-id="e4e8d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4e8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4e8d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4e8d-111">Permission type</span></span>|<span data-ttu-id="e4e8d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4e8d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4e8d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4e8d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4e8d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4e8d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e4e8d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4e8d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4e8d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4e8d-116">Not supported.</span></span>|
|<span data-ttu-id="e4e8d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4e8d-117">Application</span></span>|<span data-ttu-id="e4e8d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4e8d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4e8d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4e8d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="e4e8d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4e8d-120">Request headers</span></span>
|<span data-ttu-id="e4e8d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4e8d-121">Header</span></span>|<span data-ttu-id="e4e8d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e4e8d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4e8d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4e8d-123">Authorization</span></span>|<span data-ttu-id="e4e8d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4e8d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4e8d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4e8d-125">Accept</span></span>|<span data-ttu-id="e4e8d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4e8d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4e8d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4e8d-127">Request body</span></span>
<span data-ttu-id="e4e8d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4e8d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4e8d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4e8d-129">Response</span></span>
<span data-ttu-id="e4e8d-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4e8d-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4e8d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4e8d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4e8d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4e8d-132">Request</span></span>
<span data-ttu-id="e4e8d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4e8d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
```

### <a name="response"></a><span data-ttu-id="e4e8d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4e8d-134">Response</span></span>
<span data-ttu-id="e4e8d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4e8d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 495

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
      "conflictingDeviceConfigurations": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
      "contributingSettings": [
        "Contributing Settings value"
      ],
      "deviceCheckinsImpacted": 6
    }
  ]
}
```



