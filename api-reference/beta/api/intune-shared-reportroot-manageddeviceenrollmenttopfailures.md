---
title: função managedDeviceEnrollmentTopFailures
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cd03290845fdf672fa298cfc4996785e8d3cddc8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898225"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="e82f3-103">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="e82f3-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="e82f3-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e82f3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e82f3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e82f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e82f3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e82f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e82f3-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e82f3-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e82f3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e82f3-108">Prerequisites</span></span>
<span data-ttu-id="e82f3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e82f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e82f3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e82f3-111">Permission type</span></span>|<span data-ttu-id="e82f3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e82f3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e82f3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e82f3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e82f3-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="e82f3-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e82f3-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e82f3-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e82f3-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e82f3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e82f3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e82f3-117">Not supported.</span></span>|
|<span data-ttu-id="e82f3-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e82f3-118">Application</span></span>|<span data-ttu-id="e82f3-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e82f3-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e82f3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e82f3-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="e82f3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e82f3-121">Request headers</span></span>
|<span data-ttu-id="e82f3-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e82f3-122">Header</span></span>|<span data-ttu-id="e82f3-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e82f3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e82f3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e82f3-124">Authorization</span></span>|<span data-ttu-id="e82f3-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e82f3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e82f3-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e82f3-126">Accept</span></span>|<span data-ttu-id="e82f3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e82f3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e82f3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e82f3-128">Request body</span></span>
<span data-ttu-id="e82f3-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="e82f3-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e82f3-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="e82f3-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e82f3-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e82f3-131">Property</span></span>|<span data-ttu-id="e82f3-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="e82f3-132">Type</span></span>|<span data-ttu-id="e82f3-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="e82f3-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e82f3-134">ponto</span><span class="sxs-lookup"><span data-stu-id="e82f3-134">period</span></span>|<span data-ttu-id="e82f3-135">String</span><span class="sxs-lookup"><span data-stu-id="e82f3-135">String</span></span>|<span data-ttu-id="e82f3-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e82f3-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e82f3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e82f3-137">Response</span></span>
<span data-ttu-id="e82f3-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e82f3-138">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e82f3-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e82f3-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="e82f3-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e82f3-140">Request</span></span>
<span data-ttu-id="e82f3-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e82f3-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e82f3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e82f3-142">Response</span></span>
<span data-ttu-id="e82f3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e82f3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



