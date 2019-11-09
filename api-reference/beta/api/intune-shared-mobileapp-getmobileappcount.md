---
title: função getMobileAppCount
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a707c6a1b131bdffe548475322124cf519ff66da
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085791"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="ed06b-103">função getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="ed06b-103">getMobileAppCount function</span></span>

> <span data-ttu-id="ed06b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed06b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed06b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed06b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed06b-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ed06b-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed06b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed06b-107">Prerequisites</span></span>
<span data-ttu-id="ed06b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed06b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed06b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed06b-110">Permission type</span></span>|<span data-ttu-id="ed06b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed06b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed06b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed06b-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ed06b-113">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="ed06b-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="ed06b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed06b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ed06b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed06b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed06b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed06b-116">Not supported.</span></span>|
|<span data-ttu-id="ed06b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed06b-117">Application</span></span>||
| <span data-ttu-id="ed06b-118">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="ed06b-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="ed06b-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed06b-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed06b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed06b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="ed06b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed06b-121">Request headers</span></span>
|<span data-ttu-id="ed06b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed06b-122">Header</span></span>|<span data-ttu-id="ed06b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ed06b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed06b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed06b-124">Authorization</span></span>|<span data-ttu-id="ed06b-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed06b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed06b-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed06b-126">Accept</span></span>|<span data-ttu-id="ed06b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ed06b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed06b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed06b-128">Request body</span></span>
<span data-ttu-id="ed06b-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="ed06b-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ed06b-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="ed06b-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ed06b-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed06b-131">Property</span></span>|<span data-ttu-id="ed06b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed06b-132">Type</span></span>|<span data-ttu-id="ed06b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed06b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed06b-134">status</span><span class="sxs-lookup"><span data-stu-id="ed06b-134">status</span></span>|<span data-ttu-id="ed06b-135">String</span><span class="sxs-lookup"><span data-stu-id="ed06b-135">String</span></span>|<span data-ttu-id="ed06b-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ed06b-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ed06b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed06b-137">Response</span></span>
<span data-ttu-id="ed06b-138">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um Int64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed06b-138">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed06b-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed06b-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed06b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed06b-140">Request</span></span>
<span data-ttu-id="ed06b-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed06b-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ed06b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed06b-142">Response</span></span>
<span data-ttu-id="ed06b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed06b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```









