---
title: função getOmaSettingPlainTextValue
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4662cf110a95bfaf718e2d9ed0756d2329bcd996
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752919"
---
# <a name="getomasettingplaintextvalue-function"></a><span data-ttu-id="7990e-103">função getOmaSettingPlainTextValue</span><span class="sxs-lookup"><span data-stu-id="7990e-103">getOmaSettingPlainTextValue function</span></span>

<span data-ttu-id="7990e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7990e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7990e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7990e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7990e-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7990e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7990e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7990e-107">Prerequisites</span></span>
<span data-ttu-id="7990e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7990e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7990e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7990e-110">Permission type</span></span>|<span data-ttu-id="7990e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7990e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7990e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7990e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7990e-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7990e-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7990e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7990e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7990e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7990e-115">Not supported.</span></span>|
|<span data-ttu-id="7990e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7990e-116">Application</span></span>|<span data-ttu-id="7990e-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7990e-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7990e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7990e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/getOmaSettingPlainTextValue
```

## <a name="request-headers"></a><span data-ttu-id="7990e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7990e-119">Request headers</span></span>
|<span data-ttu-id="7990e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7990e-120">Header</span></span>|<span data-ttu-id="7990e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7990e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7990e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7990e-122">Authorization</span></span>|<span data-ttu-id="7990e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7990e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7990e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7990e-124">Accept</span></span>|<span data-ttu-id="7990e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7990e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7990e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7990e-126">Request body</span></span>
<span data-ttu-id="7990e-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="7990e-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7990e-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="7990e-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7990e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7990e-129">Property</span></span>|<span data-ttu-id="7990e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7990e-130">Type</span></span>|<span data-ttu-id="7990e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7990e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7990e-132">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="7990e-132">secretReferenceValueId</span></span>|<span data-ttu-id="7990e-133">String</span><span class="sxs-lookup"><span data-stu-id="7990e-133">String</span></span>|<span data-ttu-id="7990e-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7990e-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7990e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7990e-135">Response</span></span>
<span data-ttu-id="7990e-136">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7990e-136">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7990e-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7990e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="7990e-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7990e-138">Request</span></span>
<span data-ttu-id="7990e-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7990e-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/getOmaSettingPlainTextValue(secretReferenceValueId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7990e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7990e-140">Response</span></span>
<span data-ttu-id="7990e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7990e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": "Get Oma Setting Plain Text Value value"
}
```




