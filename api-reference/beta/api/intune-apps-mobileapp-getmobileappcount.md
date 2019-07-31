---
title: função getMobileAppCount
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ff1b796bfc9b026ddf6866cc054dd8ab0014cca7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961102"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="e1973-103">função getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="e1973-103">getMobileAppCount function</span></span>

> <span data-ttu-id="e1973-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1973-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1973-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1973-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1973-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e1973-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1973-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1973-107">Prerequisites</span></span>
<span data-ttu-id="e1973-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1973-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1973-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1973-110">Permission type</span></span>|<span data-ttu-id="e1973-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1973-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1973-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1973-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1973-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1973-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e1973-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1973-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1973-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1973-115">Not supported.</span></span>|
|<span data-ttu-id="e1973-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1973-116">Application</span></span>|<span data-ttu-id="e1973-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1973-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1973-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1973-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="e1973-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1973-119">Request headers</span></span>
|<span data-ttu-id="e1973-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1973-120">Header</span></span>|<span data-ttu-id="e1973-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e1973-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1973-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1973-122">Authorization</span></span>|<span data-ttu-id="e1973-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1973-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1973-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1973-124">Accept</span></span>|<span data-ttu-id="e1973-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e1973-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1973-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1973-126">Request body</span></span>
<span data-ttu-id="e1973-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="e1973-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e1973-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="e1973-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e1973-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1973-129">Property</span></span>|<span data-ttu-id="e1973-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1973-130">Type</span></span>|<span data-ttu-id="e1973-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1973-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1973-132">status</span><span class="sxs-lookup"><span data-stu-id="e1973-132">status</span></span>|<span data-ttu-id="e1973-133">String</span><span class="sxs-lookup"><span data-stu-id="e1973-133">String</span></span>|<span data-ttu-id="e1973-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e1973-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e1973-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1973-135">Response</span></span>
<span data-ttu-id="e1973-136">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um Int64 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1973-136">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1973-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1973-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1973-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1973-138">Request</span></span>
<span data-ttu-id="e1973-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1973-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e1973-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1973-140">Response</span></span>
<span data-ttu-id="e1973-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1973-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```





