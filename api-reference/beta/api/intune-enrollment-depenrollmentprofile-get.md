---
title: Obter depEnrollmentProfile
description: Leia as propriedades e as relações do objeto depEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26aa8f8458c2e9910e0b54fcc588534496e11e87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467267"
---
# <a name="get-depenrollmentprofile"></a><span data-ttu-id="e0651-103">Obter depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e0651-103">Get depEnrollmentProfile</span></span>

<span data-ttu-id="e0651-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e0651-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0651-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0651-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0651-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0651-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0651-107">Leia as propriedades e as relações do objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e0651-107">Read properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0651-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e0651-108">Prerequisites</span></span>
<span data-ttu-id="e0651-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0651-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0651-111">Permission type</span></span>|<span data-ttu-id="e0651-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e0651-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0651-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0651-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0651-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0651-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e0651-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0651-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0651-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0651-116">Not supported.</span></span>|
|<span data-ttu-id="e0651-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0651-117">Application</span></span>|<span data-ttu-id="e0651-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0651-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0651-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0651-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0651-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0651-120">Optional query parameters</span></span>
<span data-ttu-id="e0651-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0651-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0651-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0651-122">Request headers</span></span>
|<span data-ttu-id="e0651-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0651-123">Header</span></span>|<span data-ttu-id="e0651-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e0651-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0651-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0651-125">Authorization</span></span>|<span data-ttu-id="e0651-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0651-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0651-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0651-127">Accept</span></span>|<span data-ttu-id="e0651-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e0651-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0651-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0651-129">Request body</span></span>
<span data-ttu-id="e0651-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0651-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0651-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0651-131">Response</span></span>
<span data-ttu-id="e0651-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0651-132">If successful, this method returns a `200 OK` response code and [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0651-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0651-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0651-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0651-134">Request</span></span>
<span data-ttu-id="e0651-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0651-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="e0651-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0651-136">Response</span></span>
<span data-ttu-id="e0651-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0651-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1498

{
  "value": {
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
}
```





