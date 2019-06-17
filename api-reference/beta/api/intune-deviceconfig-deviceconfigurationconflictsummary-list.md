---
title: Listar deviceConfigurationConflictSummaries
description: Listar Propriedades e relações dos objetos Propriedadesdeviceconfigurationconflictsummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29060dba640a686664bfdce2f00a422870b0ad6a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967780"
---
# <a name="list-deviceconfigurationconflictsummaries"></a><span data-ttu-id="5f964-103">Listar deviceConfigurationConflictSummaries</span><span class="sxs-lookup"><span data-stu-id="5f964-103">List deviceConfigurationConflictSummaries</span></span>

> <span data-ttu-id="5f964-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5f964-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f964-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f964-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f964-106">Listar Propriedades e relações dos objetos [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="5f964-106">List properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f964-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5f964-107">Prerequisites</span></span>
<span data-ttu-id="5f964-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f964-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f964-110">Permission type</span></span>|<span data-ttu-id="5f964-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5f964-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f964-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f964-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f964-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f964-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5f964-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f964-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f964-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f964-115">Not supported.</span></span>|
|<span data-ttu-id="5f964-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f964-116">Application</span></span>|<span data-ttu-id="5f964-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f964-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f964-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f964-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="5f964-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f964-119">Request headers</span></span>
|<span data-ttu-id="5f964-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f964-120">Header</span></span>|<span data-ttu-id="5f964-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5f964-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f964-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f964-122">Authorization</span></span>|<span data-ttu-id="5f964-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f964-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f964-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5f964-124">Accept</span></span>|<span data-ttu-id="5f964-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f964-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f964-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f964-126">Request body</span></span>
<span data-ttu-id="5f964-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f964-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f964-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f964-128">Response</span></span>
<span data-ttu-id="5f964-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f964-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f964-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f964-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f964-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f964-131">Request</span></span>
<span data-ttu-id="5f964-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f964-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
```

### <a name="response"></a><span data-ttu-id="5f964-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f964-133">Response</span></span>
<span data-ttu-id="5f964-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f964-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





