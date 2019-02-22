---
title: Obter windows81GeneralConfiguration
description: Ler propriedades e relações do objeto windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f77092d054f6fee6c9987384ebd11efd354101ac
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165475"
---
# <a name="get-windows81generalconfiguration"></a><span data-ttu-id="c7d5c-103">Obter windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7d5c-103">Get windows81GeneralConfiguration</span></span>

> <span data-ttu-id="c7d5c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7d5c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7d5c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7d5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7d5c-106">Ler propriedades e relações do objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7d5c-106">Read properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7d5c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7d5c-107">Prerequisites</span></span>
<span data-ttu-id="c7d5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c7d5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c7d5c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7d5c-110">Permission type</span></span>|<span data-ttu-id="c7d5c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7d5c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7d5c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7d5c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7d5c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7d5c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c7d5c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7d5c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7d5c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7d5c-115">Not supported.</span></span>|
|<span data-ttu-id="c7d5c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7d5c-116">Application</span></span>|<span data-ttu-id="c7d5c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7d5c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7d5c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7d5c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7d5c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c7d5c-119">Optional query parameters</span></span>
<span data-ttu-id="c7d5c-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c7d5c-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7d5c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d5c-121">Request headers</span></span>
|<span data-ttu-id="c7d5c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7d5c-122">Header</span></span>|<span data-ttu-id="c7d5c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c7d5c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7d5c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7d5c-124">Authorization</span></span>|<span data-ttu-id="c7d5c-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7d5c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7d5c-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7d5c-126">Accept</span></span>|<span data-ttu-id="c7d5c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c7d5c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7d5c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d5c-128">Request body</span></span>
<span data-ttu-id="c7d5c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7d5c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7d5c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7d5c-130">Response</span></span>
<span data-ttu-id="c7d5c-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7d5c-131">If successful, this method returns a `200 OK` response code and [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7d5c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7d5c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7d5c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d5c-133">Request</span></span>
<span data-ttu-id="c7d5c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7d5c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c7d5c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7d5c-135">Response</span></span>
<span data-ttu-id="c7d5c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7d5c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2207

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
    "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "accountsBlockAddingNonMicrosoftAccountEmail": true,
    "applyOnlyToWindows81": true,
    "browserBlockAutofill": true,
    "browserBlockAutomaticDetectionOfIntranetSites": true,
    "browserBlockEnterpriseModeAccess": true,
    "browserBlockJavaScript": true,
    "browserBlockPlugins": true,
    "browserBlockPopups": true,
    "browserBlockSendingDoNotTrackHeader": true,
    "browserBlockSingleWordEntryOnIntranetSites": true,
    "browserRequireSmartScreen": true,
    "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
    "browserInternetSecurityLevel": "medium",
    "browserIntranetSecurityLevel": "low",
    "browserLoggingReportLocation": "Browser Logging Report Location value",
    "browserRequireHighSecurityForRestrictedSites": true,
    "browserRequireFirewall": true,
    "browserRequireFraudWarning": true,
    "browserTrustedSitesSecurityLevel": "low",
    "cellularBlockDataRoaming": true,
    "diagnosticsBlockDataSubmission": true,
    "passwordBlockPicturePasswordAndPin": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordMinimumCharacterSetCount": 0,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequiredType": "alphanumeric",
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "storageRequireDeviceEncryption": true,
    "minimumAutoInstallClassification": "recommendedAndImportant",
    "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
    "updatesRequireAutomaticUpdates": true,
    "userAccountControlSettings": "alwaysNotify",
    "workFoldersUrl": "https://example.com/workFoldersUrl/"
  }
}
```




