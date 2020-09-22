---
title: função getMobileAppCount
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4c032c3dd8017aca170e77709e5526e6c0c8a4ab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074318"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="f232d-103">função getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="f232d-103">getMobileAppCount function</span></span>

<span data-ttu-id="f232d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f232d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f232d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f232d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f232d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f232d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f232d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f232d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f232d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f232d-108">Prerequisites</span></span>
<span data-ttu-id="f232d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f232d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f232d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f232d-111">Permission type</span></span>|<span data-ttu-id="f232d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f232d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f232d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f232d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f232d-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="f232d-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="f232d-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f232d-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f232d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f232d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f232d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f232d-117">Not supported.</span></span>|
|<span data-ttu-id="f232d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f232d-118">Application</span></span>||
| <span data-ttu-id="f232d-119">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="f232d-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="f232d-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f232d-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f232d-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f232d-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="f232d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f232d-122">Request headers</span></span>
|<span data-ttu-id="f232d-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f232d-123">Header</span></span>|<span data-ttu-id="f232d-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f232d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f232d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f232d-125">Authorization</span></span>|<span data-ttu-id="f232d-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f232d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f232d-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f232d-127">Accept</span></span>|<span data-ttu-id="f232d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f232d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f232d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f232d-129">Request body</span></span>
<span data-ttu-id="f232d-130">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="f232d-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f232d-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="f232d-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f232d-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f232d-132">Property</span></span>|<span data-ttu-id="f232d-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="f232d-133">Type</span></span>|<span data-ttu-id="f232d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f232d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f232d-135">status</span><span class="sxs-lookup"><span data-stu-id="f232d-135">status</span></span>|<span data-ttu-id="f232d-136">String</span><span class="sxs-lookup"><span data-stu-id="f232d-136">String</span></span>|<span data-ttu-id="f232d-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f232d-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f232d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f232d-138">Response</span></span>
<span data-ttu-id="f232d-139">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um Int64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f232d-139">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f232d-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f232d-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f232d-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f232d-141">Request</span></span>
<span data-ttu-id="f232d-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f232d-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="f232d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f232d-143">Response</span></span>
<span data-ttu-id="f232d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f232d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```









