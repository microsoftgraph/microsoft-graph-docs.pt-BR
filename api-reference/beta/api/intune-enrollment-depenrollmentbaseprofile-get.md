---
title: Obter depEnrollmentBaseProfile
description: Leia as propriedades e os relacionamentos do objeto depEnrollmentBaseProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 00833f87bb2fb6d39dc4f1bd194aee540d959067
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881092"
---
# <a name="get-depenrollmentbaseprofile"></a><span data-ttu-id="f220d-103">Obter depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="f220d-103">Get depEnrollmentBaseProfile</span></span>

> <span data-ttu-id="f220d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f220d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f220d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f220d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f220d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f220d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f220d-107">Leia as propriedades e os relacionamentos do objeto [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f220d-107">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f220d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f220d-108">Prerequisites</span></span>
<span data-ttu-id="f220d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f220d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f220d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f220d-111">Permission type</span></span>|<span data-ttu-id="f220d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f220d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f220d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f220d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f220d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f220d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f220d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f220d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f220d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f220d-116">Not supported.</span></span>|
|<span data-ttu-id="f220d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f220d-117">Application</span></span>|<span data-ttu-id="f220d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f220d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f220d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f220d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f220d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f220d-120">Optional query parameters</span></span>
<span data-ttu-id="f220d-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f220d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f220d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f220d-122">Request headers</span></span>
|<span data-ttu-id="f220d-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f220d-123">Header</span></span>|<span data-ttu-id="f220d-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f220d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f220d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f220d-125">Authorization</span></span>|<span data-ttu-id="f220d-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f220d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f220d-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f220d-127">Accept</span></span>|<span data-ttu-id="f220d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f220d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f220d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f220d-129">Request body</span></span>
<span data-ttu-id="f220d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f220d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f220d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f220d-131">Response</span></span>
<span data-ttu-id="f220d-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f220d-132">If successful, this method returns a `200 OK` response code and [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f220d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f220d-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="f220d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f220d-134">Request</span></span>
<span data-ttu-id="f220d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f220d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="f220d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f220d-136">Response</span></span>
<span data-ttu-id="f220d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f220d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 940

{
  "value": {
    "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
    "id": "db378868-8868-db37-6888-37db688837db",
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
    "diagnosticsDisabled": true
  }
}
```





