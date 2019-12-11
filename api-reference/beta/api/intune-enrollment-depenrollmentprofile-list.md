---
title: Listar depEnrollmentProfiles
description: Listar Propriedades e relações dos objetos depEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 617d7a839be475047534cc1a7d0574975b0e108a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944010"
---
# <a name="list-depenrollmentprofiles"></a><span data-ttu-id="9e17e-103">Listar depEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="9e17e-103">List depEnrollmentProfiles</span></span>

> <span data-ttu-id="9e17e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e17e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e17e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e17e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e17e-106">Listar Propriedades e relações dos objetos [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9e17e-106">List properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e17e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e17e-107">Prerequisites</span></span>
<span data-ttu-id="9e17e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e17e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e17e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e17e-110">Permission type</span></span>|<span data-ttu-id="9e17e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9e17e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e17e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e17e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e17e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e17e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9e17e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e17e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e17e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e17e-115">Not supported.</span></span>|
|<span data-ttu-id="9e17e-116">Application</span><span class="sxs-lookup"><span data-stu-id="9e17e-116">Application</span></span>|<span data-ttu-id="9e17e-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e17e-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e17e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e17e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="9e17e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e17e-119">Request headers</span></span>
|<span data-ttu-id="9e17e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e17e-120">Header</span></span>|<span data-ttu-id="9e17e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9e17e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e17e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e17e-122">Authorization</span></span>|<span data-ttu-id="9e17e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e17e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e17e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e17e-124">Accept</span></span>|<span data-ttu-id="9e17e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e17e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e17e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e17e-126">Request body</span></span>
<span data-ttu-id="9e17e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e17e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e17e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e17e-128">Response</span></span>
<span data-ttu-id="9e17e-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e17e-129">If successful, this method returns a `200 OK` response code and a collection of [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e17e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e17e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e17e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e17e-131">Request</span></span>
<span data-ttu-id="9e17e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e17e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="9e17e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e17e-133">Response</span></span>
<span data-ttu-id="9e17e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e17e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1588

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depEnrollmentProfile",
      "id": "3d4534f7-34f7-3d45-f734-453df734453d",
      "displayName": "Display Name value",
      "description": "Description value",
      "requiresUserAuthentication": true,
      "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
      "enableAuthenticationViaCompanyPortal": true,
      "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
      "isDefault": true,
      "supervisedModeEnabled": true,
      "supportDepartment": "Support Department value",
      "passCodeDisabled": true,
      "isMandatory": true,
      "locationDisabled": true,
      "supportPhoneNumber": "Support Phone Number value",
      "iTunesPairingMode": "allow",
      "profileRemovalDisabled": true,
      "managementCertificates": [
        {
          "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
          "thumbprint": "Thumbprint value",
          "certificate": "Certificate value"
        }
      ],
      "restoreBlocked": true,
      "restoreFromAndroidDisabled": true,
      "appleIdDisabled": true,
      "termsAndConditionsDisabled": true,
      "touchIdDisabled": true,
      "applePayDisabled": true,
      "zoomDisabled": true,
      "siriDisabled": true,
      "diagnosticsDisabled": true,
      "macOSRegistrationDisabled": true,
      "macOSFileVaultDisabled": true,
      "awaitDeviceConfiguredConfirmation": true,
      "sharedIPadMaximumUserCount": 10,
      "enableSharedIPad": true
    }
  ]
}
```





