---
title: função compare
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8fe8ef09b1aff798b62e995f6136e0acb7657d5e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43328283"
---
# <a name="compare-function"></a><span data-ttu-id="2ae91-103">função compare</span><span class="sxs-lookup"><span data-stu-id="2ae91-103">compare function</span></span>

<span data-ttu-id="2ae91-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ae91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ae91-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ae91-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ae91-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ae91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ae91-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2ae91-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ae91-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ae91-108">Prerequisites</span></span>
<span data-ttu-id="2ae91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ae91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ae91-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ae91-111">Permission type</span></span>|<span data-ttu-id="2ae91-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ae91-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ae91-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ae91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ae91-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ae91-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2ae91-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ae91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ae91-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ae91-116">Not supported.</span></span>|
|<span data-ttu-id="2ae91-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ae91-117">Application</span></span>|<span data-ttu-id="2ae91-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ae91-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ae91-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ae91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/compare
```

## <a name="request-headers"></a><span data-ttu-id="2ae91-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ae91-120">Request headers</span></span>
|<span data-ttu-id="2ae91-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ae91-121">Header</span></span>|<span data-ttu-id="2ae91-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2ae91-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ae91-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ae91-123">Authorization</span></span>|<span data-ttu-id="2ae91-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ae91-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ae91-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ae91-125">Accept</span></span>|<span data-ttu-id="2ae91-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ae91-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ae91-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ae91-127">Request body</span></span>
<span data-ttu-id="2ae91-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="2ae91-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2ae91-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="2ae91-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2ae91-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ae91-130">Property</span></span>|<span data-ttu-id="2ae91-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ae91-131">Type</span></span>|<span data-ttu-id="2ae91-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ae91-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ae91-133">templateId</span><span class="sxs-lookup"><span data-stu-id="2ae91-133">templateId</span></span>|<span data-ttu-id="2ae91-134">String</span><span class="sxs-lookup"><span data-stu-id="2ae91-134">String</span></span>|<span data-ttu-id="2ae91-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2ae91-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2ae91-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ae91-136">Response</span></span>
<span data-ttu-id="2ae91-137">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ae91-137">If successful, this function returns a `200 OK` response code and a [deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ae91-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ae91-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ae91-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ae91-139">Request</span></span>
<span data-ttu-id="2ae91-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ae91-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/compare(templateId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="2ae91-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ae91-141">Response</span></span>
<span data-ttu-id="2ae91-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ae91-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 364

{
  "value": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingComparison",
      "id": "Id value",
      "displayName": "Display Name value",
      "definitionId": "Definition Id value",
      "currentValueJson": "Current Value Json value",
      "newValueJson": "New Value Json value",
      "comparisonResult": "equal"
    }
  ]
}
```



