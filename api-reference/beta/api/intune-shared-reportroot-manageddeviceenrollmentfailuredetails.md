---
title: Função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08d9664ac74cd26018380844eebceabe42bb1154
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866990"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="e7e09-103">Função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="e7e09-103">managedDeviceEnrollmentFailureDetails function</span></span>

<span data-ttu-id="e7e09-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7e09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7e09-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e7e09-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e7e09-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e7e09-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7e09-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7e09-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7e09-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e7e09-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7e09-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7e09-109">Prerequisites</span></span>
<span data-ttu-id="e7e09-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7e09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7e09-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7e09-112">Permission type</span></span>|<span data-ttu-id="e7e09-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7e09-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7e09-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7e09-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e7e09-115">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="e7e09-115">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e7e09-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7e09-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e7e09-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7e09-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7e09-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7e09-118">Not supported.</span></span>|
|<span data-ttu-id="e7e09-119">Application</span><span class="sxs-lookup"><span data-stu-id="e7e09-119">Application</span></span>||
| <span data-ttu-id="e7e09-120">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="e7e09-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e7e09-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7e09-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7e09-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7e09-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="e7e09-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7e09-123">Request headers</span></span>
|<span data-ttu-id="e7e09-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7e09-124">Header</span></span>|<span data-ttu-id="e7e09-125">Valor</span><span class="sxs-lookup"><span data-stu-id="e7e09-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7e09-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7e09-126">Authorization</span></span>|<span data-ttu-id="e7e09-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7e09-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7e09-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7e09-128">Accept</span></span>|<span data-ttu-id="e7e09-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e7e09-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7e09-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7e09-130">Request body</span></span>
<span data-ttu-id="e7e09-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="e7e09-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e7e09-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7e09-132">Property</span></span>|<span data-ttu-id="e7e09-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7e09-133">Type</span></span>|<span data-ttu-id="e7e09-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7e09-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7e09-135">filter</span><span class="sxs-lookup"><span data-stu-id="e7e09-135">filter</span></span>|<span data-ttu-id="e7e09-136">String</span><span class="sxs-lookup"><span data-stu-id="e7e09-136">String</span></span>|<span data-ttu-id="e7e09-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e7e09-137">Not yet documented</span></span>|
|<span data-ttu-id="e7e09-138">skipToken</span><span class="sxs-lookup"><span data-stu-id="e7e09-138">skipToken</span></span>|<span data-ttu-id="e7e09-139">String</span><span class="sxs-lookup"><span data-stu-id="e7e09-139">String</span></span>|<span data-ttu-id="e7e09-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e7e09-140">Not yet documented</span></span>|
|<span data-ttu-id="e7e09-141">skip</span><span class="sxs-lookup"><span data-stu-id="e7e09-141">skip</span></span>|<span data-ttu-id="e7e09-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e7e09-142">Int32</span></span>|<span data-ttu-id="e7e09-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e7e09-143">Not yet documented</span></span>|
|<span data-ttu-id="e7e09-144">top</span><span class="sxs-lookup"><span data-stu-id="e7e09-144">top</span></span>|<span data-ttu-id="e7e09-145">Int32</span><span class="sxs-lookup"><span data-stu-id="e7e09-145">Int32</span></span>|<span data-ttu-id="e7e09-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e7e09-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e7e09-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7e09-147">Response</span></span>
<span data-ttu-id="e7e09-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7e09-148">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7e09-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7e09-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7e09-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7e09-150">Request</span></span>
<span data-ttu-id="e7e09-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7e09-151">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e7e09-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7e09-152">Response</span></span>
<span data-ttu-id="e7e09-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7e09-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










