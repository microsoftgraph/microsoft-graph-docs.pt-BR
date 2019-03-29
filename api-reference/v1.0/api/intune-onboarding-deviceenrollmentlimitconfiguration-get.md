---
title: Acessar deviceEnrollmentLimitConfiguration
description: Leia as propriedades e as relações do objeto deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6806cdc0fc02a1edcec712a4a39e0dc4b50578b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966065"
---
# <a name="get-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="b6ed6-103">Acessar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="b6ed6-103">Get deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="b6ed6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6ed6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6ed6-105">Leia as propriedades e as relações do objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6ed6-105">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6ed6-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6ed6-106">Prerequisites</span></span>
<span data-ttu-id="b6ed6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6ed6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6ed6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6ed6-109">Permission type</span></span>|<span data-ttu-id="b6ed6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6ed6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6ed6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6ed6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b6ed6-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6ed6-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b6ed6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6ed6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6ed6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6ed6-114">Not supported.</span></span>|
|<span data-ttu-id="b6ed6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6ed6-115">Application</span></span>|<span data-ttu-id="b6ed6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6ed6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6ed6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6ed6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6ed6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6ed6-118">Optional query parameters</span></span>
<span data-ttu-id="b6ed6-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6ed6-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6ed6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6ed6-120">Request headers</span></span>
|<span data-ttu-id="b6ed6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6ed6-121">Header</span></span>|<span data-ttu-id="b6ed6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6ed6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6ed6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6ed6-123">Authorization</span></span>|<span data-ttu-id="b6ed6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6ed6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6ed6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6ed6-125">Accept</span></span>|<span data-ttu-id="b6ed6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6ed6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6ed6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6ed6-127">Request body</span></span>
<span data-ttu-id="b6ed6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6ed6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6ed6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6ed6-129">Response</span></span>
<span data-ttu-id="b6ed6-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6ed6-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6ed6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6ed6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6ed6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6ed6-132">Request</span></span>
<span data-ttu-id="b6ed6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6ed6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b6ed6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6ed6-134">Response</span></span>
<span data-ttu-id="b6ed6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6ed6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



