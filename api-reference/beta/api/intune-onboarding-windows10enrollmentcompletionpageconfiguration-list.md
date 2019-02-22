---
title: Listar windows10EnrollmentCompletionPageConfigurations
description: Listar Propriedades e relações dos objetos windows10EnrollmentCompletionPageConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef07ce0c3f37d2ac27c74557d10e2a697adac644
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154751"
---
# <a name="list-windows10enrollmentcompletionpageconfigurations"></a><span data-ttu-id="a38ca-103">Listar windows10EnrollmentCompletionPageConfigurations</span><span class="sxs-lookup"><span data-stu-id="a38ca-103">List windows10EnrollmentCompletionPageConfigurations</span></span>

> <span data-ttu-id="a38ca-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a38ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a38ca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a38ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a38ca-106">Listar Propriedades e relações dos objetos [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a38ca-106">List properties and relationships of the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a38ca-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a38ca-107">Prerequisites</span></span>
<span data-ttu-id="a38ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a38ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a38ca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a38ca-110">Permission type</span></span>|<span data-ttu-id="a38ca-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a38ca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a38ca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a38ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a38ca-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a38ca-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a38ca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a38ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a38ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a38ca-115">Not supported.</span></span>|
|<span data-ttu-id="a38ca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a38ca-116">Application</span></span>|<span data-ttu-id="a38ca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a38ca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a38ca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a38ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a38ca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a38ca-119">Request headers</span></span>
|<span data-ttu-id="a38ca-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a38ca-120">Header</span></span>|<span data-ttu-id="a38ca-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a38ca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a38ca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a38ca-122">Authorization</span></span>|<span data-ttu-id="a38ca-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a38ca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a38ca-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a38ca-124">Accept</span></span>|<span data-ttu-id="a38ca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a38ca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a38ca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a38ca-126">Request body</span></span>
<span data-ttu-id="a38ca-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a38ca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a38ca-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a38ca-128">Response</span></span>
<span data-ttu-id="a38ca-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a38ca-129">If successful, this method returns a `200 OK` response code and a collection of [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a38ca-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a38ca-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a38ca-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a38ca-131">Request</span></span>
<span data-ttu-id="a38ca-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a38ca-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="a38ca-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a38ca-133">Response</span></span>
<span data-ttu-id="a38ca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a38ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 860

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
      ]
    }
  ]
}
```




