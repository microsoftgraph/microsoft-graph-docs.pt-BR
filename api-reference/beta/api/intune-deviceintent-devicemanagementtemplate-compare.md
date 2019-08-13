---
title: função compare
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 15b3755dcd3fb13d3afafa66322b2ad984030b67
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313143"
---
# <a name="compare-function"></a><span data-ttu-id="080d3-103">função compare</span><span class="sxs-lookup"><span data-stu-id="080d3-103">compare function</span></span>

> <span data-ttu-id="080d3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="080d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="080d3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="080d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="080d3-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="080d3-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="080d3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="080d3-107">Prerequisites</span></span>
<span data-ttu-id="080d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="080d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="080d3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="080d3-110">Permission type</span></span>|<span data-ttu-id="080d3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="080d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="080d3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="080d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="080d3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="080d3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="080d3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="080d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="080d3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="080d3-115">Not supported.</span></span>|
|<span data-ttu-id="080d3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="080d3-116">Application</span></span>|<span data-ttu-id="080d3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="080d3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="080d3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="080d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/compare
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}/compare
```

## <a name="request-headers"></a><span data-ttu-id="080d3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="080d3-119">Request headers</span></span>
|<span data-ttu-id="080d3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="080d3-120">Header</span></span>|<span data-ttu-id="080d3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="080d3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="080d3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="080d3-122">Authorization</span></span>|<span data-ttu-id="080d3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="080d3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="080d3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="080d3-124">Accept</span></span>|<span data-ttu-id="080d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="080d3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="080d3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="080d3-126">Request body</span></span>
<span data-ttu-id="080d3-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="080d3-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="080d3-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="080d3-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="080d3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="080d3-129">Property</span></span>|<span data-ttu-id="080d3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="080d3-130">Type</span></span>|<span data-ttu-id="080d3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="080d3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="080d3-132">templateId</span><span class="sxs-lookup"><span data-stu-id="080d3-132">templateId</span></span>|<span data-ttu-id="080d3-133">String</span><span class="sxs-lookup"><span data-stu-id="080d3-133">String</span></span>|<span data-ttu-id="080d3-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="080d3-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="080d3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="080d3-135">Response</span></span>
<span data-ttu-id="080d3-136">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="080d3-136">If successful, this function returns a `200 OK` response code and a [deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="080d3-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="080d3-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="080d3-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="080d3-138">Request</span></span>
<span data-ttu-id="080d3-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="080d3-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/compare(templateId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="080d3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="080d3-140">Response</span></span>
<span data-ttu-id="080d3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="080d3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






