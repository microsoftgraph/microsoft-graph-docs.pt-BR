---
title: Obter windows81GeneralConfiguration
description: Ler propriedades e relações do objeto windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2dec869e420fbb7ab4eefa328760ec05f6ded14e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020028"
---
# <a name="get-windows81generalconfiguration"></a><span data-ttu-id="a14c7-103">Obter windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="a14c7-103">Get windows81GeneralConfiguration</span></span>

> <span data-ttu-id="a14c7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a14c7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a14c7-105">Ler propriedades e relações do objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a14c7-105">Read properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a14c7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a14c7-106">Prerequisites</span></span>
<span data-ttu-id="a14c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a14c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a14c7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a14c7-109">Permission type</span></span>|<span data-ttu-id="a14c7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a14c7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a14c7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a14c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a14c7-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a14c7-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a14c7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a14c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a14c7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a14c7-114">Not supported.</span></span>|
|<span data-ttu-id="a14c7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a14c7-115">Application</span></span>|<span data-ttu-id="a14c7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a14c7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a14c7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a14c7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a14c7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a14c7-118">Optional query parameters</span></span>
<span data-ttu-id="a14c7-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a14c7-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a14c7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a14c7-120">Request headers</span></span>
|<span data-ttu-id="a14c7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a14c7-121">Header</span></span>|<span data-ttu-id="a14c7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a14c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a14c7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a14c7-123">Authorization</span></span>|<span data-ttu-id="a14c7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a14c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a14c7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a14c7-125">Accept</span></span>|<span data-ttu-id="a14c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a14c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a14c7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a14c7-127">Request body</span></span>
<span data-ttu-id="a14c7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a14c7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a14c7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a14c7-129">Response</span></span>
<span data-ttu-id="a14c7-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a14c7-130">If successful, this method returns a `200 OK` response code and [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a14c7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a14c7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a14c7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a14c7-132">Request</span></span>
<span data-ttu-id="a14c7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a14c7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a14c7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a14c7-134">Response</span></span>
<span data-ttu-id="a14c7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a14c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1964

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
    "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
    "updatesRequireAutomaticUpdates": true,
    "userAccountControlSettings": "alwaysNotify",
    "workFoldersUrl": "https://example.com/workFoldersUrl/"
  }
}
```



