---
title: Acessar deviceEnrollmentLimitConfiguration
description: Leia as propriedades e as relações do objeto deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1741cae31b1aed982bf2b80abde7b73ba98b94e4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709261"
---
# <a name="get-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="fd673-103">Acessar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd673-103">Get deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="fd673-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd673-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd673-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fd673-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd673-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fd673-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd673-107">Leia as propriedades e as relações do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd673-107">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd673-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd673-108">Prerequisites</span></span>
<span data-ttu-id="fd673-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd673-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd673-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd673-111">Permission type</span></span>|<span data-ttu-id="fd673-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd673-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd673-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd673-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fd673-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd673-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fd673-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd673-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd673-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd673-116">Not supported.</span></span>|
|<span data-ttu-id="fd673-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd673-117">Application</span></span>|<span data-ttu-id="fd673-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd673-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd673-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd673-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd673-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fd673-120">Optional query parameters</span></span>
<span data-ttu-id="fd673-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fd673-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd673-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd673-122">Request headers</span></span>
|<span data-ttu-id="fd673-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd673-123">Header</span></span>|<span data-ttu-id="fd673-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fd673-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd673-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd673-125">Authorization</span></span>|<span data-ttu-id="fd673-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd673-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd673-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd673-127">Accept</span></span>|<span data-ttu-id="fd673-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fd673-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd673-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd673-129">Request body</span></span>
<span data-ttu-id="fd673-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fd673-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd673-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd673-131">Response</span></span>
<span data-ttu-id="fd673-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd673-132">If successful, this method returns a `200 OK` response code and [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd673-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd673-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd673-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd673-134">Request</span></span>
<span data-ttu-id="fd673-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd673-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="fd673-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd673-136">Response</span></span>
<span data-ttu-id="fd673-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd673-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





