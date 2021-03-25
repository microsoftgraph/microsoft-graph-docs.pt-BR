---
title: função compare
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76564db375a5d70719ef443bf2105a14fb852b20
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150728"
---
# <a name="compare-function"></a><span data-ttu-id="fa4f3-103">função compare</span><span class="sxs-lookup"><span data-stu-id="fa4f3-103">compare function</span></span>

<span data-ttu-id="fa4f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa4f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa4f3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fa4f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa4f3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa4f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa4f3-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fa4f3-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa4f3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fa4f3-108">Prerequisites</span></span>
<span data-ttu-id="fa4f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa4f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa4f3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa4f3-111">Permission type</span></span>|<span data-ttu-id="fa4f3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa4f3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa4f3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa4f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa4f3-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa4f3-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa4f3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa4f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa4f3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa4f3-116">Not supported.</span></span>|
|<span data-ttu-id="fa4f3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa4f3-117">Application</span></span>|<span data-ttu-id="fa4f3-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa4f3-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa4f3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa4f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/compare
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}/compare
```

## <a name="request-headers"></a><span data-ttu-id="fa4f3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa4f3-120">Request headers</span></span>
|<span data-ttu-id="fa4f3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa4f3-121">Header</span></span>|<span data-ttu-id="fa4f3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fa4f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa4f3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa4f3-123">Authorization</span></span>|<span data-ttu-id="fa4f3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa4f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa4f3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fa4f3-125">Accept</span></span>|<span data-ttu-id="fa4f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa4f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa4f3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa4f3-127">Request body</span></span>
<span data-ttu-id="fa4f3-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="fa4f3-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="fa4f3-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="fa4f3-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="fa4f3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa4f3-130">Property</span></span>|<span data-ttu-id="fa4f3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa4f3-131">Type</span></span>|<span data-ttu-id="fa4f3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa4f3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa4f3-133">templateId</span><span class="sxs-lookup"><span data-stu-id="fa4f3-133">templateId</span></span>|<span data-ttu-id="fa4f3-134">String</span><span class="sxs-lookup"><span data-stu-id="fa4f3-134">String</span></span>|<span data-ttu-id="fa4f3-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fa4f3-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fa4f3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa4f3-136">Response</span></span>
<span data-ttu-id="fa4f3-137">Se tiver êxito, essa função retornará um código de resposta e uma `200 OK` [coleção deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa4f3-137">If successful, this function returns a `200 OK` response code and a [deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa4f3-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa4f3-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa4f3-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa4f3-139">Request</span></span>
<span data-ttu-id="fa4f3-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa4f3-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/compare(templateId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="fa4f3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa4f3-141">Response</span></span>
<span data-ttu-id="fa4f3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa4f3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




