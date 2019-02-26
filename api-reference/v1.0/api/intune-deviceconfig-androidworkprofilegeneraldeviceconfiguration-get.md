---
title: Obter Entidadeandroidforworkprofiledeviceconfiguration
description: Leia as propriedades e as relações do objeto Entidadeandroidforworkprofiledeviceconfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: be25825bf83a28254283e0e465ba3aaf8383413c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251773"
---
# <a name="get-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="87179-103">Obter Entidadeandroidforworkprofiledeviceconfiguration</span><span class="sxs-lookup"><span data-stu-id="87179-103">Get androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="87179-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87179-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87179-105">Leia as propriedades e as relações do objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="87179-105">Read properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87179-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87179-106">Prerequisites</span></span>
<span data-ttu-id="87179-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="87179-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="87179-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87179-109">Permission type</span></span>|<span data-ttu-id="87179-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87179-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87179-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87179-111">Delegated (work or school account)</span></span>|<span data-ttu-id="87179-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87179-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87179-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87179-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87179-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87179-114">Not supported.</span></span>|
|<span data-ttu-id="87179-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87179-115">Application</span></span>|<span data-ttu-id="87179-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87179-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87179-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87179-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87179-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87179-118">Optional query parameters</span></span>
<span data-ttu-id="87179-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87179-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87179-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87179-120">Request headers</span></span>
|<span data-ttu-id="87179-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87179-121">Header</span></span>|<span data-ttu-id="87179-122">Valor</span><span class="sxs-lookup"><span data-stu-id="87179-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87179-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="87179-123">Authorization</span></span>|<span data-ttu-id="87179-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87179-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87179-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87179-125">Accept</span></span>|<span data-ttu-id="87179-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87179-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87179-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87179-127">Request body</span></span>
<span data-ttu-id="87179-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87179-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87179-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="87179-129">Response</span></span>
<span data-ttu-id="87179-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87179-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87179-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87179-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="87179-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87179-132">Request</span></span>
<span data-ttu-id="87179-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87179-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="87179-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="87179-134">Response</span></span>
<span data-ttu-id="87179-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87179-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



