---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8d526c66c99e25d7e23340e7acc992badeac1c9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800680"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="857bf-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="857bf-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="857bf-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="857bf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="857bf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="857bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="857bf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="857bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="857bf-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="857bf-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="857bf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="857bf-108">Prerequisites</span></span>
<span data-ttu-id="857bf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="857bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="857bf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="857bf-111">Permission type</span></span>|<span data-ttu-id="857bf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="857bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="857bf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="857bf-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="857bf-114">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="857bf-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="857bf-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="857bf-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="857bf-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="857bf-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="857bf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="857bf-117">Not supported.</span></span>|
|<span data-ttu-id="857bf-118">Application</span><span class="sxs-lookup"><span data-stu-id="857bf-118">Application</span></span>||
| <span data-ttu-id="857bf-119">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="857bf-119">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="857bf-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="857bf-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="857bf-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="857bf-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="857bf-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="857bf-122">Request headers</span></span>
|<span data-ttu-id="857bf-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="857bf-123">Header</span></span>|<span data-ttu-id="857bf-124">Valor</span><span class="sxs-lookup"><span data-stu-id="857bf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="857bf-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="857bf-125">Authorization</span></span>|<span data-ttu-id="857bf-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="857bf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="857bf-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="857bf-127">Accept</span></span>|<span data-ttu-id="857bf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="857bf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="857bf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="857bf-129">Request body</span></span>
<span data-ttu-id="857bf-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="857bf-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="857bf-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="857bf-131">Property</span></span>|<span data-ttu-id="857bf-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="857bf-132">Type</span></span>|<span data-ttu-id="857bf-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="857bf-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="857bf-134">filter</span><span class="sxs-lookup"><span data-stu-id="857bf-134">filter</span></span>|<span data-ttu-id="857bf-135">String</span><span class="sxs-lookup"><span data-stu-id="857bf-135">String</span></span>|<span data-ttu-id="857bf-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="857bf-136">Not yet documented</span></span>|
|<span data-ttu-id="857bf-137">skipToken</span><span class="sxs-lookup"><span data-stu-id="857bf-137">skipToken</span></span>|<span data-ttu-id="857bf-138">String</span><span class="sxs-lookup"><span data-stu-id="857bf-138">String</span></span>|<span data-ttu-id="857bf-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="857bf-139">Not yet documented</span></span>|
|<span data-ttu-id="857bf-140">skip</span><span class="sxs-lookup"><span data-stu-id="857bf-140">skip</span></span>|<span data-ttu-id="857bf-141">Int32</span><span class="sxs-lookup"><span data-stu-id="857bf-141">Int32</span></span>|<span data-ttu-id="857bf-142">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="857bf-142">Not yet documented</span></span>|
|<span data-ttu-id="857bf-143">top</span><span class="sxs-lookup"><span data-stu-id="857bf-143">top</span></span>|<span data-ttu-id="857bf-144">Int32</span><span class="sxs-lookup"><span data-stu-id="857bf-144">Int32</span></span>|<span data-ttu-id="857bf-145">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="857bf-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="857bf-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="857bf-146">Response</span></span>
<span data-ttu-id="857bf-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="857bf-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="857bf-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="857bf-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="857bf-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="857bf-149">Request</span></span>
<span data-ttu-id="857bf-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="857bf-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="857bf-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="857bf-151">Response</span></span>
<span data-ttu-id="857bf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="857bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










