---
title: Obter importedAppleDeviceIdentity
description: Leia as propriedades e os relacionamentos do objeto importedAppleDeviceIdentity.
author: tfitzmac
ms.openlocfilehash: fc4a68086620e8c152703af8da1d604e3a4da7f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310189"
---
# <a name="get-importedappledeviceidentity"></a><span data-ttu-id="451c3-103">Obter importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="451c3-103">Get importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="451c3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="451c3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="451c3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="451c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="451c3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="451c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="451c3-107">Leia as propriedades e os relacionamentos do objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="451c3-107">Read properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="451c3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="451c3-108">Prerequisites</span></span>
<span data-ttu-id="451c3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="451c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="451c3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="451c3-111">Permission type</span></span>|<span data-ttu-id="451c3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="451c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="451c3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="451c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="451c3-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="451c3-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="451c3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="451c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="451c3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="451c3-116">Not supported.</span></span>|
|<span data-ttu-id="451c3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="451c3-117">Application</span></span>|<span data-ttu-id="451c3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="451c3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="451c3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="451c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="451c3-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="451c3-120">Optional query parameters</span></span>
<span data-ttu-id="451c3-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="451c3-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="451c3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="451c3-122">Request headers</span></span>
|<span data-ttu-id="451c3-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="451c3-123">Header</span></span>|<span data-ttu-id="451c3-124">Valor</span><span class="sxs-lookup"><span data-stu-id="451c3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="451c3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="451c3-125">Authorization</span></span>|<span data-ttu-id="451c3-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="451c3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="451c3-127">Accept</span><span class="sxs-lookup"><span data-stu-id="451c3-127">Accept</span></span>|<span data-ttu-id="451c3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="451c3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="451c3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="451c3-129">Request body</span></span>
<span data-ttu-id="451c3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="451c3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="451c3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="451c3-131">Response</span></span>
<span data-ttu-id="451c3-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="451c3-132">If successful, this method returns a `200 OK` response code and [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="451c3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="451c3-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="451c3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="451c3-134">Request</span></span>
<span data-ttu-id="451c3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="451c3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="451c3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="451c3-136">Response</span></span>
<span data-ttu-id="451c3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="451c3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 648

{
  "value": {
    "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
    "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
    "serialNumber": "Serial Number value",
    "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
    "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
    "isSupervised": true,
    "discoverySource": "adminImport",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
    "description": "Description value",
    "enrollmentState": "enrolled",
    "platform": "ios"
  }
}
```





