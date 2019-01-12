---
title: Listar windows81GeneralConfigurations
description: Listar propriedades e relações dos objetos windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 219ca47840efe36bbe9ebd00ad92669a1a76391b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924129"
---
# <a name="list-windows81generalconfigurations"></a><span data-ttu-id="dbeea-103">Listar windows81GeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="dbeea-103">List windows81GeneralConfigurations</span></span>

> <span data-ttu-id="dbeea-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dbeea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbeea-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dbeea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dbeea-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dbeea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbeea-107">Listar propriedades e relações dos objetos [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dbeea-107">List properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dbeea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dbeea-108">Prerequisites</span></span>
<span data-ttu-id="dbeea-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbeea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbeea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbeea-111">Permission type</span></span>|<span data-ttu-id="dbeea-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dbeea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbeea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbeea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dbeea-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbeea-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dbeea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbeea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbeea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbeea-116">Not supported.</span></span>|
|<span data-ttu-id="dbeea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbeea-117">Application</span></span>|<span data-ttu-id="dbeea-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbeea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbeea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbeea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dbeea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbeea-120">Request headers</span></span>
|<span data-ttu-id="dbeea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dbeea-121">Header</span></span>|<span data-ttu-id="dbeea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dbeea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbeea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbeea-123">Authorization</span></span>|<span data-ttu-id="dbeea-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbeea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbeea-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dbeea-125">Accept</span></span>|<span data-ttu-id="dbeea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dbeea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbeea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbeea-127">Request body</span></span>
<span data-ttu-id="dbeea-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dbeea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbeea-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbeea-129">Response</span></span>
<span data-ttu-id="dbeea-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbeea-130">If successful, this method returns a `200 OK` response code and a collection of [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbeea-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbeea-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="dbeea-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbeea-132">Request</span></span>
<span data-ttu-id="dbeea-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbeea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="dbeea-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbeea-134">Response</span></span>
<span data-ttu-id="dbeea-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbeea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2313

{
  "value": [
    {
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
  ]
}
```





