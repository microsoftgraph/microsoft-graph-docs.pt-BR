---
title: Listar windows10EnrollmentCompletionPageConfigurations
description: Listar Propriedades e relações dos objetos windows10EnrollmentCompletionPageConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d9ed61c27fabdfd7b1b975bc6c34fc6a599d784
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455790"
---
# <a name="list-windows10enrollmentcompletionpageconfigurations"></a><span data-ttu-id="5ac94-103">Listar windows10EnrollmentCompletionPageConfigurations</span><span class="sxs-lookup"><span data-stu-id="5ac94-103">List windows10EnrollmentCompletionPageConfigurations</span></span>

<span data-ttu-id="5ac94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ac94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ac94-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ac94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ac94-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ac94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ac94-107">Listar Propriedades e relações dos objetos [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5ac94-107">List properties and relationships of the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ac94-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ac94-108">Prerequisites</span></span>
<span data-ttu-id="5ac94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ac94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ac94-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ac94-111">Permission type</span></span>|<span data-ttu-id="5ac94-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ac94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ac94-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ac94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ac94-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ac94-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5ac94-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ac94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ac94-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ac94-116">Not supported.</span></span>|
|<span data-ttu-id="5ac94-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ac94-117">Application</span></span>|<span data-ttu-id="5ac94-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ac94-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ac94-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ac94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5ac94-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ac94-120">Request headers</span></span>
|<span data-ttu-id="5ac94-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ac94-121">Header</span></span>|<span data-ttu-id="5ac94-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5ac94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ac94-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ac94-123">Authorization</span></span>|<span data-ttu-id="5ac94-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ac94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ac94-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ac94-125">Accept</span></span>|<span data-ttu-id="5ac94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ac94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ac94-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ac94-127">Request body</span></span>
<span data-ttu-id="5ac94-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ac94-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ac94-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ac94-129">Response</span></span>
<span data-ttu-id="5ac94-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ac94-130">If successful, this method returns a `200 OK` response code and a collection of [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ac94-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ac94-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ac94-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ac94-132">Request</span></span>
<span data-ttu-id="5ac94-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ac94-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="5ac94-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ac94-134">Response</span></span>
<span data-ttu-id="5ac94-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ac94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 969

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
      "id": "77bf8248-8248-77bf-4882-bf774882bf77",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "showInstallationProgress": true,
      "blockDeviceSetupRetryByUser": true,
      "allowDeviceResetOnInstallFailure": true,
      "allowLogCollectionOnInstallFailure": true,
      "customErrorMessage": "Custom Error Message value",
      "installProgressTimeoutInMinutes": 15,
      "allowDeviceUseOnInstallFailure": true,
      "selectedMobileAppIds": [
        "Selected Mobile App Ids value"
      ],
      "trackInstallProgressForAutopilotOnly": true,
      "disableUserStatusTrackingAfterFirstUser": true
    }
  ]
}
```



