---
title: Listar androidWorkProfileGeneralDeviceConfigurations
description: Listar Propriedades e relações dos objetos Entidadeandroidforworkprofiledeviceconfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 85ff1c43dda37da74428d39b184acf1a41428134
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401041"
---
# <a name="list-androidworkprofilegeneraldeviceconfigurations"></a><span data-ttu-id="a1298-103">Listar androidWorkProfileGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="a1298-103">List androidWorkProfileGeneralDeviceConfigurations</span></span>

<span data-ttu-id="a1298-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1298-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1298-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1298-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1298-106">Listar Propriedades e relações dos objetos [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a1298-106">List properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1298-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1298-107">Prerequisites</span></span>
<span data-ttu-id="a1298-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1298-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1298-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1298-110">Permission type</span></span>|<span data-ttu-id="a1298-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1298-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1298-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1298-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1298-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1298-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a1298-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1298-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1298-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1298-115">Not supported.</span></span>|
|<span data-ttu-id="a1298-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1298-116">Application</span></span>|<span data-ttu-id="a1298-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1298-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1298-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1298-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a1298-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1298-119">Request headers</span></span>
|<span data-ttu-id="a1298-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1298-120">Header</span></span>|<span data-ttu-id="a1298-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a1298-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1298-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1298-122">Authorization</span></span>|<span data-ttu-id="a1298-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1298-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1298-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1298-124">Accept</span></span>|<span data-ttu-id="a1298-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1298-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1298-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1298-126">Request body</span></span>
<span data-ttu-id="a1298-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1298-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1298-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1298-128">Response</span></span>
<span data-ttu-id="a1298-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1298-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1298-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1298-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1298-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1298-131">Request</span></span>
<span data-ttu-id="a1298-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1298-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a1298-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1298-133">Response</span></span>
<span data-ttu-id="a1298-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1298-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2200

{
  "value": [
    {
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
  ]
}
```






