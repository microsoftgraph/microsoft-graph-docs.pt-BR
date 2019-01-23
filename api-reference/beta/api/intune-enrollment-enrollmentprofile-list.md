---
title: Lista enrollmentProfiles
description: Lista as propriedades e os relacionamentos dos objetos enrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: accbfdde2baa03d104fdbde523233e957d82ac81
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419979"
---
# <a name="list-enrollmentprofiles"></a><span data-ttu-id="38231-103">Lista enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="38231-103">List enrollmentProfiles</span></span>

> <span data-ttu-id="38231-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="38231-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="38231-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="38231-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38231-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="38231-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38231-107">Lista as propriedades e os relacionamentos dos objetos [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="38231-107">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38231-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38231-108">Prerequisites</span></span>
<span data-ttu-id="38231-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="38231-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="38231-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38231-111">Permission type</span></span>|<span data-ttu-id="38231-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38231-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38231-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38231-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38231-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="38231-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="38231-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38231-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38231-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38231-116">Not supported.</span></span>|
|<span data-ttu-id="38231-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38231-117">Application</span></span>|<span data-ttu-id="38231-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38231-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38231-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38231-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="38231-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38231-120">Request headers</span></span>
|<span data-ttu-id="38231-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38231-121">Header</span></span>|<span data-ttu-id="38231-122">Valor</span><span class="sxs-lookup"><span data-stu-id="38231-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38231-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="38231-123">Authorization</span></span>|<span data-ttu-id="38231-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38231-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38231-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38231-125">Accept</span></span>|<span data-ttu-id="38231-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38231-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38231-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38231-127">Request body</span></span>
<span data-ttu-id="38231-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38231-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38231-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="38231-129">Response</span></span>
<span data-ttu-id="38231-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38231-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38231-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38231-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="38231-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38231-132">Request</span></span>
<span data-ttu-id="38231-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38231-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="38231-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="38231-134">Response</span></span>
<span data-ttu-id="38231-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38231-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentProfile",
      "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
      "displayName": "Display Name value",
      "description": "Description value",
      "requiresUserAuthentication": true,
      "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
      "enableAuthenticationViaCompanyPortal": true,
      "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
    }
  ]
}
```




