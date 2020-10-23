---
title: função getMobileAppCount
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f8cb917403ecb942d385506b5a382f8f23fe3fc3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729872"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="bef28-103">função getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="bef28-103">getMobileAppCount function</span></span>

<span data-ttu-id="bef28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bef28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bef28-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bef28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bef28-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bef28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bef28-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bef28-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bef28-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bef28-108">Prerequisites</span></span>
<span data-ttu-id="bef28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bef28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bef28-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bef28-111">Permission type</span></span>|<span data-ttu-id="bef28-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bef28-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bef28-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bef28-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bef28-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="bef28-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="bef28-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bef28-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bef28-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bef28-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bef28-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bef28-117">Not supported.</span></span>|
|<span data-ttu-id="bef28-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bef28-118">Application</span></span>||
| <span data-ttu-id="bef28-119">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="bef28-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="bef28-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bef28-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bef28-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bef28-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="bef28-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bef28-122">Request headers</span></span>
|<span data-ttu-id="bef28-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bef28-123">Header</span></span>|<span data-ttu-id="bef28-124">Valor</span><span class="sxs-lookup"><span data-stu-id="bef28-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bef28-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="bef28-125">Authorization</span></span>|<span data-ttu-id="bef28-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bef28-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bef28-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bef28-127">Accept</span></span>|<span data-ttu-id="bef28-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bef28-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bef28-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bef28-129">Request body</span></span>
<span data-ttu-id="bef28-130">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="bef28-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="bef28-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="bef28-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="bef28-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bef28-132">Property</span></span>|<span data-ttu-id="bef28-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="bef28-133">Type</span></span>|<span data-ttu-id="bef28-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="bef28-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bef28-135">status</span><span class="sxs-lookup"><span data-stu-id="bef28-135">status</span></span>|<span data-ttu-id="bef28-136">String</span><span class="sxs-lookup"><span data-stu-id="bef28-136">String</span></span>|<span data-ttu-id="bef28-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bef28-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bef28-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bef28-138">Response</span></span>
<span data-ttu-id="bef28-139">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um Int64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bef28-139">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bef28-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bef28-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="bef28-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bef28-141">Request</span></span>
<span data-ttu-id="bef28-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bef28-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="bef28-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="bef28-143">Response</span></span>
<span data-ttu-id="bef28-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bef28-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```








