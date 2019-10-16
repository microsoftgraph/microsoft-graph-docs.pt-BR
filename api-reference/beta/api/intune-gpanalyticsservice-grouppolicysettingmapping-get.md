---
title: Obter groupPolicySettingMapping
description: Leia as propriedades e as relações do objeto groupPolicySettingMapping.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 318ec1c0d2fc4827097eb552eae7a3fa73fa46ab
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535757"
---
# <a name="get-grouppolicysettingmapping"></a><span data-ttu-id="65597-103">Obter groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="65597-103">Get groupPolicySettingMapping</span></span>

> <span data-ttu-id="65597-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65597-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65597-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65597-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65597-106">Leia as propriedades e as relações do objeto [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="65597-106">Read properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65597-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="65597-107">Prerequisites</span></span>
<span data-ttu-id="65597-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65597-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65597-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65597-110">Permission type</span></span>|<span data-ttu-id="65597-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="65597-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65597-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65597-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65597-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="65597-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="65597-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65597-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65597-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65597-115">Not supported.</span></span>|
|<span data-ttu-id="65597-116">Application</span><span class="sxs-lookup"><span data-stu-id="65597-116">Application</span></span>|<span data-ttu-id="65597-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="65597-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65597-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65597-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="65597-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="65597-119">Optional query parameters</span></span>
<span data-ttu-id="65597-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="65597-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65597-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65597-121">Request headers</span></span>
|<span data-ttu-id="65597-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65597-122">Header</span></span>|<span data-ttu-id="65597-123">Valor</span><span class="sxs-lookup"><span data-stu-id="65597-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65597-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="65597-124">Authorization</span></span>|<span data-ttu-id="65597-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65597-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65597-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="65597-126">Accept</span></span>|<span data-ttu-id="65597-127">application/json</span><span class="sxs-lookup"><span data-stu-id="65597-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65597-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65597-128">Request body</span></span>
<span data-ttu-id="65597-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="65597-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65597-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="65597-130">Response</span></span>
<span data-ttu-id="65597-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65597-131">If successful, this method returns a `200 OK` response code and [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65597-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65597-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="65597-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65597-133">Request</span></span>
<span data-ttu-id="65597-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65597-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

### <a name="response"></a><span data-ttu-id="65597-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="65597-135">Response</span></span>
<span data-ttu-id="65597-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65597-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 964

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
    "settingScope": "device",
    "intuneSettingUriList": [
      "Intune Setting Uri List value"
    ]
  }
}
```






