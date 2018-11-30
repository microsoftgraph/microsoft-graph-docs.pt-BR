---
title: Obter androidWorkProfileGeneralDeviceConfiguration
description: Leia as propriedades e os relacionamentos do objeto androidWorkProfileGeneralDeviceConfiguration.
ms.openlocfilehash: bdb7d9ff8d4707b3ac34ad77c945d09538c4b740
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005400"
---
# <a name="get-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="32f62-103">Obter androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="32f62-103">Get androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="32f62-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="32f62-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32f62-105">Leia as propriedades e os relacionamentos do objeto [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="32f62-105">Read properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32f62-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32f62-106">Prerequisites</span></span>
<span data-ttu-id="32f62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32f62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32f62-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32f62-109">Permission type</span></span>|<span data-ttu-id="32f62-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="32f62-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32f62-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32f62-111">Delegated (work or school account)</span></span>|<span data-ttu-id="32f62-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="32f62-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="32f62-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32f62-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32f62-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32f62-114">Not supported.</span></span>|
|<span data-ttu-id="32f62-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32f62-115">Application</span></span>|<span data-ttu-id="32f62-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32f62-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32f62-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32f62-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32f62-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="32f62-118">Optional query parameters</span></span>
<span data-ttu-id="32f62-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="32f62-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="32f62-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32f62-120">Request headers</span></span>
|<span data-ttu-id="32f62-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32f62-121">Header</span></span>|<span data-ttu-id="32f62-122">Valor</span><span class="sxs-lookup"><span data-stu-id="32f62-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32f62-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="32f62-123">Authorization</span></span>|<span data-ttu-id="32f62-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32f62-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32f62-125">Accept</span><span class="sxs-lookup"><span data-stu-id="32f62-125">Accept</span></span>|<span data-ttu-id="32f62-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32f62-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32f62-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32f62-127">Request body</span></span>
<span data-ttu-id="32f62-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32f62-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32f62-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f62-129">Response</span></span>
<span data-ttu-id="32f62-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32f62-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32f62-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32f62-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="32f62-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32f62-132">Request</span></span>
<span data-ttu-id="32f62-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32f62-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="32f62-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f62-134">Response</span></span>
<span data-ttu-id="32f62-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32f62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



