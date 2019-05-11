---
title: função managedDeviceEnrollmentAbandonmentDetails
description: Metadados para o relatório de detalhes de abandono de registro
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 598b7941370ed729b5f3010bebe6feed0422ed80
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898238"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="f0187-103">função managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="f0187-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="f0187-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f0187-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f0187-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f0187-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0187-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0187-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0187-107">Metadados para o relatório de detalhes de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="f0187-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0187-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0187-108">Prerequisites</span></span>
<span data-ttu-id="f0187-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0187-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0187-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0187-111">Permission type</span></span>|<span data-ttu-id="f0187-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f0187-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0187-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0187-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f0187-114">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="f0187-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="f0187-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0187-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f0187-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0187-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0187-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0187-117">Not supported.</span></span>|
|<span data-ttu-id="f0187-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0187-118">Application</span></span>|<span data-ttu-id="f0187-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0187-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0187-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0187-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="f0187-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0187-121">Request headers</span></span>
|<span data-ttu-id="f0187-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0187-122">Header</span></span>|<span data-ttu-id="f0187-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f0187-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0187-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0187-124">Authorization</span></span>|<span data-ttu-id="f0187-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0187-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0187-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f0187-126">Accept</span></span>|<span data-ttu-id="f0187-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f0187-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0187-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0187-128">Request body</span></span>
<span data-ttu-id="f0187-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="f0187-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f0187-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="f0187-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f0187-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0187-131">Property</span></span>|<span data-ttu-id="f0187-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0187-132">Type</span></span>|<span data-ttu-id="f0187-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0187-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0187-134">skip</span><span class="sxs-lookup"><span data-stu-id="f0187-134">skip</span></span>|<span data-ttu-id="f0187-135">Int32</span><span class="sxs-lookup"><span data-stu-id="f0187-135">Int32</span></span>|<span data-ttu-id="f0187-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f0187-136">Not yet documented</span></span>|
|<span data-ttu-id="f0187-137">top</span><span class="sxs-lookup"><span data-stu-id="f0187-137">top</span></span>|<span data-ttu-id="f0187-138">Int32</span><span class="sxs-lookup"><span data-stu-id="f0187-138">Int32</span></span>|<span data-ttu-id="f0187-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f0187-139">Not yet documented</span></span>|
|<span data-ttu-id="f0187-140">filter</span><span class="sxs-lookup"><span data-stu-id="f0187-140">filter</span></span>|<span data-ttu-id="f0187-141">String</span><span class="sxs-lookup"><span data-stu-id="f0187-141">String</span></span>|<span data-ttu-id="f0187-142">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f0187-142">Not yet documented</span></span>|
|<span data-ttu-id="f0187-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="f0187-143">skipToken</span></span>|<span data-ttu-id="f0187-144">String</span><span class="sxs-lookup"><span data-stu-id="f0187-144">String</span></span>|<span data-ttu-id="f0187-145">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f0187-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f0187-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0187-146">Response</span></span>
<span data-ttu-id="f0187-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0187-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0187-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0187-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0187-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0187-149">Request</span></span>
<span data-ttu-id="f0187-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0187-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="f0187-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0187-151">Response</span></span>
<span data-ttu-id="f0187-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0187-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





