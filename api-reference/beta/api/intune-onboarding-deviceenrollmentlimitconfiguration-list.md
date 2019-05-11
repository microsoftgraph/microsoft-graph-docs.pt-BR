---
title: Listar deviceEnrollmentLimitConfigurations
description: Listar propriedades e relações de objetos de deviceEnrollmentLimitConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97febf4b0ee4b85dbd46dbb295e92ebaeb0b12f9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900276"
---
# <a name="list-deviceenrollmentlimitconfigurations"></a><span data-ttu-id="68af5-103">Listar deviceEnrollmentLimitConfigurations</span><span class="sxs-lookup"><span data-stu-id="68af5-103">List deviceEnrollmentLimitConfigurations</span></span>

> <span data-ttu-id="68af5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="68af5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68af5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="68af5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68af5-106">Listar propriedades e relações de objetos de [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68af5-106">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68af5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="68af5-107">Prerequisites</span></span>
<span data-ttu-id="68af5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68af5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68af5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68af5-110">Permission type</span></span>|<span data-ttu-id="68af5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="68af5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68af5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68af5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68af5-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="68af5-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="68af5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68af5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68af5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68af5-115">Not supported.</span></span>|
|<span data-ttu-id="68af5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68af5-116">Application</span></span>|<span data-ttu-id="68af5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68af5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68af5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68af5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="68af5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68af5-119">Request headers</span></span>
|<span data-ttu-id="68af5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68af5-120">Header</span></span>|<span data-ttu-id="68af5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="68af5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68af5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="68af5-122">Authorization</span></span>|<span data-ttu-id="68af5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68af5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68af5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="68af5-124">Accept</span></span>|<span data-ttu-id="68af5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="68af5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68af5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68af5-126">Request body</span></span>
<span data-ttu-id="68af5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="68af5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68af5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="68af5-128">Response</span></span>
<span data-ttu-id="68af5-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68af5-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68af5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68af5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="68af5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68af5-131">Request</span></span>
<span data-ttu-id="68af5-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68af5-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="68af5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="68af5-133">Response</span></span>
<span data-ttu-id="68af5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68af5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 446

{
  "value": [
    {
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
  ]
}
```




