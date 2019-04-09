---
title: Obter securityBaselineState
description: Leia as propriedades e as relações do objeto securityBaselineState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb7d60b37d0e9b8c916e44308414ae32062fd685
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522381"
---
# <a name="get-securitybaselinestate"></a><span data-ttu-id="82672-103">Obter securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="82672-103">Get securityBaselineState</span></span>

> <span data-ttu-id="82672-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="82672-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82672-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82672-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82672-106">Leia as propriedades e as relações do objeto [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) .</span><span class="sxs-lookup"><span data-stu-id="82672-106">Read properties and relationships of the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82672-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82672-107">Prerequisites</span></span>
<span data-ttu-id="82672-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="82672-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="82672-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82672-110">Permission type</span></span>|<span data-ttu-id="82672-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="82672-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82672-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82672-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82672-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="82672-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="82672-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82672-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82672-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82672-115">Not supported.</span></span>|
|<span data-ttu-id="82672-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82672-116">Application</span></span>|<span data-ttu-id="82672-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82672-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82672-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82672-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82672-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="82672-119">Optional query parameters</span></span>
<span data-ttu-id="82672-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="82672-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82672-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82672-121">Request headers</span></span>
|<span data-ttu-id="82672-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82672-122">Header</span></span>|<span data-ttu-id="82672-123">Valor</span><span class="sxs-lookup"><span data-stu-id="82672-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82672-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="82672-124">Authorization</span></span>|<span data-ttu-id="82672-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82672-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82672-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="82672-126">Accept</span></span>|<span data-ttu-id="82672-127">application/json</span><span class="sxs-lookup"><span data-stu-id="82672-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82672-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82672-128">Request body</span></span>
<span data-ttu-id="82672-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="82672-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82672-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="82672-130">Response</span></span>
<span data-ttu-id="82672-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82672-131">If successful, this method returns a `200 OK` response code and [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82672-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82672-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="82672-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82672-133">Request</span></span>
<span data-ttu-id="82672-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82672-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}
```

### <a name="response"></a><span data-ttu-id="82672-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="82672-135">Response</span></span>
<span data-ttu-id="82672-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82672-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "value": {
    "@odata.type": "#microsoft.graph.securityBaselineState",
    "id": "23dc2503-2503-23dc-0325-dc230325dc23",
    "securityBaselineTemplateId": "Security Baseline Template Id value",
    "displayName": "Display Name value"
  }
}
```



