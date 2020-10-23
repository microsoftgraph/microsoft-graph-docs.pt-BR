---
title: Obter groupPolicySettingMapping
description: Leia as propriedades e as relações do objeto groupPolicySettingMapping.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 853ea77d43a44de192ba62e6248f2fc59db9ba78
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692958"
---
# <a name="get-grouppolicysettingmapping"></a><span data-ttu-id="f2a5e-103">Obter groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="f2a5e-103">Get groupPolicySettingMapping</span></span>

<span data-ttu-id="f2a5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2a5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2a5e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2a5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2a5e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2a5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2a5e-107">Leia as propriedades e as relações do objeto [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="f2a5e-107">Read properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2a5e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2a5e-108">Prerequisites</span></span>
<span data-ttu-id="f2a5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2a5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2a5e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2a5e-111">Permission type</span></span>|<span data-ttu-id="f2a5e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2a5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2a5e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2a5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2a5e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2a5e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f2a5e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2a5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2a5e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2a5e-116">Not supported.</span></span>|
|<span data-ttu-id="f2a5e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2a5e-117">Application</span></span>|<span data-ttu-id="f2a5e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2a5e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2a5e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2a5e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2a5e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f2a5e-120">Optional query parameters</span></span>
<span data-ttu-id="f2a5e-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f2a5e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2a5e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a5e-122">Request headers</span></span>
|<span data-ttu-id="f2a5e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2a5e-123">Header</span></span>|<span data-ttu-id="f2a5e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f2a5e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2a5e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2a5e-125">Authorization</span></span>|<span data-ttu-id="f2a5e-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2a5e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2a5e-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2a5e-127">Accept</span></span>|<span data-ttu-id="f2a5e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f2a5e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2a5e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a5e-129">Request body</span></span>
<span data-ttu-id="f2a5e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2a5e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2a5e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2a5e-131">Response</span></span>
<span data-ttu-id="f2a5e-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2a5e-132">If successful, this method returns a `200 OK` response code and [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2a5e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2a5e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2a5e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a5e-134">Request</span></span>
<span data-ttu-id="f2a5e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2a5e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

### <a name="response"></a><span data-ttu-id="f2a5e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2a5e-136">Response</span></span>
<span data-ttu-id="f2a5e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2a5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1143

{
  "value": {
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
}
```





