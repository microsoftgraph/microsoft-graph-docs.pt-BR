---
title: função getMobileAppCount
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: be043b447e3b97bc248d62f25cdce19c906e81fd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935360"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="4b0fc-103">função getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="4b0fc-103">getMobileAppCount function</span></span>

> <span data-ttu-id="4b0fc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b0fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b0fc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b0fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b0fc-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4b0fc-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b0fc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b0fc-107">Prerequisites</span></span>
<span data-ttu-id="4b0fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b0fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b0fc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b0fc-110">Permission type</span></span>|<span data-ttu-id="4b0fc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4b0fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b0fc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b0fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b0fc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b0fc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4b0fc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b0fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b0fc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b0fc-115">Not supported.</span></span>|
|<span data-ttu-id="4b0fc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b0fc-116">Application</span></span>|<span data-ttu-id="4b0fc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b0fc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b0fc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b0fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="4b0fc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b0fc-119">Request headers</span></span>
|<span data-ttu-id="4b0fc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b0fc-120">Header</span></span>|<span data-ttu-id="4b0fc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4b0fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b0fc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b0fc-122">Authorization</span></span>|<span data-ttu-id="4b0fc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b0fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b0fc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b0fc-124">Accept</span></span>|<span data-ttu-id="4b0fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b0fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b0fc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b0fc-126">Request body</span></span>
<span data-ttu-id="4b0fc-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="4b0fc-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4b0fc-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="4b0fc-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4b0fc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b0fc-129">Property</span></span>|<span data-ttu-id="4b0fc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b0fc-130">Type</span></span>|<span data-ttu-id="4b0fc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b0fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b0fc-132">status</span><span class="sxs-lookup"><span data-stu-id="4b0fc-132">status</span></span>|<span data-ttu-id="4b0fc-133">String</span><span class="sxs-lookup"><span data-stu-id="4b0fc-133">String</span></span>|<span data-ttu-id="4b0fc-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4b0fc-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4b0fc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b0fc-135">Response</span></span>
<span data-ttu-id="4b0fc-136">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um Int64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b0fc-136">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b0fc-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b0fc-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b0fc-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b0fc-138">Request</span></span>
<span data-ttu-id="4b0fc-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b0fc-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="4b0fc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b0fc-140">Response</span></span>
<span data-ttu-id="4b0fc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b0fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```




