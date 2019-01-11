---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6902a10d7558426d1547bfb590922c225414ad54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827332"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="07c57-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="07c57-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="07c57-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="07c57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07c57-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="07c57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07c57-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="07c57-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07c57-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07c57-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="07c57-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07c57-108">Prerequisites</span></span>
<span data-ttu-id="07c57-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07c57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07c57-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07c57-111">Permission type</span></span>|<span data-ttu-id="07c57-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07c57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07c57-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07c57-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="07c57-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="07c57-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="07c57-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07c57-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="07c57-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07c57-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07c57-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07c57-117">Not supported.</span></span>|
|<span data-ttu-id="07c57-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07c57-118">Application</span></span>|<span data-ttu-id="07c57-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07c57-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07c57-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07c57-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="07c57-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07c57-121">Request headers</span></span>
|<span data-ttu-id="07c57-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07c57-122">Header</span></span>|<span data-ttu-id="07c57-123">Valor</span><span class="sxs-lookup"><span data-stu-id="07c57-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07c57-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="07c57-124">Authorization</span></span>|<span data-ttu-id="07c57-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07c57-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07c57-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07c57-126">Accept</span></span>|<span data-ttu-id="07c57-127">application/json</span><span class="sxs-lookup"><span data-stu-id="07c57-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07c57-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07c57-128">Request body</span></span>
<span data-ttu-id="07c57-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="07c57-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="07c57-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07c57-130">Property</span></span>|<span data-ttu-id="07c57-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="07c57-131">Type</span></span>|<span data-ttu-id="07c57-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="07c57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07c57-133">filter</span><span class="sxs-lookup"><span data-stu-id="07c57-133">filter</span></span>|<span data-ttu-id="07c57-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07c57-134">String</span></span>|<span data-ttu-id="07c57-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07c57-135">Not yet documented</span></span>|
|<span data-ttu-id="07c57-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="07c57-136">skipToken</span></span>|<span data-ttu-id="07c57-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07c57-137">String</span></span>|<span data-ttu-id="07c57-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07c57-138">Not yet documented</span></span>|
|<span data-ttu-id="07c57-139">skip</span><span class="sxs-lookup"><span data-stu-id="07c57-139">skip</span></span>|<span data-ttu-id="07c57-140">Int32</span><span class="sxs-lookup"><span data-stu-id="07c57-140">Int32</span></span>|<span data-ttu-id="07c57-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07c57-141">Not yet documented</span></span>|
|<span data-ttu-id="07c57-142">top</span><span class="sxs-lookup"><span data-stu-id="07c57-142">top</span></span>|<span data-ttu-id="07c57-143">Int32</span><span class="sxs-lookup"><span data-stu-id="07c57-143">Int32</span></span>|<span data-ttu-id="07c57-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07c57-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="07c57-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="07c57-145">Response</span></span>
<span data-ttu-id="07c57-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07c57-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07c57-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07c57-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="07c57-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07c57-148">Request</span></span>
<span data-ttu-id="07c57-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07c57-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="07c57-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="07c57-150">Response</span></span>
<span data-ttu-id="07c57-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07c57-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



