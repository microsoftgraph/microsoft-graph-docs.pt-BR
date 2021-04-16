---
title: Função managedDeviceEnrollmentTopFailures
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f853dd3cda226aadc75ab5d0ac4dd66bf926940d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866689"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="2ac2a-103">Função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="2ac2a-103">managedDeviceEnrollmentTopFailures function</span></span>

<span data-ttu-id="2ac2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ac2a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ac2a-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2ac2a-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ac2a-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2ac2a-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ac2a-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ac2a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ac2a-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2ac2a-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2ac2a-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ac2a-109">Prerequisites</span></span>
<span data-ttu-id="2ac2a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ac2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ac2a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ac2a-112">Permission type</span></span>|<span data-ttu-id="2ac2a-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ac2a-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ac2a-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ac2a-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2ac2a-115">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="2ac2a-115">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="2ac2a-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ac2a-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2ac2a-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ac2a-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ac2a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ac2a-118">Not supported.</span></span>|
|<span data-ttu-id="2ac2a-119">Application</span><span class="sxs-lookup"><span data-stu-id="2ac2a-119">Application</span></span>||
| <span data-ttu-id="2ac2a-120">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="2ac2a-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="2ac2a-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ac2a-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ac2a-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ac2a-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="2ac2a-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ac2a-123">Request headers</span></span>
|<span data-ttu-id="2ac2a-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ac2a-124">Header</span></span>|<span data-ttu-id="2ac2a-125">Valor</span><span class="sxs-lookup"><span data-stu-id="2ac2a-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ac2a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ac2a-126">Authorization</span></span>|<span data-ttu-id="2ac2a-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ac2a-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ac2a-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ac2a-128">Accept</span></span>|<span data-ttu-id="2ac2a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="2ac2a-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ac2a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ac2a-130">Request body</span></span>
<span data-ttu-id="2ac2a-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="2ac2a-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2ac2a-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="2ac2a-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2ac2a-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ac2a-133">Property</span></span>|<span data-ttu-id="2ac2a-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ac2a-134">Type</span></span>|<span data-ttu-id="2ac2a-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ac2a-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ac2a-136">ponto</span><span class="sxs-lookup"><span data-stu-id="2ac2a-136">period</span></span>|<span data-ttu-id="2ac2a-137">String</span><span class="sxs-lookup"><span data-stu-id="2ac2a-137">String</span></span>|<span data-ttu-id="2ac2a-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2ac2a-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2ac2a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ac2a-139">Response</span></span>
<span data-ttu-id="2ac2a-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ac2a-140">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ac2a-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ac2a-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="2ac2a-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ac2a-142">Request</span></span>
<span data-ttu-id="2ac2a-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ac2a-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="2ac2a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ac2a-144">Response</span></span>
<span data-ttu-id="2ac2a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ac2a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










