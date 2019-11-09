---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a3c12467127bb47d54e824da2349ace7b9e2463d
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085679"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="a950c-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="a950c-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="a950c-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a950c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a950c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a950c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a950c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a950c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a950c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a950c-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a950c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a950c-108">Prerequisites</span></span>
<span data-ttu-id="a950c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a950c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a950c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a950c-111">Permission type</span></span>|<span data-ttu-id="a950c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a950c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a950c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a950c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a950c-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="a950c-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a950c-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a950c-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a950c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a950c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a950c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a950c-117">Not supported.</span></span>|
|<span data-ttu-id="a950c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a950c-118">Application</span></span>||
| <span data-ttu-id="a950c-119">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="a950c-119">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a950c-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a950c-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a950c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a950c-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="a950c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a950c-122">Request headers</span></span>
|<span data-ttu-id="a950c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a950c-123">Header</span></span>|<span data-ttu-id="a950c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a950c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a950c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a950c-125">Authorization</span></span>|<span data-ttu-id="a950c-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a950c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a950c-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a950c-127">Accept</span></span>|<span data-ttu-id="a950c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a950c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a950c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a950c-129">Request body</span></span>
<span data-ttu-id="a950c-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="a950c-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a950c-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a950c-131">Property</span></span>|<span data-ttu-id="a950c-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a950c-132">Type</span></span>|<span data-ttu-id="a950c-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a950c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a950c-134">filter</span><span class="sxs-lookup"><span data-stu-id="a950c-134">filter</span></span>|<span data-ttu-id="a950c-135">String</span><span class="sxs-lookup"><span data-stu-id="a950c-135">String</span></span>|<span data-ttu-id="a950c-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a950c-136">Not yet documented</span></span>|
|<span data-ttu-id="a950c-137">skipToken</span><span class="sxs-lookup"><span data-stu-id="a950c-137">skipToken</span></span>|<span data-ttu-id="a950c-138">String</span><span class="sxs-lookup"><span data-stu-id="a950c-138">String</span></span>|<span data-ttu-id="a950c-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a950c-139">Not yet documented</span></span>|
|<span data-ttu-id="a950c-140">skip</span><span class="sxs-lookup"><span data-stu-id="a950c-140">skip</span></span>|<span data-ttu-id="a950c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a950c-141">Int32</span></span>|<span data-ttu-id="a950c-142">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a950c-142">Not yet documented</span></span>|
|<span data-ttu-id="a950c-143">top</span><span class="sxs-lookup"><span data-stu-id="a950c-143">top</span></span>|<span data-ttu-id="a950c-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a950c-144">Int32</span></span>|<span data-ttu-id="a950c-145">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a950c-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a950c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a950c-146">Response</span></span>
<span data-ttu-id="a950c-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a950c-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a950c-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a950c-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="a950c-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a950c-149">Request</span></span>
<span data-ttu-id="a950c-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a950c-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a950c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a950c-151">Response</span></span>
<span data-ttu-id="a950c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a950c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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












