---
title: função managedDeviceEnrollmentTopFailures
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d10f59a07a71406b4cac07072920bd73062375e9
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195815"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="9e04e-103">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="9e04e-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="9e04e-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9e04e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9e04e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9e04e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e04e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e04e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e04e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9e04e-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e04e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e04e-108">Prerequisites</span></span>
<span data-ttu-id="9e04e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e04e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e04e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e04e-111">Permission type</span></span>|<span data-ttu-id="9e04e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9e04e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e04e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e04e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9e04e-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="9e04e-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="9e04e-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e04e-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9e04e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e04e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e04e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e04e-117">Not supported.</span></span>|
|<span data-ttu-id="9e04e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e04e-118">Application</span></span>||
| <span data-ttu-id="9e04e-119">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="9e04e-119">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="9e04e-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e04e-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e04e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e04e-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="9e04e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e04e-122">Request headers</span></span>
|<span data-ttu-id="9e04e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e04e-123">Header</span></span>|<span data-ttu-id="9e04e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="9e04e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e04e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e04e-125">Authorization</span></span>|<span data-ttu-id="9e04e-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e04e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e04e-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e04e-127">Accept</span></span>|<span data-ttu-id="9e04e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9e04e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e04e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e04e-129">Request body</span></span>
<span data-ttu-id="9e04e-130">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="9e04e-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9e04e-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="9e04e-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9e04e-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e04e-132">Property</span></span>|<span data-ttu-id="9e04e-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e04e-133">Type</span></span>|<span data-ttu-id="9e04e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e04e-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e04e-135">ponto</span><span class="sxs-lookup"><span data-stu-id="9e04e-135">period</span></span>|<span data-ttu-id="9e04e-136">String</span><span class="sxs-lookup"><span data-stu-id="9e04e-136">String</span></span>|<span data-ttu-id="9e04e-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9e04e-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9e04e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e04e-138">Response</span></span>
<span data-ttu-id="9e04e-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e04e-139">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e04e-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e04e-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e04e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e04e-141">Request</span></span>
<span data-ttu-id="9e04e-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e04e-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9e04e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e04e-143">Response</span></span>
<span data-ttu-id="9e04e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e04e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







