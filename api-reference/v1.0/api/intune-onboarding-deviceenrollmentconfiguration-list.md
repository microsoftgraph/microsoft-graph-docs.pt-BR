---
title: Listar deviceEnrollmentConfigurations
description: Listar propriedades e relações de objetos de deviceEnrollmentConfiguration.
ms.openlocfilehash: 45fcc3fb7fe3a1dfaae3d8591dd37213bc1be9f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005974"
---
# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="ebfcb-103">Listar deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="ebfcb-103">List deviceEnrollmentConfigurations</span></span>

> <span data-ttu-id="ebfcb-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ebfcb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebfcb-105">Listar propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebfcb-105">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ebfcb-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ebfcb-106">Prerequisites</span></span>
<span data-ttu-id="ebfcb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebfcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebfcb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebfcb-109">Permission type</span></span>|<span data-ttu-id="ebfcb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ebfcb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebfcb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebfcb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ebfcb-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebfcb-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ebfcb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebfcb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebfcb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebfcb-114">Not supported.</span></span>|
|<span data-ttu-id="ebfcb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebfcb-115">Application</span></span>|<span data-ttu-id="ebfcb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebfcb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebfcb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebfcb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ebfcb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebfcb-118">Request headers</span></span>
|<span data-ttu-id="ebfcb-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebfcb-119">Header</span></span>|<span data-ttu-id="ebfcb-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ebfcb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebfcb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebfcb-121">Authorization</span></span>|<span data-ttu-id="ebfcb-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebfcb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebfcb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ebfcb-123">Accept</span></span>|<span data-ttu-id="ebfcb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ebfcb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebfcb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebfcb-125">Request body</span></span>
<span data-ttu-id="ebfcb-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ebfcb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebfcb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebfcb-127">Response</span></span>
<span data-ttu-id="ebfcb-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebfcb-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebfcb-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebfcb-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="ebfcb-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebfcb-130">Request</span></span>
<span data-ttu-id="ebfcb-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebfcb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="ebfcb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebfcb-132">Response</span></span>
<span data-ttu-id="ebfcb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebfcb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



