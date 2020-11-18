---
title: função getSuggestedEnrollmentLimit
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 22529ec1571c1f7bc363d0ed3740739316ecd53e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49201657"
---
# <a name="getsuggestedenrollmentlimit-function"></a><span data-ttu-id="9579a-103">função getSuggestedEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="9579a-103">getSuggestedEnrollmentLimit function</span></span>

<span data-ttu-id="9579a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9579a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9579a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9579a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9579a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9579a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9579a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9579a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9579a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9579a-108">Prerequisites</span></span>
<span data-ttu-id="9579a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9579a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9579a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9579a-111">Permission type</span></span>|<span data-ttu-id="9579a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9579a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9579a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9579a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9579a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9579a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9579a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9579a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9579a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9579a-116">Not supported.</span></span>|
|<span data-ttu-id="9579a-117">Application</span><span class="sxs-lookup"><span data-stu-id="9579a-117">Application</span></span>|<span data-ttu-id="9579a-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9579a-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9579a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9579a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getSuggestedEnrollmentLimit
```

## <a name="request-headers"></a><span data-ttu-id="9579a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9579a-120">Request headers</span></span>
|<span data-ttu-id="9579a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9579a-121">Header</span></span>|<span data-ttu-id="9579a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9579a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9579a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9579a-123">Authorization</span></span>|<span data-ttu-id="9579a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9579a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9579a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9579a-125">Accept</span></span>|<span data-ttu-id="9579a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9579a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9579a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9579a-127">Request body</span></span>
<span data-ttu-id="9579a-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="9579a-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9579a-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="9579a-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9579a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9579a-130">Property</span></span>|<span data-ttu-id="9579a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9579a-131">Type</span></span>|<span data-ttu-id="9579a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9579a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9579a-133">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="9579a-133">enrollmentType</span></span>|<span data-ttu-id="9579a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9579a-134">String</span></span>|<span data-ttu-id="9579a-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9579a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9579a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9579a-136">Response</span></span>
<span data-ttu-id="9579a-137">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um [suggestedEnrollmentLimit](../resources/intune-enrollment-suggestedenrollmentlimit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9579a-137">If successful, this function returns a `200 OK` response code and a [suggestedEnrollmentLimit](../resources/intune-enrollment-suggestedenrollmentlimit.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9579a-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9579a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="9579a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9579a-139">Request</span></span>
<span data-ttu-id="9579a-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9579a-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getSuggestedEnrollmentLimit(enrollmentType='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9579a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9579a-141">Response</span></span>
<span data-ttu-id="9579a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9579a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 117

{
  "value": {
    "@odata.type": "microsoft.graph.suggestedEnrollmentLimit",
    "suggestedDailyLimit": 3
  }
}
```




