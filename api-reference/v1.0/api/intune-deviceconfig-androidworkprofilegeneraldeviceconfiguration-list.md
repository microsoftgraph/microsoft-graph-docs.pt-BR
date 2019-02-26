---
title: Listar androidWorkProfileGeneralDeviceConfigurations
description: Listar Propriedades e relações dos objetos Entidadeandroidforworkprofiledeviceconfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f821208383f6dece05433f8541e5be2fcfc3acd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250779"
---
# <a name="list-androidworkprofilegeneraldeviceconfigurations"></a><span data-ttu-id="0a00d-103">Listar androidWorkProfileGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="0a00d-103">List androidWorkProfileGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="0a00d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a00d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a00d-105">Listar Propriedades e relações dos objetos [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0a00d-105">List properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a00d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a00d-106">Prerequisites</span></span>
<span data-ttu-id="0a00d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0a00d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0a00d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a00d-109">Permission type</span></span>|<span data-ttu-id="0a00d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a00d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a00d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a00d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0a00d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a00d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0a00d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a00d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a00d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a00d-114">Not supported.</span></span>|
|<span data-ttu-id="0a00d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a00d-115">Application</span></span>|<span data-ttu-id="0a00d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a00d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a00d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a00d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0a00d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a00d-118">Request headers</span></span>
|<span data-ttu-id="0a00d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a00d-119">Header</span></span>|<span data-ttu-id="0a00d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0a00d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a00d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a00d-121">Authorization</span></span>|<span data-ttu-id="0a00d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a00d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a00d-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0a00d-123">Accept</span></span>|<span data-ttu-id="0a00d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0a00d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a00d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a00d-125">Request body</span></span>
<span data-ttu-id="0a00d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a00d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a00d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a00d-127">Response</span></span>
<span data-ttu-id="0a00d-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a00d-128">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a00d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a00d-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a00d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a00d-130">Request</span></span>
<span data-ttu-id="0a00d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a00d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0a00d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a00d-132">Response</span></span>
<span data-ttu-id="0a00d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a00d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



