---
title: função getMobileAppCount
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b65496109dcfcf9a259e4274e3bca636da12b218
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538004"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="d55ce-103">função getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="d55ce-103">getMobileAppCount function</span></span>

> <span data-ttu-id="d55ce-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d55ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d55ce-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d55ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d55ce-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d55ce-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d55ce-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d55ce-107">Prerequisites</span></span>
<span data-ttu-id="d55ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d55ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d55ce-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d55ce-110">Permission type</span></span>|<span data-ttu-id="d55ce-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d55ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d55ce-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d55ce-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d55ce-113">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="d55ce-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d55ce-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d55ce-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d55ce-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d55ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d55ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d55ce-116">Not supported.</span></span>|
|<span data-ttu-id="d55ce-117">Application</span><span class="sxs-lookup"><span data-stu-id="d55ce-117">Application</span></span>||
| <span data-ttu-id="d55ce-118">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="d55ce-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d55ce-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d55ce-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d55ce-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d55ce-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="d55ce-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d55ce-121">Request headers</span></span>
|<span data-ttu-id="d55ce-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d55ce-122">Header</span></span>|<span data-ttu-id="d55ce-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d55ce-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d55ce-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d55ce-124">Authorization</span></span>|<span data-ttu-id="d55ce-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d55ce-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d55ce-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d55ce-126">Accept</span></span>|<span data-ttu-id="d55ce-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d55ce-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d55ce-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d55ce-128">Request body</span></span>
<span data-ttu-id="d55ce-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="d55ce-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d55ce-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="d55ce-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d55ce-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d55ce-131">Property</span></span>|<span data-ttu-id="d55ce-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d55ce-132">Type</span></span>|<span data-ttu-id="d55ce-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d55ce-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d55ce-134">status</span><span class="sxs-lookup"><span data-stu-id="d55ce-134">status</span></span>|<span data-ttu-id="d55ce-135">String</span><span class="sxs-lookup"><span data-stu-id="d55ce-135">String</span></span>|<span data-ttu-id="d55ce-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d55ce-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d55ce-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d55ce-137">Response</span></span>
<span data-ttu-id="d55ce-138">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um Int64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d55ce-138">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d55ce-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d55ce-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="d55ce-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d55ce-140">Request</span></span>
<span data-ttu-id="d55ce-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d55ce-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d55ce-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d55ce-142">Response</span></span>
<span data-ttu-id="d55ce-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d55ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```






