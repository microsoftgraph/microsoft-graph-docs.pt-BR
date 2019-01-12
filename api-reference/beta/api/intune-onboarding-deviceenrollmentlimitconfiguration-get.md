---
title: Acessar deviceEnrollmentLimitConfiguration
description: Leia as propriedades e as relações do objeto deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 56ffdbf3e26ad2b33a68de98a105d9bc4f7a6252
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915360"
---
# <a name="get-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="e1326-103">Acessar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1326-103">Get deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="e1326-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e1326-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1326-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e1326-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1326-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e1326-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1326-107">Leia as propriedades e as relações do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e1326-107">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1326-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1326-108">Prerequisites</span></span>
<span data-ttu-id="e1326-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1326-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1326-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1326-111">Permission type</span></span>|<span data-ttu-id="e1326-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1326-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1326-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1326-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1326-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1326-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e1326-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1326-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1326-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1326-116">Not supported.</span></span>|
|<span data-ttu-id="e1326-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1326-117">Application</span></span>|<span data-ttu-id="e1326-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1326-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1326-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1326-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1326-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e1326-120">Optional query parameters</span></span>
<span data-ttu-id="e1326-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e1326-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e1326-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1326-122">Request headers</span></span>
|<span data-ttu-id="e1326-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1326-123">Header</span></span>|<span data-ttu-id="e1326-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e1326-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1326-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1326-125">Authorization</span></span>|<span data-ttu-id="e1326-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1326-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1326-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1326-127">Accept</span></span>|<span data-ttu-id="e1326-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e1326-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1326-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1326-129">Request body</span></span>
<span data-ttu-id="e1326-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1326-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1326-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1326-131">Response</span></span>
<span data-ttu-id="e1326-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1326-132">If successful, this method returns a `200 OK` response code and [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1326-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1326-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1326-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1326-134">Request</span></span>
<span data-ttu-id="e1326-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1326-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e1326-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1326-136">Response</span></span>
<span data-ttu-id="e1326-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1326-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 414

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
    "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7,
    "limit": 5
  }
}
```





