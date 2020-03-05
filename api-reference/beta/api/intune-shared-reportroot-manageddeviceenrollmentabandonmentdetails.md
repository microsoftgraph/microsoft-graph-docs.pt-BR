---
title: função managedDeviceEnrollmentAbandonmentDetails
description: Metadados para o relatório de detalhes de abandono de registro
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ae34f9a85624d8e08d2529ec881338aef212aa39
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458179"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="c63c0-103">função managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="c63c0-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

<span data-ttu-id="c63c0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c63c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c63c0-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c63c0-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c63c0-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c63c0-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c63c0-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c63c0-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c63c0-108">Metadados para o relatório de detalhes de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="c63c0-108">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c63c0-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c63c0-109">Prerequisites</span></span>
<span data-ttu-id="c63c0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c63c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c63c0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c63c0-112">Permission type</span></span>|<span data-ttu-id="c63c0-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c63c0-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c63c0-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c63c0-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c63c0-115">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="c63c0-115">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="c63c0-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c63c0-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c63c0-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c63c0-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c63c0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c63c0-118">Not supported.</span></span>|
|<span data-ttu-id="c63c0-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c63c0-119">Application</span></span>||
| <span data-ttu-id="c63c0-120">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="c63c0-120">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="c63c0-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c63c0-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c63c0-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c63c0-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="c63c0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c63c0-123">Request headers</span></span>
|<span data-ttu-id="c63c0-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c63c0-124">Header</span></span>|<span data-ttu-id="c63c0-125">Valor</span><span class="sxs-lookup"><span data-stu-id="c63c0-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c63c0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c63c0-126">Authorization</span></span>|<span data-ttu-id="c63c0-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c63c0-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c63c0-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c63c0-128">Accept</span></span>|<span data-ttu-id="c63c0-129">application/json</span><span class="sxs-lookup"><span data-stu-id="c63c0-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c63c0-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c63c0-130">Request body</span></span>
<span data-ttu-id="c63c0-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="c63c0-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="c63c0-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="c63c0-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="c63c0-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c63c0-133">Property</span></span>|<span data-ttu-id="c63c0-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="c63c0-134">Type</span></span>|<span data-ttu-id="c63c0-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="c63c0-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c63c0-136">skip</span><span class="sxs-lookup"><span data-stu-id="c63c0-136">skip</span></span>|<span data-ttu-id="c63c0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c63c0-137">Int32</span></span>|<span data-ttu-id="c63c0-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c63c0-138">Not yet documented</span></span>|
|<span data-ttu-id="c63c0-139">top</span><span class="sxs-lookup"><span data-stu-id="c63c0-139">top</span></span>|<span data-ttu-id="c63c0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c63c0-140">Int32</span></span>|<span data-ttu-id="c63c0-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c63c0-141">Not yet documented</span></span>|
|<span data-ttu-id="c63c0-142">filter</span><span class="sxs-lookup"><span data-stu-id="c63c0-142">filter</span></span>|<span data-ttu-id="c63c0-143">String</span><span class="sxs-lookup"><span data-stu-id="c63c0-143">String</span></span>|<span data-ttu-id="c63c0-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c63c0-144">Not yet documented</span></span>|
|<span data-ttu-id="c63c0-145">skipToken</span><span class="sxs-lookup"><span data-stu-id="c63c0-145">skipToken</span></span>|<span data-ttu-id="c63c0-146">String</span><span class="sxs-lookup"><span data-stu-id="c63c0-146">String</span></span>|<span data-ttu-id="c63c0-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c63c0-147">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c63c0-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c63c0-148">Response</span></span>
<span data-ttu-id="c63c0-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c63c0-149">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c63c0-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c63c0-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="c63c0-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c63c0-151">Request</span></span>
<span data-ttu-id="c63c0-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c63c0-152">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="c63c0-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c63c0-153">Response</span></span>
<span data-ttu-id="c63c0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c63c0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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













