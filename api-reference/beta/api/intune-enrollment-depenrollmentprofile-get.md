---
title: Obter depEnrollmentProfile
description: Leia as propriedades e os relacionamentos do objeto depEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aa3c9da25c4afa0b8ba4130f6cc7afb869aa33f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878964"
---
# <a name="get-depenrollmentprofile"></a><span data-ttu-id="800ab-103">Obter depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="800ab-103">Get depEnrollmentProfile</span></span>

> <span data-ttu-id="800ab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="800ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="800ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="800ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="800ab-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="800ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="800ab-107">Leia as propriedades e os relacionamentos do objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="800ab-107">Read properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="800ab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="800ab-108">Prerequisites</span></span>
<span data-ttu-id="800ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="800ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="800ab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="800ab-111">Permission type</span></span>|<span data-ttu-id="800ab-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="800ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="800ab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="800ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="800ab-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="800ab-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="800ab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="800ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="800ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="800ab-116">Not supported.</span></span>|
|<span data-ttu-id="800ab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="800ab-117">Application</span></span>|<span data-ttu-id="800ab-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="800ab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="800ab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="800ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="800ab-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="800ab-120">Optional query parameters</span></span>
<span data-ttu-id="800ab-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="800ab-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="800ab-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="800ab-122">Request headers</span></span>
|<span data-ttu-id="800ab-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="800ab-123">Header</span></span>|<span data-ttu-id="800ab-124">Valor</span><span class="sxs-lookup"><span data-stu-id="800ab-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="800ab-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="800ab-125">Authorization</span></span>|<span data-ttu-id="800ab-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="800ab-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="800ab-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="800ab-127">Accept</span></span>|<span data-ttu-id="800ab-128">application/json</span><span class="sxs-lookup"><span data-stu-id="800ab-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="800ab-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="800ab-129">Request body</span></span>
<span data-ttu-id="800ab-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="800ab-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="800ab-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="800ab-131">Response</span></span>
<span data-ttu-id="800ab-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="800ab-132">If successful, this method returns a `200 OK` response code and [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="800ab-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="800ab-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="800ab-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="800ab-134">Request</span></span>
<span data-ttu-id="800ab-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="800ab-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="800ab-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="800ab-136">Response</span></span>
<span data-ttu-id="800ab-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="800ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1432

{
  "value": {
    "@odata.type": "#microsoft.graph.depEnrollmentProfile",
    "id": "3d4534f7-34f7-3d45-f734-453df734453d",
    "displayName": "Display Name value",
    "description": "Description value",
    "requiresUserAuthentication": true,
    "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
    "enableAuthenticationViaCompanyPortal": true,
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





