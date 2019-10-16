---
title: função getExpiringVppTokenCount
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aa32e0a09c038cead24c5c988a7cc33f464757fb
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535951"
---
# <a name="getexpiringvpptokencount-function"></a><span data-ttu-id="0cdab-103">função getExpiringVppTokenCount</span><span class="sxs-lookup"><span data-stu-id="0cdab-103">getExpiringVppTokenCount function</span></span>

> <span data-ttu-id="0cdab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0cdab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cdab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0cdab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cdab-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0cdab-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cdab-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0cdab-107">Prerequisites</span></span>
<span data-ttu-id="0cdab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cdab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cdab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cdab-110">Permission type</span></span>|<span data-ttu-id="0cdab-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0cdab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cdab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cdab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0cdab-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cdab-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0cdab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cdab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cdab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cdab-115">Not supported.</span></span>|
|<span data-ttu-id="0cdab-116">Application</span><span class="sxs-lookup"><span data-stu-id="0cdab-116">Application</span></span>|<span data-ttu-id="0cdab-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cdab-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cdab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cdab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/getExpiringVppTokenCount
```

## <a name="request-headers"></a><span data-ttu-id="0cdab-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cdab-119">Request headers</span></span>
|<span data-ttu-id="0cdab-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0cdab-120">Header</span></span>|<span data-ttu-id="0cdab-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0cdab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cdab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cdab-122">Authorization</span></span>|<span data-ttu-id="0cdab-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cdab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cdab-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0cdab-124">Accept</span></span>|<span data-ttu-id="0cdab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0cdab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cdab-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cdab-126">Request body</span></span>
<span data-ttu-id="0cdab-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="0cdab-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="0cdab-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="0cdab-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="0cdab-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cdab-129">Property</span></span>|<span data-ttu-id="0cdab-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cdab-130">Type</span></span>|<span data-ttu-id="0cdab-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cdab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cdab-132">expiringBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="0cdab-132">expiringBeforeDateTime</span></span>|<span data-ttu-id="0cdab-133">String</span><span class="sxs-lookup"><span data-stu-id="0cdab-133">String</span></span>|<span data-ttu-id="0cdab-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0cdab-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0cdab-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cdab-135">Response</span></span>
<span data-ttu-id="0cdab-136">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um Int32 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cdab-136">If successful, this function returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cdab-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cdab-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cdab-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cdab-138">Request</span></span>
<span data-ttu-id="0cdab-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cdab-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/getExpiringVppTokenCount(expiringBeforeDateTime='parameterValue')
```

### <a name="response"></a><span data-ttu-id="0cdab-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cdab-140">Response</span></span>
<span data-ttu-id="0cdab-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0cdab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 8
}
```






