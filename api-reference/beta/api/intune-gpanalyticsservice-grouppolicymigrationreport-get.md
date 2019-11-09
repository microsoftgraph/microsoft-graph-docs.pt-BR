---
title: Obter groupPolicyMigrationReport
description: Leia as propriedades e as relações do objeto groupPolicyMigrationReport.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: acff13fd92448131d4112b9217e87f0b9e23d511
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087114"
---
# <a name="get-grouppolicymigrationreport"></a><span data-ttu-id="40547-103">Obter groupPolicyMigrationReport</span><span class="sxs-lookup"><span data-stu-id="40547-103">Get groupPolicyMigrationReport</span></span>

> <span data-ttu-id="40547-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40547-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40547-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40547-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40547-106">Leia as propriedades e as relações do objeto [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .</span><span class="sxs-lookup"><span data-stu-id="40547-106">Read properties and relationships of the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40547-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40547-107">Prerequisites</span></span>
<span data-ttu-id="40547-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40547-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40547-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40547-110">Permission type</span></span>|<span data-ttu-id="40547-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40547-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40547-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40547-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40547-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="40547-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="40547-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40547-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40547-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40547-115">Not supported.</span></span>|
|<span data-ttu-id="40547-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40547-116">Application</span></span>|<span data-ttu-id="40547-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="40547-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40547-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40547-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40547-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="40547-119">Optional query parameters</span></span>
<span data-ttu-id="40547-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="40547-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40547-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40547-121">Request headers</span></span>
|<span data-ttu-id="40547-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40547-122">Header</span></span>|<span data-ttu-id="40547-123">Valor</span><span class="sxs-lookup"><span data-stu-id="40547-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40547-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="40547-124">Authorization</span></span>|<span data-ttu-id="40547-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40547-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40547-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40547-126">Accept</span></span>|<span data-ttu-id="40547-127">application/json</span><span class="sxs-lookup"><span data-stu-id="40547-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40547-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40547-128">Request body</span></span>
<span data-ttu-id="40547-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40547-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40547-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="40547-130">Response</span></span>
<span data-ttu-id="40547-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40547-131">If successful, this method returns a `200 OK` response code and [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40547-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40547-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="40547-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40547-133">Request</span></span>
<span data-ttu-id="40547-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40547-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

### <a name="response"></a><span data-ttu-id="40547-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="40547-135">Response</span></span>
<span data-ttu-id="40547-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40547-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
    "id": "60663fa8-3fa8-6066-a83f-6660a83f6660",
    "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
    "displayName": "Display Name value",
    "ouDistinguishedName": "Ou Distinguished Name value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
    "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
    "migrationReadiness": "partial",
    "targetedInActiveDirectory": true,
    "totalSettingsCount": 2,
    "supportedSettingsCount": 6,
    "supportedSettingsPercent": 8
  }
}
```






