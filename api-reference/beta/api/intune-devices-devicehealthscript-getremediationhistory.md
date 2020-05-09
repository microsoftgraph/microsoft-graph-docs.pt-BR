---
title: função getRemediationHistory
description: Função para obter o número de correções por scripts de integridade do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5469f8c5c4ae35d69e92b6d1e007bf4a0b3703ea
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44176978"
---
# <a name="getremediationhistory-function"></a><span data-ttu-id="7ed66-103">função getRemediationHistory</span><span class="sxs-lookup"><span data-stu-id="7ed66-103">getRemediationHistory function</span></span>

<span data-ttu-id="7ed66-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ed66-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ed66-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ed66-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ed66-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ed66-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ed66-107">Função para obter o número de correções por scripts de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7ed66-107">Function to get the number of remediations by a device health scripts</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ed66-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ed66-108">Prerequisites</span></span>
<span data-ttu-id="7ed66-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ed66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ed66-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ed66-111">Permission type</span></span>|<span data-ttu-id="7ed66-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ed66-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ed66-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ed66-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ed66-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ed66-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7ed66-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ed66-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ed66-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ed66-116">Not supported.</span></span>|
|<span data-ttu-id="7ed66-117">Application</span><span class="sxs-lookup"><span data-stu-id="7ed66-117">Application</span></span>|<span data-ttu-id="7ed66-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ed66-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ed66-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ed66-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getRemediationHistory
```

## <a name="request-headers"></a><span data-ttu-id="7ed66-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed66-120">Request headers</span></span>
|<span data-ttu-id="7ed66-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ed66-121">Header</span></span>|<span data-ttu-id="7ed66-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7ed66-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ed66-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ed66-123">Authorization</span></span>|<span data-ttu-id="7ed66-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ed66-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ed66-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7ed66-125">Accept</span></span>|<span data-ttu-id="7ed66-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ed66-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ed66-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed66-127">Request body</span></span>
<span data-ttu-id="7ed66-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ed66-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ed66-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ed66-129">Response</span></span>
<span data-ttu-id="7ed66-130">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um [deviceHealthScriptRemediationHistory](../resources/intune-devices-devicehealthscriptremediationhistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ed66-130">If successful, this function returns a `200 OK` response code and a [deviceHealthScriptRemediationHistory](../resources/intune-devices-devicehealthscriptremediationhistory.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ed66-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ed66-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ed66-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed66-132">Request</span></span>
<span data-ttu-id="7ed66-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ed66-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getRemediationHistory
```

### <a name="response"></a><span data-ttu-id="7ed66-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ed66-134">Response</span></span>
<span data-ttu-id="7ed66-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ed66-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 397

{
  "value": {
    "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistory",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "historyData": [
      {
        "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData",
        "date": "2016-12-31",
        "remediatedDeviceCount": 5,
        "noIssueDeviceCount": 2
      }
    ]
  }
}
```



