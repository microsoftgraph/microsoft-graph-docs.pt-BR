---
title: função managedDeviceEnrollmentAbandonmentDetails
description: Metadados para o relatório de detalhes de abandono de registro
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08c80c18718109a58498b57a58ad1396cd75024b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694190"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="fcd13-103">função managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="fcd13-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

<span data-ttu-id="fcd13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcd13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcd13-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fcd13-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fcd13-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fcd13-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fcd13-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fcd13-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcd13-108">Metadados para o relatório de detalhes de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="fcd13-108">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fcd13-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fcd13-109">Prerequisites</span></span>
<span data-ttu-id="fcd13-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcd13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcd13-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcd13-112">Permission type</span></span>|<span data-ttu-id="fcd13-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fcd13-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcd13-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcd13-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fcd13-115">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="fcd13-115">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="fcd13-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd13-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fcd13-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcd13-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcd13-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcd13-118">Not supported.</span></span>|
|<span data-ttu-id="fcd13-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcd13-119">Application</span></span>||
| <span data-ttu-id="fcd13-120">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="fcd13-120">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="fcd13-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd13-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcd13-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcd13-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="fcd13-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcd13-123">Request headers</span></span>
|<span data-ttu-id="fcd13-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fcd13-124">Header</span></span>|<span data-ttu-id="fcd13-125">Valor</span><span class="sxs-lookup"><span data-stu-id="fcd13-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcd13-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcd13-126">Authorization</span></span>|<span data-ttu-id="fcd13-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcd13-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcd13-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fcd13-128">Accept</span></span>|<span data-ttu-id="fcd13-129">application/json</span><span class="sxs-lookup"><span data-stu-id="fcd13-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcd13-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcd13-130">Request body</span></span>
<span data-ttu-id="fcd13-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="fcd13-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="fcd13-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="fcd13-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="fcd13-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fcd13-133">Property</span></span>|<span data-ttu-id="fcd13-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcd13-134">Type</span></span>|<span data-ttu-id="fcd13-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcd13-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcd13-136">skip</span><span class="sxs-lookup"><span data-stu-id="fcd13-136">skip</span></span>|<span data-ttu-id="fcd13-137">Int32</span><span class="sxs-lookup"><span data-stu-id="fcd13-137">Int32</span></span>|<span data-ttu-id="fcd13-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fcd13-138">Not yet documented</span></span>|
|<span data-ttu-id="fcd13-139">top</span><span class="sxs-lookup"><span data-stu-id="fcd13-139">top</span></span>|<span data-ttu-id="fcd13-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fcd13-140">Int32</span></span>|<span data-ttu-id="fcd13-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fcd13-141">Not yet documented</span></span>|
|<span data-ttu-id="fcd13-142">filter</span><span class="sxs-lookup"><span data-stu-id="fcd13-142">filter</span></span>|<span data-ttu-id="fcd13-143">String</span><span class="sxs-lookup"><span data-stu-id="fcd13-143">String</span></span>|<span data-ttu-id="fcd13-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fcd13-144">Not yet documented</span></span>|
|<span data-ttu-id="fcd13-145">skipToken</span><span class="sxs-lookup"><span data-stu-id="fcd13-145">skipToken</span></span>|<span data-ttu-id="fcd13-146">String</span><span class="sxs-lookup"><span data-stu-id="fcd13-146">String</span></span>|<span data-ttu-id="fcd13-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fcd13-147">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fcd13-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcd13-148">Response</span></span>
<span data-ttu-id="fcd13-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fcd13-149">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcd13-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fcd13-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="fcd13-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcd13-151">Request</span></span>
<span data-ttu-id="fcd13-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcd13-152">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="fcd13-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcd13-153">Response</span></span>
<span data-ttu-id="fcd13-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fcd13-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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













