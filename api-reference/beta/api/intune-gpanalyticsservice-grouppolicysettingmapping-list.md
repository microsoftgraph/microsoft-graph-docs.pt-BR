---
title: Listar groupPolicySettingMappings
description: Listar Propriedades e relações dos objetos groupPolicySettingMapping.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 81b0189fc01c539458cf2eb311150983887087ef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48043308"
---
# <a name="list-grouppolicysettingmappings"></a><span data-ttu-id="6b9cb-103">Listar groupPolicySettingMappings</span><span class="sxs-lookup"><span data-stu-id="6b9cb-103">List groupPolicySettingMappings</span></span>

<span data-ttu-id="6b9cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b9cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b9cb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b9cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b9cb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b9cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b9cb-107">Listar Propriedades e relações dos objetos [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="6b9cb-107">List properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b9cb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b9cb-108">Prerequisites</span></span>
<span data-ttu-id="6b9cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b9cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b9cb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b9cb-111">Permission type</span></span>|<span data-ttu-id="6b9cb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6b9cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b9cb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b9cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b9cb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b9cb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6b9cb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b9cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b9cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b9cb-116">Not supported.</span></span>|
|<span data-ttu-id="6b9cb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b9cb-117">Application</span></span>|<span data-ttu-id="6b9cb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b9cb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b9cb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b9cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## <a name="request-headers"></a><span data-ttu-id="6b9cb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b9cb-120">Request headers</span></span>
|<span data-ttu-id="6b9cb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b9cb-121">Header</span></span>|<span data-ttu-id="6b9cb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6b9cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b9cb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b9cb-123">Authorization</span></span>|<span data-ttu-id="6b9cb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b9cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b9cb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b9cb-125">Accept</span></span>|<span data-ttu-id="6b9cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b9cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b9cb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b9cb-127">Request body</span></span>
<span data-ttu-id="6b9cb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b9cb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b9cb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b9cb-129">Response</span></span>
<span data-ttu-id="6b9cb-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b9cb-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b9cb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b9cb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b9cb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b9cb-132">Request</span></span>
<span data-ttu-id="6b9cb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b9cb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

### <a name="response"></a><span data-ttu-id="6b9cb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b9cb-134">Response</span></span>
<span data-ttu-id="6b9cb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b9cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1209

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
      "id": "8fa04560-4560-8fa0-6045-a08f6045a08f",
      "parentId": "Parent Id value",
      "childIdList": [
        "Child Id List value"
      ],
      "settingName": "Setting Name value",
      "settingValue": "Setting Value value",
      "settingValueType": "Setting Value Type value",
      "settingDisplayName": "Setting Display Name value",
      "settingDisplayValue": "Setting Display Value value",
      "settingDisplayValueType": "Setting Display Value Type value",
      "settingValueDisplayUnits": "Setting Value Display Units value",
      "settingCategory": "Setting Category value",
      "mdmCspName": "Mdm Csp Name value",
      "mdmSettingUri": "Mdm Setting Uri value",
      "mdmMinimumOSVersion": 3,
      "settingType": "policy",
      "isMdmSupported": true,
      "mdmSupportedState": "supported",
      "settingScope": "device",
      "intuneSettingUriList": [
        "Intune Setting Uri List value"
      ],
      "intuneSettingDefinitionId": "Intune Setting Definition Id value",
      "admxSettingDefinitionId": "Admx Setting Definition Id value"
    }
  ]
}
```






