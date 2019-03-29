---
title: Listar deviceComplianceUserStatuses
description: Listar propriedades e relações dos objetos deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9aff77b4d8ea8262e96186ad39f9d1eaa2706b5e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975165"
---
# <a name="list-devicecomplianceuserstatuses"></a><span data-ttu-id="73c7d-103">Listar deviceComplianceUserStatuses</span><span class="sxs-lookup"><span data-stu-id="73c7d-103">List deviceComplianceUserStatuses</span></span>

> <span data-ttu-id="73c7d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73c7d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73c7d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73c7d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73c7d-106">Listar propriedades e relações dos objetos [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="73c7d-106">List properties and relationships of the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73c7d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73c7d-107">Prerequisites</span></span>
<span data-ttu-id="73c7d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73c7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73c7d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73c7d-110">Permission type</span></span>|<span data-ttu-id="73c7d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73c7d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73c7d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73c7d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73c7d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73c7d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="73c7d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73c7d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73c7d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73c7d-115">Not supported.</span></span>|
|<span data-ttu-id="73c7d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73c7d-116">Application</span></span>|<span data-ttu-id="73c7d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73c7d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73c7d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73c7d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="73c7d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73c7d-119">Request headers</span></span>
|<span data-ttu-id="73c7d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73c7d-120">Header</span></span>|<span data-ttu-id="73c7d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="73c7d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73c7d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="73c7d-122">Authorization</span></span>|<span data-ttu-id="73c7d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73c7d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73c7d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73c7d-124">Accept</span></span>|<span data-ttu-id="73c7d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73c7d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73c7d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73c7d-126">Request body</span></span>
<span data-ttu-id="73c7d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73c7d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73c7d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="73c7d-128">Response</span></span>
<span data-ttu-id="73c7d-129">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73c7d-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73c7d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73c7d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="73c7d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73c7d-131">Request</span></span>
<span data-ttu-id="73c7d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73c7d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="73c7d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="73c7d-133">Response</span></span>
<span data-ttu-id="73c7d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73c7d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




