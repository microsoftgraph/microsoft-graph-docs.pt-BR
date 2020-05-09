---
title: Acessar deviceEnrollmentLimitConfiguration
description: Leia as propriedades e as relações do objeto deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 77891153bf4e85089a48f6ccbd94932baaf4850e
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177748"
---
# <a name="get-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="81ced-103">Acessar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="81ced-103">Get deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="81ced-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81ced-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81ced-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81ced-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81ced-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81ced-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81ced-107">Leia as propriedades e as relações do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81ced-107">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81ced-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81ced-108">Prerequisites</span></span>
<span data-ttu-id="81ced-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81ced-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81ced-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81ced-111">Permission type</span></span>|<span data-ttu-id="81ced-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81ced-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81ced-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81ced-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81ced-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="81ced-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="81ced-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81ced-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81ced-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81ced-116">Not supported.</span></span>|
|<span data-ttu-id="81ced-117">Application</span><span class="sxs-lookup"><span data-stu-id="81ced-117">Application</span></span>|<span data-ttu-id="81ced-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="81ced-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81ced-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81ced-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81ced-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="81ced-120">Optional query parameters</span></span>
<span data-ttu-id="81ced-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="81ced-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81ced-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81ced-122">Request headers</span></span>
|<span data-ttu-id="81ced-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81ced-123">Header</span></span>|<span data-ttu-id="81ced-124">Valor</span><span class="sxs-lookup"><span data-stu-id="81ced-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81ced-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="81ced-125">Authorization</span></span>|<span data-ttu-id="81ced-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81ced-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81ced-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81ced-127">Accept</span></span>|<span data-ttu-id="81ced-128">application/json</span><span class="sxs-lookup"><span data-stu-id="81ced-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81ced-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81ced-129">Request body</span></span>
<span data-ttu-id="81ced-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81ced-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81ced-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="81ced-131">Response</span></span>
<span data-ttu-id="81ced-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81ced-132">If successful, this method returns a `200 OK` response code and [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81ced-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81ced-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="81ced-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81ced-134">Request</span></span>
<span data-ttu-id="81ced-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81ced-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="81ced-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="81ced-136">Response</span></span>
<span data-ttu-id="81ced-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81ced-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 482

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
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "limit": 5
  }
}
```



