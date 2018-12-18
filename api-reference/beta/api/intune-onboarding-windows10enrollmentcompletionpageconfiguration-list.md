---
title: Lista windows10EnrollmentCompletionPageConfigurations
description: Lista as propriedades e os relacionamentos dos objetos windows10EnrollmentCompletionPageConfiguration.
author: tfitzmac
ms.openlocfilehash: 0a58303efbf97e8f447d0fdd0345d46d559b3c77
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338721"
---
# <a name="list-windows10enrollmentcompletionpageconfigurations"></a><span data-ttu-id="da3e8-103">Lista windows10EnrollmentCompletionPageConfigurations</span><span class="sxs-lookup"><span data-stu-id="da3e8-103">List windows10EnrollmentCompletionPageConfigurations</span></span>

> <span data-ttu-id="da3e8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="da3e8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da3e8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da3e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da3e8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="da3e8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da3e8-107">Lista as propriedades e os relacionamentos dos objetos [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="da3e8-107">List properties and relationships of the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da3e8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da3e8-108">Prerequisites</span></span>
<span data-ttu-id="da3e8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da3e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da3e8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da3e8-111">Permission type</span></span>|<span data-ttu-id="da3e8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da3e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da3e8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da3e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da3e8-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="da3e8-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="da3e8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da3e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da3e8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da3e8-116">Not supported.</span></span>|
|<span data-ttu-id="da3e8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da3e8-117">Application</span></span>|<span data-ttu-id="da3e8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da3e8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da3e8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da3e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="da3e8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da3e8-120">Request headers</span></span>
|<span data-ttu-id="da3e8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da3e8-121">Header</span></span>|<span data-ttu-id="da3e8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="da3e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da3e8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="da3e8-123">Authorization</span></span>|<span data-ttu-id="da3e8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da3e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da3e8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="da3e8-125">Accept</span></span>|<span data-ttu-id="da3e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da3e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da3e8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da3e8-127">Request body</span></span>
<span data-ttu-id="da3e8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da3e8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da3e8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="da3e8-129">Response</span></span>
<span data-ttu-id="da3e8-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da3e8-130">If successful, this method returns a `200 OK` response code and a collection of [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da3e8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da3e8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="da3e8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da3e8-132">Request</span></span>
<span data-ttu-id="da3e8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da3e8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="da3e8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="da3e8-134">Response</span></span>
<span data-ttu-id="da3e8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da3e8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





