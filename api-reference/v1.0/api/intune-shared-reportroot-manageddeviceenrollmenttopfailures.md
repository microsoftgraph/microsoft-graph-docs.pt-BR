---
title: função managedDeviceEnrollmentTopFailures
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2cdc523507964f87863131ef114b102f383524a8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576787"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="57ab4-103">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="57ab4-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="57ab4-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57ab4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57ab4-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="57ab4-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57ab4-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57ab4-106">Prerequisites</span></span>
<span data-ttu-id="57ab4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57ab4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57ab4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57ab4-109">Permission type</span></span>|<span data-ttu-id="57ab4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57ab4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57ab4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57ab4-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="57ab4-112">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="57ab4-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="57ab4-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57ab4-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="57ab4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57ab4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57ab4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57ab4-115">Not supported.</span></span>|
|<span data-ttu-id="57ab4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57ab4-116">Application</span></span>|<span data-ttu-id="57ab4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57ab4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57ab4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57ab4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="57ab4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57ab4-119">Request headers</span></span>
|<span data-ttu-id="57ab4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57ab4-120">Header</span></span>|<span data-ttu-id="57ab4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="57ab4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57ab4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="57ab4-122">Authorization</span></span>|<span data-ttu-id="57ab4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57ab4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57ab4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57ab4-124">Accept</span></span>|<span data-ttu-id="57ab4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57ab4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57ab4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57ab4-126">Request body</span></span>
<span data-ttu-id="57ab4-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="57ab4-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="57ab4-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="57ab4-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="57ab4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57ab4-129">Property</span></span>|<span data-ttu-id="57ab4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="57ab4-130">Type</span></span>|<span data-ttu-id="57ab4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="57ab4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57ab4-132">ponto</span><span class="sxs-lookup"><span data-stu-id="57ab4-132">period</span></span>|<span data-ttu-id="57ab4-133">String</span><span class="sxs-lookup"><span data-stu-id="57ab4-133">String</span></span>|<span data-ttu-id="57ab4-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="57ab4-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="57ab4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="57ab4-135">Response</span></span>
<span data-ttu-id="57ab4-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57ab4-136">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57ab4-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57ab4-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="57ab4-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57ab4-138">Request</span></span>
<span data-ttu-id="57ab4-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57ab4-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="57ab4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="57ab4-140">Response</span></span>
<span data-ttu-id="57ab4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57ab4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




