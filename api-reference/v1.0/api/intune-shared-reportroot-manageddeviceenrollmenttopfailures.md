---
title: função managedDeviceEnrollmentTopFailures
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df7e3331194f274ea1b6035d640e780e212a88b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972893"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="e1000-103">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="e1000-103">managedDeviceEnrollmentTopFailures function</span></span>

<span data-ttu-id="e1000-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1000-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1000-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1000-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1000-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e1000-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1000-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1000-107">Prerequisites</span></span>
<span data-ttu-id="e1000-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1000-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1000-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1000-110">Permission type</span></span>|<span data-ttu-id="e1000-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1000-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1000-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1000-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e1000-113">&nbsp;&nbsp;Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="e1000-113">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="e1000-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1000-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e1000-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1000-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1000-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1000-116">Not supported.</span></span>|
|<span data-ttu-id="e1000-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1000-117">Application</span></span>|<span data-ttu-id="e1000-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1000-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1000-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1000-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="e1000-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1000-120">Request headers</span></span>
|<span data-ttu-id="e1000-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1000-121">Header</span></span>|<span data-ttu-id="e1000-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e1000-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1000-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1000-123">Authorization</span></span>|<span data-ttu-id="e1000-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1000-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1000-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1000-125">Accept</span></span>|<span data-ttu-id="e1000-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1000-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1000-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1000-127">Request body</span></span>
<span data-ttu-id="e1000-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="e1000-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e1000-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="e1000-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e1000-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1000-130">Property</span></span>|<span data-ttu-id="e1000-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1000-131">Type</span></span>|<span data-ttu-id="e1000-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1000-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1000-133">ponto</span><span class="sxs-lookup"><span data-stu-id="e1000-133">period</span></span>|<span data-ttu-id="e1000-134">String</span><span class="sxs-lookup"><span data-stu-id="e1000-134">String</span></span>|<span data-ttu-id="e1000-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e1000-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e1000-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1000-136">Response</span></span>
<span data-ttu-id="e1000-137">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1000-137">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1000-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1000-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1000-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1000-139">Request</span></span>
<span data-ttu-id="e1000-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1000-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e1000-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1000-141">Response</span></span>
<span data-ttu-id="e1000-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1000-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```










