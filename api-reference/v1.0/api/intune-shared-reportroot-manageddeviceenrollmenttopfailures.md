---
title: Função managedDeviceEnrollmentTopFailures
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df7e3331194f274ea1b6035d640e780e212a88b0
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732244"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="c7e34-103">Função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="c7e34-103">managedDeviceEnrollmentTopFailures function</span></span>

<span data-ttu-id="c7e34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7e34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7e34-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7e34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7e34-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c7e34-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7e34-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7e34-107">Prerequisites</span></span>
<span data-ttu-id="c7e34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7e34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7e34-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7e34-110">Permission type</span></span>|<span data-ttu-id="c7e34-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7e34-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7e34-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7e34-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c7e34-113">&nbsp;&nbsp;Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="c7e34-113">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="c7e34-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7e34-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c7e34-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7e34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7e34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7e34-116">Not supported.</span></span>|
|<span data-ttu-id="c7e34-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7e34-117">Application</span></span>|<span data-ttu-id="c7e34-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7e34-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7e34-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7e34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="c7e34-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7e34-120">Request headers</span></span>
|<span data-ttu-id="c7e34-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7e34-121">Header</span></span>|<span data-ttu-id="c7e34-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c7e34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7e34-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7e34-123">Authorization</span></span>|<span data-ttu-id="c7e34-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7e34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7e34-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7e34-125">Accept</span></span>|<span data-ttu-id="c7e34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7e34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7e34-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7e34-127">Request body</span></span>
<span data-ttu-id="c7e34-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="c7e34-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="c7e34-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="c7e34-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="c7e34-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7e34-130">Property</span></span>|<span data-ttu-id="c7e34-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7e34-131">Type</span></span>|<span data-ttu-id="c7e34-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7e34-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7e34-133">ponto</span><span class="sxs-lookup"><span data-stu-id="c7e34-133">period</span></span>|<span data-ttu-id="c7e34-134">String</span><span class="sxs-lookup"><span data-stu-id="c7e34-134">String</span></span>|<span data-ttu-id="c7e34-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c7e34-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c7e34-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7e34-136">Response</span></span>
<span data-ttu-id="c7e34-137">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7e34-137">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7e34-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7e34-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7e34-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7e34-139">Request</span></span>
<span data-ttu-id="c7e34-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7e34-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="c7e34-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7e34-141">Response</span></span>
<span data-ttu-id="c7e34-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7e34-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










