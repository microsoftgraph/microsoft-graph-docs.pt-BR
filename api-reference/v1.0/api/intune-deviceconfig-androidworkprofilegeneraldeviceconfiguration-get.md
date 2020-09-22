---
title: Obter Entidadeandroidforworkprofiledeviceconfiguration
description: Leia as propriedades e as relações do objeto Entidadeandroidforworkprofiledeviceconfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a727ada677fd136405ced79ae56a46dcf150ab9e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083635"
---
# <a name="get-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="a3672-103">Obter Entidadeandroidforworkprofiledeviceconfiguration</span><span class="sxs-lookup"><span data-stu-id="a3672-103">Get androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="a3672-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3672-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3672-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a3672-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3672-106">Leia as propriedades e as relações do objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a3672-106">Read properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3672-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a3672-107">Prerequisites</span></span>
<span data-ttu-id="a3672-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3672-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3672-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3672-110">Permission type</span></span>|<span data-ttu-id="a3672-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a3672-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3672-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3672-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3672-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3672-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a3672-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3672-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3672-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3672-115">Not supported.</span></span>|
|<span data-ttu-id="a3672-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3672-116">Application</span></span>|<span data-ttu-id="a3672-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3672-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3672-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3672-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3672-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a3672-119">Optional query parameters</span></span>
<span data-ttu-id="a3672-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a3672-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3672-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3672-121">Request headers</span></span>
|<span data-ttu-id="a3672-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3672-122">Header</span></span>|<span data-ttu-id="a3672-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a3672-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3672-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3672-124">Authorization</span></span>|<span data-ttu-id="a3672-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3672-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3672-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a3672-126">Accept</span></span>|<span data-ttu-id="a3672-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a3672-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3672-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3672-128">Request body</span></span>
<span data-ttu-id="a3672-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3672-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3672-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3672-130">Response</span></span>
<span data-ttu-id="a3672-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3672-131">If successful, this method returns a `200 OK` response code and [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3672-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3672-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3672-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3672-133">Request</span></span>
<span data-ttu-id="a3672-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3672-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a3672-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3672-135">Response</span></span>
<span data-ttu-id="a3672-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3672-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









