---
title: Listar deviceComplianceUserStatuses
description: Listar propriedades e relações dos objetos deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 517bf763f6b7de4c65b2106d7a50af7ecf263313
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839960"
---
# <a name="list-devicecomplianceuserstatuses"></a><span data-ttu-id="be6f5-103">Listar deviceComplianceUserStatuses</span><span class="sxs-lookup"><span data-stu-id="be6f5-103">List deviceComplianceUserStatuses</span></span>

> <span data-ttu-id="be6f5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="be6f5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be6f5-105">Listar propriedades e relações dos objetos [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="be6f5-105">List properties and relationships of the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be6f5-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be6f5-106">Prerequisites</span></span>
<span data-ttu-id="be6f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be6f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be6f5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be6f5-109">Permission type</span></span>|<span data-ttu-id="be6f5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="be6f5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be6f5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be6f5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="be6f5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="be6f5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="be6f5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be6f5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be6f5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be6f5-114">Not supported.</span></span>|
|<span data-ttu-id="be6f5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be6f5-115">Application</span></span>|<span data-ttu-id="be6f5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be6f5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be6f5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be6f5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="be6f5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be6f5-118">Request headers</span></span>
|<span data-ttu-id="be6f5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be6f5-119">Header</span></span>|<span data-ttu-id="be6f5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="be6f5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be6f5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="be6f5-121">Authorization</span></span>|<span data-ttu-id="be6f5-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be6f5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be6f5-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="be6f5-123">Accept</span></span>|<span data-ttu-id="be6f5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="be6f5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be6f5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be6f5-125">Request body</span></span>
<span data-ttu-id="be6f5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be6f5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be6f5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="be6f5-127">Response</span></span>
<span data-ttu-id="be6f5-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be6f5-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be6f5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be6f5-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="be6f5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be6f5-130">Request</span></span>
<span data-ttu-id="be6f5-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be6f5-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="be6f5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="be6f5-132">Response</span></span>
<span data-ttu-id="be6f5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be6f5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 397

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
      "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



