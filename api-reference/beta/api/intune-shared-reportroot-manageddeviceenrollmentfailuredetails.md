---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: f9dc6f0a1a0a211de1cbfb1443dc4393796bd2d4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337580"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="b6920-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="b6920-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="b6920-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b6920-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6920-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b6920-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6920-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b6920-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6920-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6920-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6920-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6920-108">Prerequisites</span></span>
<span data-ttu-id="b6920-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6920-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6920-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6920-111">Permission type</span></span>|<span data-ttu-id="b6920-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6920-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6920-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6920-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b6920-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="b6920-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b6920-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6920-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b6920-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6920-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6920-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6920-117">Not supported.</span></span>|
|<span data-ttu-id="b6920-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6920-118">Application</span></span>|<span data-ttu-id="b6920-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6920-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6920-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6920-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="b6920-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6920-121">Request headers</span></span>
|<span data-ttu-id="b6920-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6920-122">Header</span></span>|<span data-ttu-id="b6920-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b6920-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6920-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6920-124">Authorization</span></span>|<span data-ttu-id="b6920-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6920-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6920-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b6920-126">Accept</span></span>|<span data-ttu-id="b6920-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b6920-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6920-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6920-128">Request body</span></span>
<span data-ttu-id="b6920-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="b6920-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b6920-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6920-130">Property</span></span>|<span data-ttu-id="b6920-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6920-131">Type</span></span>|<span data-ttu-id="b6920-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6920-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6920-133">filter</span><span class="sxs-lookup"><span data-stu-id="b6920-133">filter</span></span>|<span data-ttu-id="b6920-134">String</span><span class="sxs-lookup"><span data-stu-id="b6920-134">String</span></span>|<span data-ttu-id="b6920-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6920-135">Not yet documented</span></span>|
|<span data-ttu-id="b6920-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="b6920-136">skipToken</span></span>|<span data-ttu-id="b6920-137">String</span><span class="sxs-lookup"><span data-stu-id="b6920-137">String</span></span>|<span data-ttu-id="b6920-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6920-138">Not yet documented</span></span>|
|<span data-ttu-id="b6920-139">skip</span><span class="sxs-lookup"><span data-stu-id="b6920-139">skip</span></span>|<span data-ttu-id="b6920-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b6920-140">Int32</span></span>|<span data-ttu-id="b6920-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6920-141">Not yet documented</span></span>|
|<span data-ttu-id="b6920-142">top</span><span class="sxs-lookup"><span data-stu-id="b6920-142">top</span></span>|<span data-ttu-id="b6920-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b6920-143">Int32</span></span>|<span data-ttu-id="b6920-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6920-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b6920-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6920-145">Response</span></span>
<span data-ttu-id="b6920-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6920-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6920-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6920-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6920-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6920-148">Request</span></span>
<span data-ttu-id="b6920-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6920-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b6920-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6920-150">Response</span></span>
<span data-ttu-id="b6920-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6920-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



