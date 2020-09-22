---
title: Listar deviceCompliancePolicies
description: Listar propriedades e relações dos objetos deviceCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ad3115207e7d8ab19e3abf053872d1001ddbf34e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083488"
---
# <a name="list-devicecompliancepolicies"></a><span data-ttu-id="c8455-103">Listar deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="c8455-103">List deviceCompliancePolicies</span></span>

<span data-ttu-id="c8455-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8455-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8455-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8455-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8455-106">Listar propriedades e relações dos objetos [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c8455-106">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8455-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8455-107">Prerequisites</span></span>
<span data-ttu-id="c8455-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8455-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8455-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8455-110">Permission type</span></span>|<span data-ttu-id="c8455-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8455-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8455-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8455-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8455-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8455-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c8455-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8455-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8455-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8455-115">Not supported.</span></span>|
|<span data-ttu-id="c8455-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8455-116">Application</span></span>|<span data-ttu-id="c8455-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8455-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8455-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8455-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c8455-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8455-119">Request headers</span></span>
|<span data-ttu-id="c8455-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8455-120">Header</span></span>|<span data-ttu-id="c8455-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c8455-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8455-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8455-122">Authorization</span></span>|<span data-ttu-id="c8455-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8455-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8455-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8455-124">Accept</span></span>|<span data-ttu-id="c8455-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8455-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8455-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8455-126">Request body</span></span>
<span data-ttu-id="c8455-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8455-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8455-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8455-128">Response</span></span>
<span data-ttu-id="c8455-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8455-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8455-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8455-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8455-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8455-131">Request</span></span>
<span data-ttu-id="c8455-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8455-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="c8455-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8455-133">Response</span></span>
<span data-ttu-id="c8455-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8455-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 393

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
      "id": "4214b716-b716-4214-16b7-144216b71442",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```









