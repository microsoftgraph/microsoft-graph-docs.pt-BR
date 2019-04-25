---
title: Obter depEnrollmentBaseProfile
description: Leia as propriedades e as relações do objeto depEnrollmentBaseProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcfc07c48ed9d780bb80c16057dd4d57627b15df
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534042"
---
# <a name="get-depenrollmentbaseprofile"></a><span data-ttu-id="54a33-103">Obter depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="54a33-103">Get depEnrollmentBaseProfile</span></span>

> <span data-ttu-id="54a33-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54a33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54a33-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54a33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54a33-106">Leia as propriedades e as relações do objeto [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="54a33-106">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54a33-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54a33-107">Prerequisites</span></span>
<span data-ttu-id="54a33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54a33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54a33-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54a33-110">Permission type</span></span>|<span data-ttu-id="54a33-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54a33-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54a33-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54a33-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54a33-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="54a33-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="54a33-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54a33-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54a33-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54a33-115">Not supported.</span></span>|
|<span data-ttu-id="54a33-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54a33-116">Application</span></span>|<span data-ttu-id="54a33-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54a33-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54a33-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54a33-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54a33-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="54a33-119">Optional query parameters</span></span>
<span data-ttu-id="54a33-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="54a33-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54a33-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54a33-121">Request headers</span></span>
|<span data-ttu-id="54a33-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54a33-122">Header</span></span>|<span data-ttu-id="54a33-123">Valor</span><span class="sxs-lookup"><span data-stu-id="54a33-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54a33-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="54a33-124">Authorization</span></span>|<span data-ttu-id="54a33-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54a33-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54a33-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54a33-126">Accept</span></span>|<span data-ttu-id="54a33-127">application/json</span><span class="sxs-lookup"><span data-stu-id="54a33-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54a33-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54a33-128">Request body</span></span>
<span data-ttu-id="54a33-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54a33-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54a33-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="54a33-130">Response</span></span>
<span data-ttu-id="54a33-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54a33-131">If successful, this method returns a `200 OK` response code and [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54a33-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54a33-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="54a33-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54a33-133">Request</span></span>
<span data-ttu-id="54a33-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54a33-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="54a33-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="54a33-135">Response</span></span>
<span data-ttu-id="54a33-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54a33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1136

{
  "value": {
    "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
    "id": "db378868-8868-db37-6888-37db688837db",
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
    "profileRemovalDisabled": true,
    "restoreBlocked": true,
    "appleIdDisabled": true,
    "termsAndConditionsDisabled": true,
    "touchIdDisabled": true,
    "applePayDisabled": true,
    "zoomDisabled": true,
    "siriDisabled": true,
    "diagnosticsDisabled": true,
    "displayToneSetupDisabled": true,
    "privacyPaneDisabled": true,
    "deviceNameTemplate": "Device Name Template value"
  }
}
```





