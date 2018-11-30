---
title: Obter deviceEnrollmentConfiguration
description: Ler propriedades e relações do objeto deviceEnrollmentConfiguration.
ms.openlocfilehash: 833dcacc91aee8d5f61c44be281f9168287b68e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007016"
---
# <a name="get-deviceenrollmentconfiguration"></a><span data-ttu-id="fec10-103">Obter deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="fec10-103">Get deviceEnrollmentConfiguration</span></span>

> <span data-ttu-id="fec10-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fec10-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fec10-105">Ler propriedades e relações do objeto [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fec10-105">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fec10-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fec10-106">Prerequisites</span></span>
<span data-ttu-id="fec10-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fec10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fec10-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fec10-109">Permission type</span></span>|<span data-ttu-id="fec10-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fec10-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fec10-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fec10-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fec10-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fec10-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fec10-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fec10-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fec10-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fec10-114">Not supported.</span></span>|
|<span data-ttu-id="fec10-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fec10-115">Application</span></span>|<span data-ttu-id="fec10-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fec10-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fec10-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fec10-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fec10-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fec10-118">Optional query parameters</span></span>
<span data-ttu-id="fec10-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fec10-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fec10-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fec10-120">Request headers</span></span>
|<span data-ttu-id="fec10-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fec10-121">Header</span></span>|<span data-ttu-id="fec10-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fec10-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fec10-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fec10-123">Authorization</span></span>|<span data-ttu-id="fec10-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fec10-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fec10-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fec10-125">Accept</span></span>|<span data-ttu-id="fec10-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fec10-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fec10-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fec10-127">Request body</span></span>
<span data-ttu-id="fec10-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fec10-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fec10-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fec10-129">Response</span></span>
<span data-ttu-id="fec10-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fec10-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fec10-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fec10-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fec10-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fec10-132">Request</span></span>
<span data-ttu-id="fec10-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fec10-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="fec10-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fec10-134">Response</span></span>
<span data-ttu-id="fec10-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fec10-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
    "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7
  }
}
```



