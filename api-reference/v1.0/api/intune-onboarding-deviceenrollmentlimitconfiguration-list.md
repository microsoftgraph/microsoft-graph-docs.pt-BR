---
title: Listar deviceEnrollmentLimitConfigurations
description: Listar propriedades e relações de objetos de deviceEnrollmentLimitConfiguration.
author: tfitzmac
ms.openlocfilehash: db91556e8810109cfcd5e98d54a641451215b36b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348745"
---
# <a name="list-deviceenrollmentlimitconfigurations"></a><span data-ttu-id="4d941-103">Listar deviceEnrollmentLimitConfigurations</span><span class="sxs-lookup"><span data-stu-id="4d941-103">List deviceEnrollmentLimitConfigurations</span></span>

> <span data-ttu-id="4d941-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4d941-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d941-105">Listar propriedades e relações de objetos de [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4d941-105">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d941-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4d941-106">Prerequisites</span></span>
<span data-ttu-id="4d941-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d941-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d941-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d941-109">Permission type</span></span>|<span data-ttu-id="4d941-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4d941-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d941-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d941-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d941-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d941-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4d941-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d941-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d941-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d941-114">Not supported.</span></span>|
|<span data-ttu-id="4d941-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d941-115">Application</span></span>|<span data-ttu-id="4d941-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d941-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d941-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d941-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4d941-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d941-118">Request headers</span></span>
|<span data-ttu-id="4d941-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d941-119">Header</span></span>|<span data-ttu-id="4d941-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4d941-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d941-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d941-121">Authorization</span></span>|<span data-ttu-id="4d941-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d941-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d941-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4d941-123">Accept</span></span>|<span data-ttu-id="4d941-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4d941-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d941-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d941-125">Request body</span></span>
<span data-ttu-id="4d941-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d941-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d941-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d941-127">Response</span></span>
<span data-ttu-id="4d941-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d941-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d941-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d941-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d941-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d941-130">Request</span></span>
<span data-ttu-id="4d941-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d941-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="4d941-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d941-132">Response</span></span>
<span data-ttu-id="4d941-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d941-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



