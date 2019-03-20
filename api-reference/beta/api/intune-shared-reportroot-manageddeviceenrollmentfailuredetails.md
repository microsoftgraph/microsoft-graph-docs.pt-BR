---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0dff0f10c1bcfbed9bb79bcf6566bb6a329521b5
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572289"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="7a013-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="7a013-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="7a013-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7a013-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7a013-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7a013-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a013-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a013-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a013-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7a013-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7a013-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7a013-108">Prerequisites</span></span>
<span data-ttu-id="7a013-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7a013-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7a013-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a013-111">Permission type</span></span>|<span data-ttu-id="7a013-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7a013-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a013-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a013-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7a013-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="7a013-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="7a013-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a013-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7a013-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a013-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a013-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a013-117">Not supported.</span></span>|
|<span data-ttu-id="7a013-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a013-118">Application</span></span>|<span data-ttu-id="7a013-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a013-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a013-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a013-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="7a013-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a013-121">Request headers</span></span>
|<span data-ttu-id="7a013-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a013-122">Header</span></span>|<span data-ttu-id="7a013-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7a013-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a013-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a013-124">Authorization</span></span>|<span data-ttu-id="7a013-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a013-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a013-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7a013-126">Accept</span></span>|<span data-ttu-id="7a013-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7a013-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a013-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a013-128">Request body</span></span>
<span data-ttu-id="7a013-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="7a013-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7a013-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a013-130">Property</span></span>|<span data-ttu-id="7a013-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a013-131">Type</span></span>|<span data-ttu-id="7a013-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a013-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a013-133">filter</span><span class="sxs-lookup"><span data-stu-id="7a013-133">filter</span></span>|<span data-ttu-id="7a013-134">String</span><span class="sxs-lookup"><span data-stu-id="7a013-134">String</span></span>|<span data-ttu-id="7a013-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7a013-135">Not yet documented</span></span>|
|<span data-ttu-id="7a013-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="7a013-136">skipToken</span></span>|<span data-ttu-id="7a013-137">String</span><span class="sxs-lookup"><span data-stu-id="7a013-137">String</span></span>|<span data-ttu-id="7a013-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7a013-138">Not yet documented</span></span>|
|<span data-ttu-id="7a013-139">ignorar</span><span class="sxs-lookup"><span data-stu-id="7a013-139">skip</span></span>|<span data-ttu-id="7a013-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7a013-140">Int32</span></span>|<span data-ttu-id="7a013-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7a013-141">Not yet documented</span></span>|
|<span data-ttu-id="7a013-142">top</span><span class="sxs-lookup"><span data-stu-id="7a013-142">top</span></span>|<span data-ttu-id="7a013-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7a013-143">Int32</span></span>|<span data-ttu-id="7a013-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7a013-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7a013-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a013-145">Response</span></span>
<span data-ttu-id="7a013-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a013-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a013-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a013-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="7a013-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a013-148">Request</span></span>
<span data-ttu-id="7a013-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a013-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7a013-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a013-150">Response</span></span>
<span data-ttu-id="7a013-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a013-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



