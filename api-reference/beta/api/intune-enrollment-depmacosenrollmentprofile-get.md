---
title: Obter depMacOSEnrollmentProfile
description: Leia as propriedades e os relacionamentos do objeto depMacOSEnrollmentProfile.
author: tfitzmac
ms.openlocfilehash: 7d1474e8291eb7d7859750c06bc76964bcdee7a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338406"
---
# <a name="get-depmacosenrollmentprofile"></a><span data-ttu-id="fff79-103">Obter depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="fff79-103">Get depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="fff79-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fff79-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fff79-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fff79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fff79-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fff79-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fff79-107">Leia as propriedades e os relacionamentos do objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="fff79-107">Read properties and relationships of the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fff79-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fff79-108">Prerequisites</span></span>
<span data-ttu-id="fff79-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fff79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fff79-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fff79-111">Permission type</span></span>|<span data-ttu-id="fff79-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fff79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fff79-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fff79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fff79-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fff79-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fff79-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fff79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fff79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fff79-116">Not supported.</span></span>|
|<span data-ttu-id="fff79-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fff79-117">Application</span></span>|<span data-ttu-id="fff79-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fff79-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fff79-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fff79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fff79-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fff79-120">Optional query parameters</span></span>
<span data-ttu-id="fff79-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fff79-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fff79-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fff79-122">Request headers</span></span>
|<span data-ttu-id="fff79-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fff79-123">Header</span></span>|<span data-ttu-id="fff79-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fff79-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fff79-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fff79-125">Authorization</span></span>|<span data-ttu-id="fff79-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fff79-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fff79-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fff79-127">Accept</span></span>|<span data-ttu-id="fff79-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fff79-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fff79-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fff79-129">Request body</span></span>
<span data-ttu-id="fff79-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fff79-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fff79-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fff79-131">Response</span></span>
<span data-ttu-id="fff79-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fff79-132">If successful, this method returns a `200 OK` response code and [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fff79-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fff79-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="fff79-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fff79-134">Request</span></span>
<span data-ttu-id="fff79-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fff79-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="fff79-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fff79-136">Response</span></span>
<span data-ttu-id="fff79-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fff79-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1048

{
  "value": {
    "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
    "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
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
    "profileRemovalDisabled": true,
    "restoreBlocked": true,
    "appleIdDisabled": true,
    "termsAndConditionsDisabled": true,
    "touchIdDisabled": true,
    "applePayDisabled": true,
    "zoomDisabled": true,
    "siriDisabled": true,
    "diagnosticsDisabled": true,
    "registrationDisabled": true,
    "fileVaultDisabled": true,
    "iCloudDiagnosticsDisabled": true
  }
}
```





