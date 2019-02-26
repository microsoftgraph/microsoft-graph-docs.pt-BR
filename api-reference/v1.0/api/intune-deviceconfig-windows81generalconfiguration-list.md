---
title: Listar windows81GeneralConfigurations
description: Listar propriedades e relações dos objetos windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0f9e7886b3bb9ce16442162d3c797ba087db042
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262647"
---
# <a name="list-windows81generalconfigurations"></a><span data-ttu-id="d8483-103">Listar windows81GeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="d8483-103">List windows81GeneralConfigurations</span></span>

> <span data-ttu-id="d8483-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8483-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8483-105">Listar propriedades e relações dos objetos [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8483-105">List properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8483-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8483-106">Prerequisites</span></span>
<span data-ttu-id="d8483-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d8483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d8483-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8483-109">Permission type</span></span>|<span data-ttu-id="d8483-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8483-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8483-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8483-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d8483-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8483-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d8483-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8483-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8483-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8483-114">Not supported.</span></span>|
|<span data-ttu-id="d8483-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8483-115">Application</span></span>|<span data-ttu-id="d8483-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8483-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8483-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8483-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d8483-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8483-118">Request headers</span></span>
|<span data-ttu-id="d8483-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8483-119">Header</span></span>|<span data-ttu-id="d8483-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d8483-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8483-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8483-121">Authorization</span></span>|<span data-ttu-id="d8483-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8483-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8483-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8483-123">Accept</span></span>|<span data-ttu-id="d8483-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d8483-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8483-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8483-125">Request body</span></span>
<span data-ttu-id="d8483-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8483-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8483-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8483-127">Response</span></span>
<span data-ttu-id="d8483-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8483-128">If successful, this method returns a `200 OK` response code and a collection of [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8483-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8483-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8483-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8483-130">Request</span></span>
<span data-ttu-id="d8483-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8483-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d8483-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8483-132">Response</span></span>
<span data-ttu-id="d8483-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8483-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2058

{
  "value": [
    {
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
  ]
}
```



