---
title: função managedDeviceEnrollmentTopFailures
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6ffdc19ffdd09cf99b29f605612f772721d5492f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729002"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="c01b8-103">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="c01b8-103">managedDeviceEnrollmentTopFailures function</span></span>

<span data-ttu-id="c01b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c01b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c01b8-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c01b8-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c01b8-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c01b8-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c01b8-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c01b8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c01b8-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c01b8-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c01b8-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c01b8-109">Prerequisites</span></span>
<span data-ttu-id="c01b8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c01b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c01b8-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c01b8-112">Permission type</span></span>|<span data-ttu-id="c01b8-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c01b8-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c01b8-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c01b8-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c01b8-115">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="c01b8-115">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c01b8-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c01b8-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c01b8-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c01b8-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c01b8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c01b8-118">Not supported.</span></span>|
|<span data-ttu-id="c01b8-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c01b8-119">Application</span></span>||
| <span data-ttu-id="c01b8-120">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="c01b8-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c01b8-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c01b8-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c01b8-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c01b8-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="c01b8-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c01b8-123">Request headers</span></span>
|<span data-ttu-id="c01b8-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c01b8-124">Header</span></span>|<span data-ttu-id="c01b8-125">Valor</span><span class="sxs-lookup"><span data-stu-id="c01b8-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c01b8-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c01b8-126">Authorization</span></span>|<span data-ttu-id="c01b8-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c01b8-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c01b8-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c01b8-128">Accept</span></span>|<span data-ttu-id="c01b8-129">application/json</span><span class="sxs-lookup"><span data-stu-id="c01b8-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c01b8-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c01b8-130">Request body</span></span>
<span data-ttu-id="c01b8-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="c01b8-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="c01b8-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="c01b8-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="c01b8-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c01b8-133">Property</span></span>|<span data-ttu-id="c01b8-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="c01b8-134">Type</span></span>|<span data-ttu-id="c01b8-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="c01b8-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c01b8-136">ponto</span><span class="sxs-lookup"><span data-stu-id="c01b8-136">period</span></span>|<span data-ttu-id="c01b8-137">String</span><span class="sxs-lookup"><span data-stu-id="c01b8-137">String</span></span>|<span data-ttu-id="c01b8-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c01b8-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c01b8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c01b8-139">Response</span></span>
<span data-ttu-id="c01b8-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c01b8-140">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c01b8-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c01b8-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="c01b8-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c01b8-142">Request</span></span>
<span data-ttu-id="c01b8-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c01b8-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="c01b8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c01b8-144">Response</span></span>
<span data-ttu-id="c01b8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c01b8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











