---
title: Listar windows81GeneralConfigurations
description: Listar propriedades e relações dos objetos windows81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b85c7685c00c3a58180e8e8811eae7970a54867f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759181"
---
# <a name="list-windows81generalconfigurations"></a><span data-ttu-id="4565f-103">Listar windows81GeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="4565f-103">List windows81GeneralConfigurations</span></span>

<span data-ttu-id="4565f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4565f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4565f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4565f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4565f-106">Listar propriedades e relações dos objetos [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4565f-106">List properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4565f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4565f-107">Prerequisites</span></span>
<span data-ttu-id="4565f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4565f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4565f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4565f-110">Permission type</span></span>|<span data-ttu-id="4565f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4565f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4565f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4565f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4565f-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4565f-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4565f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4565f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4565f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4565f-115">Not supported.</span></span>|
|<span data-ttu-id="4565f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4565f-116">Application</span></span>|<span data-ttu-id="4565f-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4565f-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4565f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4565f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4565f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4565f-119">Request headers</span></span>
|<span data-ttu-id="4565f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4565f-120">Header</span></span>|<span data-ttu-id="4565f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4565f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4565f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4565f-122">Authorization</span></span>|<span data-ttu-id="4565f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4565f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4565f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4565f-124">Accept</span></span>|<span data-ttu-id="4565f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4565f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4565f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4565f-126">Request body</span></span>
<span data-ttu-id="4565f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4565f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4565f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4565f-128">Response</span></span>
<span data-ttu-id="4565f-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4565f-129">If successful, this method returns a `200 OK` response code and a collection of [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4565f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4565f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4565f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4565f-131">Request</span></span>
<span data-ttu-id="4565f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4565f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4565f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4565f-133">Response</span></span>
<span data-ttu-id="4565f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4565f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




