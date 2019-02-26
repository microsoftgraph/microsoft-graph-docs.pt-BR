---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9521a2265e6fcdb86b60d6fc427c74d74be0b31f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164376"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="b5390-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="b5390-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="b5390-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b5390-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b5390-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b5390-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5390-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b5390-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5390-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b5390-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b5390-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b5390-108">Prerequisites</span></span>
<span data-ttu-id="b5390-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5390-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="b5390-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5390-111">Permission type</span></span>|<span data-ttu-id="b5390-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b5390-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5390-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5390-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b5390-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="b5390-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b5390-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5390-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b5390-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5390-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5390-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5390-117">Not supported.</span></span>|
|<span data-ttu-id="b5390-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5390-118">Application</span></span>|<span data-ttu-id="b5390-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5390-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5390-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5390-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="b5390-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5390-121">Request headers</span></span>
|<span data-ttu-id="b5390-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b5390-122">Header</span></span>|<span data-ttu-id="b5390-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b5390-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5390-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5390-124">Authorization</span></span>|<span data-ttu-id="b5390-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5390-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5390-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b5390-126">Accept</span></span>|<span data-ttu-id="b5390-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b5390-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5390-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5390-128">Request body</span></span>
<span data-ttu-id="b5390-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="b5390-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b5390-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5390-130">Property</span></span>|<span data-ttu-id="b5390-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5390-131">Type</span></span>|<span data-ttu-id="b5390-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5390-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5390-133">filter</span><span class="sxs-lookup"><span data-stu-id="b5390-133">filter</span></span>|<span data-ttu-id="b5390-134">String</span><span class="sxs-lookup"><span data-stu-id="b5390-134">String</span></span>|<span data-ttu-id="b5390-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b5390-135">Not yet documented</span></span>|
|<span data-ttu-id="b5390-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="b5390-136">skipToken</span></span>|<span data-ttu-id="b5390-137">String</span><span class="sxs-lookup"><span data-stu-id="b5390-137">String</span></span>|<span data-ttu-id="b5390-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b5390-138">Not yet documented</span></span>|
|<span data-ttu-id="b5390-139">skip</span><span class="sxs-lookup"><span data-stu-id="b5390-139">skip</span></span>|<span data-ttu-id="b5390-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b5390-140">Int32</span></span>|<span data-ttu-id="b5390-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b5390-141">Not yet documented</span></span>|
|<span data-ttu-id="b5390-142">top</span><span class="sxs-lookup"><span data-stu-id="b5390-142">top</span></span>|<span data-ttu-id="b5390-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b5390-143">Int32</span></span>|<span data-ttu-id="b5390-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b5390-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b5390-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5390-145">Response</span></span>
<span data-ttu-id="b5390-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5390-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5390-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5390-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5390-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5390-148">Request</span></span>
<span data-ttu-id="b5390-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5390-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b5390-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5390-150">Response</span></span>
<span data-ttu-id="b5390-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5390-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



