---
title: Obter securityConfigurationTask
description: Leia as propriedades e as relações do objeto securityConfigurationTask.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6403cc544dfca382d15e658a31cb8133132f2076
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793179"
---
# <a name="get-securityconfigurationtask"></a><span data-ttu-id="390a5-103">Obter securityConfigurationTask</span><span class="sxs-lookup"><span data-stu-id="390a5-103">Get securityConfigurationTask</span></span>

<span data-ttu-id="390a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="390a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="390a5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="390a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="390a5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="390a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="390a5-107">Leia as propriedades e as relações do objeto [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) .</span><span class="sxs-lookup"><span data-stu-id="390a5-107">Read properties and relationships of the [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="390a5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="390a5-108">Prerequisites</span></span>
<span data-ttu-id="390a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="390a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="390a5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="390a5-111">Permission type</span></span>|<span data-ttu-id="390a5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="390a5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="390a5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="390a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="390a5-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="390a5-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="390a5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="390a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="390a5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="390a5-116">Not supported.</span></span>|
|<span data-ttu-id="390a5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="390a5-117">Application</span></span>|<span data-ttu-id="390a5-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="390a5-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="390a5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="390a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="390a5-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="390a5-120">Optional query parameters</span></span>
<span data-ttu-id="390a5-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="390a5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="390a5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="390a5-122">Request headers</span></span>
|<span data-ttu-id="390a5-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="390a5-123">Header</span></span>|<span data-ttu-id="390a5-124">Valor</span><span class="sxs-lookup"><span data-stu-id="390a5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="390a5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="390a5-125">Authorization</span></span>|<span data-ttu-id="390a5-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="390a5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="390a5-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="390a5-127">Accept</span></span>|<span data-ttu-id="390a5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="390a5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="390a5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="390a5-129">Request body</span></span>
<span data-ttu-id="390a5-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="390a5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="390a5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="390a5-131">Response</span></span>
<span data-ttu-id="390a5-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="390a5-132">If successful, this method returns a `200 OK` response code and [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="390a5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="390a5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="390a5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="390a5-134">Request</span></span>
<span data-ttu-id="390a5-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="390a5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

### <a name="response"></a><span data-ttu-id="390a5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="390a5-136">Response</span></span>
<span data-ttu-id="390a5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="390a5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 921

{
  "value": {
    "@odata.type": "#microsoft.graph.securityConfigurationTask",
    "id": "5d630f12-0f12-5d63-120f-635d120f635d",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
    "category": "advancedThreatProtection",
    "priority": "high",
    "creator": "Creator value",
    "creatorNotes": "Creator Notes value",
    "assignedTo": "Assigned To value",
    "status": "pending",
    "endpointSecurityPolicy": "antivirus",
    "applicablePlatform": "macOS",
    "endpointSecurityPolicyProfile": "antivirus",
    "insights": "Insights value",
    "managedDeviceCount": 2,
    "intendedSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ]
  }
}
```


