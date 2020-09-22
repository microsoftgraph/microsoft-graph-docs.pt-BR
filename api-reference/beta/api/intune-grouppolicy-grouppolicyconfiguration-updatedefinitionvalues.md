---
title: ação updateDefinitionValues
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cfd402a0ff6e6b4588630ab64c29692c8e60672
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48068382"
---
# <a name="updatedefinitionvalues-action"></a><span data-ttu-id="48e52-103">ação updateDefinitionValues</span><span class="sxs-lookup"><span data-stu-id="48e52-103">updateDefinitionValues action</span></span>

<span data-ttu-id="48e52-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48e52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48e52-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48e52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48e52-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48e52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48e52-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48e52-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48e52-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="48e52-108">Prerequisites</span></span>
<span data-ttu-id="48e52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48e52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48e52-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48e52-111">Permission type</span></span>|<span data-ttu-id="48e52-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="48e52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48e52-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48e52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48e52-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48e52-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48e52-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48e52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48e52-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48e52-116">Not supported.</span></span>|
|<span data-ttu-id="48e52-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48e52-117">Application</span></span>|<span data-ttu-id="48e52-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48e52-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48e52-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48e52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues
```

## <a name="request-headers"></a><span data-ttu-id="48e52-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48e52-120">Request headers</span></span>
|<span data-ttu-id="48e52-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48e52-121">Header</span></span>|<span data-ttu-id="48e52-122">Valor</span><span class="sxs-lookup"><span data-stu-id="48e52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48e52-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="48e52-123">Authorization</span></span>|<span data-ttu-id="48e52-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48e52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48e52-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="48e52-125">Accept</span></span>|<span data-ttu-id="48e52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48e52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48e52-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48e52-127">Request body</span></span>
<span data-ttu-id="48e52-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="48e52-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="48e52-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="48e52-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="48e52-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48e52-130">Property</span></span>|<span data-ttu-id="48e52-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="48e52-131">Type</span></span>|<span data-ttu-id="48e52-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="48e52-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48e52-133">adicionado</span><span class="sxs-lookup"><span data-stu-id="48e52-133">added</span></span>|<span data-ttu-id="48e52-134">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="48e52-134">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="48e52-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48e52-135">Not yet documented</span></span>|
|<span data-ttu-id="48e52-136">atualizado</span><span class="sxs-lookup"><span data-stu-id="48e52-136">updated</span></span>|<span data-ttu-id="48e52-137">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="48e52-137">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="48e52-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48e52-138">Not yet documented</span></span>|
|<span data-ttu-id="48e52-139">deletedIds</span><span class="sxs-lookup"><span data-stu-id="48e52-139">deletedIds</span></span>|<span data-ttu-id="48e52-140">String collection</span><span class="sxs-lookup"><span data-stu-id="48e52-140">String collection</span></span>|<span data-ttu-id="48e52-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48e52-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="48e52-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="48e52-142">Response</span></span>
<span data-ttu-id="48e52-143">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="48e52-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="48e52-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48e52-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="48e52-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48e52-145">Request</span></span>
<span data-ttu-id="48e52-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48e52-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues

Content-type: application/json
Content-length: 759

{
  "added": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "enabled": true,
      "configurationType": "preference",
      "id": "50428918-8918-5042-1889-425018894250",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ],
  "updated": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "enabled": true,
      "configurationType": "preference",
      "id": "50428918-8918-5042-1889-425018894250",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ],
  "deletedIds": [
    "Deleted Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="48e52-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="48e52-147">Response</span></span>
<span data-ttu-id="48e52-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48e52-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






