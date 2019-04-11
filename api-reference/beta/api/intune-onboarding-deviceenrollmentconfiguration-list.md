---
title: Listar deviceEnrollmentConfigurations
description: Listar propriedades e relações de objetos de deviceEnrollmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e73ab2d946e760eca1e8648f9beff737f6fd840
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801796"
---
# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="13c60-103">Listar deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="13c60-103">List deviceEnrollmentConfigurations</span></span>

> <span data-ttu-id="13c60-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="13c60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13c60-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13c60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13c60-106">Listar propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13c60-106">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13c60-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13c60-107">Prerequisites</span></span>
<span data-ttu-id="13c60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13c60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13c60-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13c60-110">Permission type</span></span>|<span data-ttu-id="13c60-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13c60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13c60-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13c60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13c60-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="13c60-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="13c60-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13c60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13c60-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13c60-115">Not supported.</span></span>|
|<span data-ttu-id="13c60-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13c60-116">Application</span></span>|<span data-ttu-id="13c60-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13c60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13c60-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13c60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="13c60-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13c60-119">Request headers</span></span>
|<span data-ttu-id="13c60-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13c60-120">Header</span></span>|<span data-ttu-id="13c60-121">Valor</span><span class="sxs-lookup"><span data-stu-id="13c60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13c60-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="13c60-122">Authorization</span></span>|<span data-ttu-id="13c60-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13c60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13c60-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13c60-124">Accept</span></span>|<span data-ttu-id="13c60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13c60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13c60-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13c60-126">Request body</span></span>
<span data-ttu-id="13c60-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13c60-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13c60-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="13c60-128">Response</span></span>
<span data-ttu-id="13c60-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13c60-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13c60-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13c60-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="13c60-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13c60-131">Request</span></span>
<span data-ttu-id="13c60-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13c60-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="13c60-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="13c60-133">Response</span></span>
<span data-ttu-id="13c60-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13c60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```





