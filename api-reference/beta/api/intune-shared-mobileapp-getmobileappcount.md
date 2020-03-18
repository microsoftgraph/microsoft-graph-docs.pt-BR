---
title: função getMobileAppCount
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6c0c0e78046ad9c9ff2833adf6b68c97ca8508d9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800792"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="4e239-103">função getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="4e239-103">getMobileAppCount function</span></span>

> <span data-ttu-id="4e239-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e239-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e239-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e239-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e239-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e239-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e239-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4e239-107">Prerequisites</span></span>
<span data-ttu-id="4e239-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e239-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e239-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e239-110">Permission type</span></span>|<span data-ttu-id="4e239-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e239-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e239-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e239-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4e239-113">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="4e239-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="4e239-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e239-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4e239-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e239-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e239-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e239-116">Not supported.</span></span>|
|<span data-ttu-id="4e239-117">Application</span><span class="sxs-lookup"><span data-stu-id="4e239-117">Application</span></span>||
| <span data-ttu-id="4e239-118">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="4e239-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="4e239-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e239-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e239-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e239-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="4e239-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e239-121">Request headers</span></span>
|<span data-ttu-id="4e239-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e239-122">Header</span></span>|<span data-ttu-id="4e239-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4e239-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e239-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e239-124">Authorization</span></span>|<span data-ttu-id="4e239-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e239-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e239-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4e239-126">Accept</span></span>|<span data-ttu-id="4e239-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4e239-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e239-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e239-128">Request body</span></span>
<span data-ttu-id="4e239-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="4e239-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4e239-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="4e239-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4e239-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e239-131">Property</span></span>|<span data-ttu-id="4e239-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e239-132">Type</span></span>|<span data-ttu-id="4e239-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e239-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e239-134">status</span><span class="sxs-lookup"><span data-stu-id="4e239-134">status</span></span>|<span data-ttu-id="4e239-135">String</span><span class="sxs-lookup"><span data-stu-id="4e239-135">String</span></span>|<span data-ttu-id="4e239-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e239-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4e239-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e239-137">Response</span></span>
<span data-ttu-id="4e239-138">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um Int64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e239-138">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e239-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e239-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e239-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e239-140">Request</span></span>
<span data-ttu-id="4e239-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e239-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="4e239-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e239-142">Response</span></span>
<span data-ttu-id="4e239-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e239-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```







