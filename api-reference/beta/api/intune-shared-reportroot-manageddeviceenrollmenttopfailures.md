---
title: função managedDeviceEnrollmentTopFailures
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 163a75a2ffa675f939086fecf3e9c4a155352aa1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934223"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="53299-103">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="53299-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="53299-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="53299-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53299-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="53299-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53299-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="53299-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53299-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="53299-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53299-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53299-108">Prerequisites</span></span>
<span data-ttu-id="53299-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53299-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53299-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53299-111">Permission type</span></span>|<span data-ttu-id="53299-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="53299-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53299-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53299-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="53299-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="53299-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="53299-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53299-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="53299-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53299-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53299-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53299-117">Not supported.</span></span>|
|<span data-ttu-id="53299-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53299-118">Application</span></span>|<span data-ttu-id="53299-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53299-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53299-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53299-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="53299-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53299-121">Request headers</span></span>
|<span data-ttu-id="53299-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53299-122">Header</span></span>|<span data-ttu-id="53299-123">Valor</span><span class="sxs-lookup"><span data-stu-id="53299-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53299-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="53299-124">Authorization</span></span>|<span data-ttu-id="53299-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53299-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53299-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53299-126">Accept</span></span>|<span data-ttu-id="53299-127">application/json</span><span class="sxs-lookup"><span data-stu-id="53299-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53299-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53299-128">Request body</span></span>
<span data-ttu-id="53299-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="53299-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="53299-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="53299-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="53299-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53299-131">Property</span></span>|<span data-ttu-id="53299-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="53299-132">Type</span></span>|<span data-ttu-id="53299-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="53299-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53299-134">ponto</span><span class="sxs-lookup"><span data-stu-id="53299-134">period</span></span>|<span data-ttu-id="53299-135">String</span><span class="sxs-lookup"><span data-stu-id="53299-135">String</span></span>|<span data-ttu-id="53299-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="53299-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="53299-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="53299-137">Response</span></span>
<span data-ttu-id="53299-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53299-138">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53299-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53299-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="53299-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53299-140">Request</span></span>
<span data-ttu-id="53299-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53299-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="53299-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="53299-142">Response</span></span>
<span data-ttu-id="53299-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53299-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



