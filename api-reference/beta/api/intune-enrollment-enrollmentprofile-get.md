---
title: Obter enrollmentProfile
description: Leia as propriedades e os relacionamentos do objeto enrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ad47c819c5c05441f6f92c09e8112a4a5152e85d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419699"
---
# <a name="get-enrollmentprofile"></a><span data-ttu-id="a7ae1-103">Obter enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a7ae1-103">Get enrollmentProfile</span></span>

> <span data-ttu-id="a7ae1-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a7ae1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a7ae1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a7ae1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7ae1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a7ae1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7ae1-107">Leia as propriedades e os relacionamentos do objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a7ae1-107">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7ae1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a7ae1-108">Prerequisites</span></span>
<span data-ttu-id="a7ae1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a7ae1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a7ae1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7ae1-111">Permission type</span></span>|<span data-ttu-id="a7ae1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a7ae1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7ae1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7ae1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7ae1-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7ae1-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a7ae1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7ae1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7ae1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7ae1-116">Not supported.</span></span>|
|<span data-ttu-id="a7ae1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7ae1-117">Application</span></span>|<span data-ttu-id="a7ae1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7ae1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7ae1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7ae1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7ae1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a7ae1-120">Optional query parameters</span></span>
<span data-ttu-id="a7ae1-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a7ae1-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7ae1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7ae1-122">Request headers</span></span>
|<span data-ttu-id="a7ae1-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7ae1-123">Header</span></span>|<span data-ttu-id="a7ae1-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a7ae1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7ae1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7ae1-125">Authorization</span></span>|<span data-ttu-id="a7ae1-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7ae1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7ae1-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a7ae1-127">Accept</span></span>|<span data-ttu-id="a7ae1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a7ae1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7ae1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7ae1-129">Request body</span></span>
<span data-ttu-id="a7ae1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7ae1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7ae1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7ae1-131">Response</span></span>
<span data-ttu-id="a7ae1-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7ae1-132">If successful, this method returns a `200 OK` response code and [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7ae1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7ae1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7ae1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7ae1-134">Request</span></span>
<span data-ttu-id="a7ae1-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7ae1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="a7ae1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7ae1-136">Response</span></span>
<span data-ttu-id="a7ae1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7ae1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 454

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentProfile",
    "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
    "displayName": "Display Name value",
    "description": "Description value",
    "requiresUserAuthentication": true,
    "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
    "enableAuthenticationViaCompanyPortal": true,
    "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
  }
}
```




