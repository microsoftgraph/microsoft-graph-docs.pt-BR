---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e861b8947396c67c72ba47493d30e6010905b107
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526920"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="a1d84-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="a1d84-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="a1d84-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a1d84-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a1d84-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a1d84-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1d84-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1d84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1d84-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1d84-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1d84-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1d84-108">Prerequisites</span></span>
<span data-ttu-id="a1d84-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1d84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1d84-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1d84-111">Permission type</span></span>|<span data-ttu-id="a1d84-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1d84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1d84-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1d84-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a1d84-114">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="a1d84-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a1d84-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1d84-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a1d84-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1d84-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1d84-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1d84-117">Not supported.</span></span>|
|<span data-ttu-id="a1d84-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1d84-118">Application</span></span>|<span data-ttu-id="a1d84-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1d84-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1d84-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1d84-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="a1d84-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d84-121">Request headers</span></span>
|<span data-ttu-id="a1d84-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1d84-122">Header</span></span>|<span data-ttu-id="a1d84-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a1d84-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1d84-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1d84-124">Authorization</span></span>|<span data-ttu-id="a1d84-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1d84-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1d84-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1d84-126">Accept</span></span>|<span data-ttu-id="a1d84-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a1d84-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1d84-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d84-128">Request body</span></span>
<span data-ttu-id="a1d84-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="a1d84-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a1d84-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1d84-130">Property</span></span>|<span data-ttu-id="a1d84-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1d84-131">Type</span></span>|<span data-ttu-id="a1d84-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1d84-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1d84-133">filter</span><span class="sxs-lookup"><span data-stu-id="a1d84-133">filter</span></span>|<span data-ttu-id="a1d84-134">String</span><span class="sxs-lookup"><span data-stu-id="a1d84-134">String</span></span>|<span data-ttu-id="a1d84-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1d84-135">Not yet documented</span></span>|
|<span data-ttu-id="a1d84-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="a1d84-136">skipToken</span></span>|<span data-ttu-id="a1d84-137">String</span><span class="sxs-lookup"><span data-stu-id="a1d84-137">String</span></span>|<span data-ttu-id="a1d84-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1d84-138">Not yet documented</span></span>|
|<span data-ttu-id="a1d84-139">skip</span><span class="sxs-lookup"><span data-stu-id="a1d84-139">skip</span></span>|<span data-ttu-id="a1d84-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a1d84-140">Int32</span></span>|<span data-ttu-id="a1d84-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1d84-141">Not yet documented</span></span>|
|<span data-ttu-id="a1d84-142">top</span><span class="sxs-lookup"><span data-stu-id="a1d84-142">top</span></span>|<span data-ttu-id="a1d84-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a1d84-143">Int32</span></span>|<span data-ttu-id="a1d84-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a1d84-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a1d84-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1d84-145">Response</span></span>
<span data-ttu-id="a1d84-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1d84-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1d84-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1d84-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1d84-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d84-148">Request</span></span>
<span data-ttu-id="a1d84-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1d84-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a1d84-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1d84-150">Response</span></span>
<span data-ttu-id="a1d84-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1d84-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



