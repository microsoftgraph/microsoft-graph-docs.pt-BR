---
title: função managedDeviceEnrollmentAbandonmentSummary
description: Metadados para o relatório de Resumo de abandono de registro
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0bd8e82aa7987e89d9f9a740a8fa9c181570ccd8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30956657"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="15c86-103">função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="15c86-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

> <span data-ttu-id="15c86-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="15c86-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15c86-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="15c86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15c86-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15c86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15c86-107">Metadados para o relatório de Resumo de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="15c86-107">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="15c86-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15c86-108">Prerequisites</span></span>
<span data-ttu-id="15c86-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15c86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15c86-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15c86-111">Permission type</span></span>|<span data-ttu-id="15c86-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15c86-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15c86-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15c86-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="15c86-114">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="15c86-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="15c86-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="15c86-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="15c86-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15c86-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15c86-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15c86-117">Not supported.</span></span>|
|<span data-ttu-id="15c86-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15c86-118">Application</span></span>|<span data-ttu-id="15c86-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15c86-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15c86-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15c86-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="15c86-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15c86-121">Request headers</span></span>
|<span data-ttu-id="15c86-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15c86-122">Header</span></span>|<span data-ttu-id="15c86-123">Valor</span><span class="sxs-lookup"><span data-stu-id="15c86-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15c86-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="15c86-124">Authorization</span></span>|<span data-ttu-id="15c86-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15c86-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15c86-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15c86-126">Accept</span></span>|<span data-ttu-id="15c86-127">application/json</span><span class="sxs-lookup"><span data-stu-id="15c86-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15c86-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15c86-128">Request body</span></span>
<span data-ttu-id="15c86-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="15c86-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="15c86-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="15c86-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="15c86-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15c86-131">Property</span></span>|<span data-ttu-id="15c86-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="15c86-132">Type</span></span>|<span data-ttu-id="15c86-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="15c86-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15c86-134">ignorar</span><span class="sxs-lookup"><span data-stu-id="15c86-134">skip</span></span>|<span data-ttu-id="15c86-135">Int32</span><span class="sxs-lookup"><span data-stu-id="15c86-135">Int32</span></span>|<span data-ttu-id="15c86-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="15c86-136">Not yet documented</span></span>|
|<span data-ttu-id="15c86-137">top</span><span class="sxs-lookup"><span data-stu-id="15c86-137">top</span></span>|<span data-ttu-id="15c86-138">Int32</span><span class="sxs-lookup"><span data-stu-id="15c86-138">Int32</span></span>|<span data-ttu-id="15c86-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="15c86-139">Not yet documented</span></span>|
|<span data-ttu-id="15c86-140">filter</span><span class="sxs-lookup"><span data-stu-id="15c86-140">filter</span></span>|<span data-ttu-id="15c86-141">String</span><span class="sxs-lookup"><span data-stu-id="15c86-141">String</span></span>|<span data-ttu-id="15c86-142">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="15c86-142">Not yet documented</span></span>|
|<span data-ttu-id="15c86-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="15c86-143">skipToken</span></span>|<span data-ttu-id="15c86-144">String</span><span class="sxs-lookup"><span data-stu-id="15c86-144">String</span></span>|<span data-ttu-id="15c86-145">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="15c86-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="15c86-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="15c86-146">Response</span></span>
<span data-ttu-id="15c86-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15c86-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15c86-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15c86-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="15c86-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15c86-149">Request</span></span>
<span data-ttu-id="15c86-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15c86-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="15c86-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="15c86-151">Response</span></span>
<span data-ttu-id="15c86-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15c86-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





