---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
ms.openlocfilehash: 92a06a4fae5d469759f633698abcf7bff2bfb322
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037393"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="509e0-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="509e0-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="509e0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="509e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="509e0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="509e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="509e0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="509e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="509e0-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="509e0-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="509e0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="509e0-108">Prerequisites</span></span>
<span data-ttu-id="509e0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="509e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="509e0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="509e0-111">Permission type</span></span>|<span data-ttu-id="509e0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="509e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="509e0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="509e0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="509e0-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="509e0-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="509e0-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="509e0-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="509e0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="509e0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="509e0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="509e0-117">Not supported.</span></span>|
|<span data-ttu-id="509e0-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="509e0-118">Application</span></span>|<span data-ttu-id="509e0-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="509e0-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="509e0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="509e0-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="509e0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="509e0-121">Request headers</span></span>
|<span data-ttu-id="509e0-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="509e0-122">Header</span></span>|<span data-ttu-id="509e0-123">Valor</span><span class="sxs-lookup"><span data-stu-id="509e0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="509e0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="509e0-124">Authorization</span></span>|<span data-ttu-id="509e0-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="509e0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="509e0-126">Accept</span><span class="sxs-lookup"><span data-stu-id="509e0-126">Accept</span></span>|<span data-ttu-id="509e0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="509e0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="509e0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="509e0-128">Request body</span></span>
<span data-ttu-id="509e0-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="509e0-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="509e0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="509e0-130">Property</span></span>|<span data-ttu-id="509e0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="509e0-131">Type</span></span>|<span data-ttu-id="509e0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="509e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="509e0-133">filter</span><span class="sxs-lookup"><span data-stu-id="509e0-133">filter</span></span>|<span data-ttu-id="509e0-134">String</span><span class="sxs-lookup"><span data-stu-id="509e0-134">String</span></span>|<span data-ttu-id="509e0-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="509e0-135">Not yet documented</span></span>|
|<span data-ttu-id="509e0-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="509e0-136">skipToken</span></span>|<span data-ttu-id="509e0-137">String</span><span class="sxs-lookup"><span data-stu-id="509e0-137">String</span></span>|<span data-ttu-id="509e0-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="509e0-138">Not yet documented</span></span>|
|<span data-ttu-id="509e0-139">skip</span><span class="sxs-lookup"><span data-stu-id="509e0-139">skip</span></span>|<span data-ttu-id="509e0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="509e0-140">Int32</span></span>|<span data-ttu-id="509e0-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="509e0-141">Not yet documented</span></span>|
|<span data-ttu-id="509e0-142">top</span><span class="sxs-lookup"><span data-stu-id="509e0-142">top</span></span>|<span data-ttu-id="509e0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="509e0-143">Int32</span></span>|<span data-ttu-id="509e0-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="509e0-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="509e0-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="509e0-145">Response</span></span>
<span data-ttu-id="509e0-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="509e0-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="509e0-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="509e0-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="509e0-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="509e0-148">Request</span></span>
<span data-ttu-id="509e0-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="509e0-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="509e0-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="509e0-150">Response</span></span>
<span data-ttu-id="509e0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="509e0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



