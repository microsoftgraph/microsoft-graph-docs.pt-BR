---
title: Obter androidWorkProfileGeneralDeviceConfiguration
description: Leia propriedades e relações do objeto androidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2b6f0c1591640cd9b36f64f0ccf8846b02af1741
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753976"
---
# <a name="get-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="7c5da-103">Obter androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c5da-103">Get androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="7c5da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c5da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c5da-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c5da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c5da-106">Leia propriedades e relações do [objeto androidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c5da-106">Read properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c5da-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c5da-107">Prerequisites</span></span>
<span data-ttu-id="7c5da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c5da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c5da-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c5da-110">Permission type</span></span>|<span data-ttu-id="7c5da-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c5da-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c5da-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c5da-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c5da-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c5da-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c5da-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c5da-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c5da-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c5da-115">Not supported.</span></span>|
|<span data-ttu-id="7c5da-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c5da-116">Application</span></span>|<span data-ttu-id="7c5da-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c5da-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c5da-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c5da-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c5da-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7c5da-119">Optional query parameters</span></span>
<span data-ttu-id="7c5da-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7c5da-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c5da-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c5da-121">Request headers</span></span>
|<span data-ttu-id="7c5da-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c5da-122">Header</span></span>|<span data-ttu-id="7c5da-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7c5da-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c5da-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c5da-124">Authorization</span></span>|<span data-ttu-id="7c5da-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c5da-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c5da-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c5da-126">Accept</span></span>|<span data-ttu-id="7c5da-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7c5da-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c5da-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c5da-128">Request body</span></span>
<span data-ttu-id="7c5da-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c5da-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c5da-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c5da-130">Response</span></span>
<span data-ttu-id="7c5da-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c5da-131">If successful, this method returns a `200 OK` response code and [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c5da-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c5da-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c5da-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c5da-133">Request</span></span>
<span data-ttu-id="7c5da-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c5da-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="7c5da-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c5da-135">Response</span></span>
<span data-ttu-id="7c5da-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c5da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2104

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
    "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "passwordBlockFingerprintUnlock": true,
    "passwordBlockTrustAgents": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "passwordRequiredType": "lowSecurityBiometric",
    "workProfileDataSharingType": "preventAny",
    "workProfileBlockNotificationsWhileDeviceLocked": true,
    "workProfileBlockAddingAccounts": true,
    "workProfileBluetoothEnableContactSharing": true,
    "workProfileBlockScreenCapture": true,
    "workProfileBlockCrossProfileCallerId": true,
    "workProfileBlockCamera": true,
    "workProfileBlockCrossProfileContactsSearch": true,
    "workProfileBlockCrossProfileCopyPaste": true,
    "workProfileDefaultAppPermissionPolicy": "prompt",
    "workProfilePasswordBlockFingerprintUnlock": true,
    "workProfilePasswordBlockTrustAgents": true,
    "workProfilePasswordExpirationDays": 1,
    "workProfilePasswordMinimumLength": 0,
    "workProfilePasswordMinNumericCharacters": 7,
    "workProfilePasswordMinNonLetterCharacters": 9,
    "workProfilePasswordMinLetterCharacters": 6,
    "workProfilePasswordMinLowerCaseCharacters": 9,
    "workProfilePasswordMinUpperCaseCharacters": 9,
    "workProfilePasswordMinSymbolCharacters": 6,
    "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
    "workProfilePasswordPreviousPasswordBlockCount": 13,
    "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
    "workProfilePasswordRequiredType": "lowSecurityBiometric",
    "workProfileRequirePassword": true,
    "securityRequireVerifyApps": true
  }
}
```




