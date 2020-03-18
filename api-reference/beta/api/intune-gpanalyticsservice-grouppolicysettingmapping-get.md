---
title: Obter groupPolicySettingMapping
description: Leia as propriedades e as relações do objeto groupPolicySettingMapping.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d57a719a2bbefb0eb6df1196d4f9d62c7b1db5a0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804587"
---
# <a name="get-grouppolicysettingmapping"></a><span data-ttu-id="47f89-103">Obter groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="47f89-103">Get groupPolicySettingMapping</span></span>

> <span data-ttu-id="47f89-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47f89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47f89-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47f89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47f89-106">Leia as propriedades e as relações do objeto [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="47f89-106">Read properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47f89-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47f89-107">Prerequisites</span></span>
<span data-ttu-id="47f89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47f89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47f89-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47f89-110">Permission type</span></span>|<span data-ttu-id="47f89-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47f89-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47f89-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47f89-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47f89-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="47f89-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="47f89-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47f89-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47f89-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47f89-115">Not supported.</span></span>|
|<span data-ttu-id="47f89-116">Application</span><span class="sxs-lookup"><span data-stu-id="47f89-116">Application</span></span>|<span data-ttu-id="47f89-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="47f89-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47f89-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47f89-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47f89-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="47f89-119">Optional query parameters</span></span>
<span data-ttu-id="47f89-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="47f89-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47f89-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47f89-121">Request headers</span></span>
|<span data-ttu-id="47f89-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47f89-122">Header</span></span>|<span data-ttu-id="47f89-123">Valor</span><span class="sxs-lookup"><span data-stu-id="47f89-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47f89-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="47f89-124">Authorization</span></span>|<span data-ttu-id="47f89-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47f89-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47f89-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47f89-126">Accept</span></span>|<span data-ttu-id="47f89-127">application/json</span><span class="sxs-lookup"><span data-stu-id="47f89-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47f89-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47f89-128">Request body</span></span>
<span data-ttu-id="47f89-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47f89-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47f89-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="47f89-130">Response</span></span>
<span data-ttu-id="47f89-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47f89-131">If successful, this method returns a `200 OK` response code and [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47f89-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47f89-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="47f89-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47f89-133">Request</span></span>
<span data-ttu-id="47f89-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47f89-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

### <a name="response"></a><span data-ttu-id="47f89-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="47f89-135">Response</span></span>
<span data-ttu-id="47f89-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47f89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1075

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
    "intuneSettingDefinitionId": "Intune Setting Definition Id value"
  }
}
```




