---
title: função scopedForResource
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0745ef277ad852ef061ea0f4f352cf07e808604
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002263"
---
# <a name="scopedforresource-function"></a><span data-ttu-id="2ba67-103">função scopedForResource</span><span class="sxs-lookup"><span data-stu-id="2ba67-103">scopedForResource function</span></span>

> <span data-ttu-id="2ba67-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ba67-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ba67-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ba67-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ba67-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2ba67-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ba67-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ba67-107">Prerequisites</span></span>
<span data-ttu-id="2ba67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ba67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ba67-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ba67-110">Permission type</span></span>|<span data-ttu-id="2ba67-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ba67-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ba67-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ba67-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ba67-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ba67-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="2ba67-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ba67-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ba67-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ba67-115">Not supported.</span></span>|
|<span data-ttu-id="2ba67-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ba67-116">Application</span></span>|<span data-ttu-id="2ba67-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ba67-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ba67-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ba67-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/scopedForResource
```

## <a name="request-headers"></a><span data-ttu-id="2ba67-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ba67-119">Request headers</span></span>
|<span data-ttu-id="2ba67-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ba67-120">Header</span></span>|<span data-ttu-id="2ba67-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2ba67-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ba67-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ba67-122">Authorization</span></span>|<span data-ttu-id="2ba67-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ba67-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ba67-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ba67-124">Accept</span></span>|<span data-ttu-id="2ba67-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ba67-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ba67-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ba67-126">Request body</span></span>
<span data-ttu-id="2ba67-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="2ba67-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2ba67-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="2ba67-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2ba67-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ba67-129">Property</span></span>|<span data-ttu-id="2ba67-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ba67-130">Type</span></span>|<span data-ttu-id="2ba67-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ba67-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ba67-132">recurso</span><span class="sxs-lookup"><span data-stu-id="2ba67-132">resource</span></span>|<span data-ttu-id="2ba67-133">String</span><span class="sxs-lookup"><span data-stu-id="2ba67-133">String</span></span>|<span data-ttu-id="2ba67-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2ba67-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2ba67-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ba67-135">Response</span></span>
<span data-ttu-id="2ba67-136">Se tiver êxito, essa função retornará o código resposta `200 OK` e um Booliano no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ba67-136">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ba67-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ba67-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ba67-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ba67-138">Request</span></span>
<span data-ttu-id="2ba67-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ba67-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/scopedForResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="2ba67-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ba67-140">Response</span></span>
<span data-ttu-id="2ba67-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ba67-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```





