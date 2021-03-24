---
title: Obter groupPolicyMigrationReport
description: Ler propriedades e relações do objeto groupPolicyMigrationReport.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 59ca750739de420f27f49ae387a31ce277013fb1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135548"
---
# <a name="get-grouppolicymigrationreport"></a><span data-ttu-id="0d2b8-103">Obter groupPolicyMigrationReport</span><span class="sxs-lookup"><span data-stu-id="0d2b8-103">Get groupPolicyMigrationReport</span></span>

<span data-ttu-id="0d2b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d2b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d2b8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0d2b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d2b8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0d2b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d2b8-107">Ler propriedades e relações do [objeto groupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)</span><span class="sxs-lookup"><span data-stu-id="0d2b8-107">Read properties and relationships of the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d2b8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0d2b8-108">Prerequisites</span></span>
<span data-ttu-id="0d2b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d2b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d2b8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d2b8-111">Permission type</span></span>|<span data-ttu-id="0d2b8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d2b8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d2b8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d2b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d2b8-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d2b8-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d2b8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d2b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d2b8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d2b8-116">Not supported.</span></span>|
|<span data-ttu-id="0d2b8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d2b8-117">Application</span></span>|<span data-ttu-id="0d2b8-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d2b8-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d2b8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d2b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0d2b8-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0d2b8-120">Optional query parameters</span></span>
<span data-ttu-id="0d2b8-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0d2b8-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d2b8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d2b8-122">Request headers</span></span>
|<span data-ttu-id="0d2b8-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0d2b8-123">Header</span></span>|<span data-ttu-id="0d2b8-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0d2b8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d2b8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d2b8-125">Authorization</span></span>|<span data-ttu-id="0d2b8-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d2b8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d2b8-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0d2b8-127">Accept</span></span>|<span data-ttu-id="0d2b8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0d2b8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d2b8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d2b8-129">Request body</span></span>
<span data-ttu-id="0d2b8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d2b8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d2b8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d2b8-131">Response</span></span>
<span data-ttu-id="0d2b8-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d2b8-132">If successful, this method returns a `200 OK` response code and [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d2b8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d2b8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d2b8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d2b8-134">Request</span></span>
<span data-ttu-id="0d2b8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d2b8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

### <a name="response"></a><span data-ttu-id="0d2b8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d2b8-136">Response</span></span>
<span data-ttu-id="0d2b8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d2b8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




