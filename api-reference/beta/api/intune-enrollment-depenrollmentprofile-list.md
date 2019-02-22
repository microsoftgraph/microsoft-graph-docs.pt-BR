---
title: Listar depEnrollmentProfiles
description: Listar Propriedades e relações dos objetos depEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c56249a0baed864eb9e3f13b3646c08a57617c1a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174965"
---
# <a name="list-depenrollmentprofiles"></a><span data-ttu-id="9b523-103">Listar depEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="9b523-103">List depEnrollmentProfiles</span></span>

> <span data-ttu-id="9b523-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b523-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b523-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b523-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b523-106">Listar Propriedades e relações dos objetos [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9b523-106">List properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b523-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9b523-107">Prerequisites</span></span>
<span data-ttu-id="9b523-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9b523-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9b523-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b523-110">Permission type</span></span>|<span data-ttu-id="9b523-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9b523-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b523-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b523-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b523-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b523-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9b523-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b523-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b523-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b523-115">Not supported.</span></span>|
|<span data-ttu-id="9b523-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b523-116">Application</span></span>|<span data-ttu-id="9b523-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b523-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b523-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b523-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="9b523-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b523-119">Request headers</span></span>
|<span data-ttu-id="9b523-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b523-120">Header</span></span>|<span data-ttu-id="9b523-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9b523-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b523-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b523-122">Authorization</span></span>|<span data-ttu-id="9b523-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b523-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b523-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9b523-124">Accept</span></span>|<span data-ttu-id="9b523-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b523-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b523-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b523-126">Request body</span></span>
<span data-ttu-id="9b523-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b523-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b523-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b523-128">Response</span></span>
<span data-ttu-id="9b523-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b523-129">If successful, this method returns a `200 OK` response code and a collection of [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b523-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b523-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b523-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b523-131">Request</span></span>
<span data-ttu-id="9b523-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b523-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="9b523-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b523-133">Response</span></span>
<span data-ttu-id="9b523-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b523-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




