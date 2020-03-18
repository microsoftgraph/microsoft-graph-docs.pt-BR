---
title: ação updateDefinitionValues
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57ca380359c1323cc0b3238f6f66b56e143afbd0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804475"
---
# <a name="updatedefinitionvalues-action"></a><span data-ttu-id="bd89c-103">ação updateDefinitionValues</span><span class="sxs-lookup"><span data-stu-id="bd89c-103">updateDefinitionValues action</span></span>

> <span data-ttu-id="bd89c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bd89c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd89c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bd89c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd89c-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bd89c-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd89c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bd89c-107">Prerequisites</span></span>
<span data-ttu-id="bd89c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd89c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd89c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd89c-110">Permission type</span></span>|<span data-ttu-id="bd89c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bd89c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd89c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd89c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bd89c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd89c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bd89c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd89c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd89c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd89c-115">Not supported.</span></span>|
|<span data-ttu-id="bd89c-116">Application</span><span class="sxs-lookup"><span data-stu-id="bd89c-116">Application</span></span>|<span data-ttu-id="bd89c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd89c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd89c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd89c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues
```

## <a name="request-headers"></a><span data-ttu-id="bd89c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd89c-119">Request headers</span></span>
|<span data-ttu-id="bd89c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd89c-120">Header</span></span>|<span data-ttu-id="bd89c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bd89c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd89c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd89c-122">Authorization</span></span>|<span data-ttu-id="bd89c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd89c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd89c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bd89c-124">Accept</span></span>|<span data-ttu-id="bd89c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bd89c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd89c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd89c-126">Request body</span></span>
<span data-ttu-id="bd89c-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="bd89c-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="bd89c-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="bd89c-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="bd89c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd89c-129">Property</span></span>|<span data-ttu-id="bd89c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd89c-130">Type</span></span>|<span data-ttu-id="bd89c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd89c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd89c-132">adicionado</span><span class="sxs-lookup"><span data-stu-id="bd89c-132">added</span></span>|<span data-ttu-id="bd89c-133">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="bd89c-133">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="bd89c-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bd89c-134">Not yet documented</span></span>|
|<span data-ttu-id="bd89c-135">atualizado</span><span class="sxs-lookup"><span data-stu-id="bd89c-135">updated</span></span>|<span data-ttu-id="bd89c-136">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="bd89c-136">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="bd89c-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bd89c-137">Not yet documented</span></span>|
|<span data-ttu-id="bd89c-138">deletedIds</span><span class="sxs-lookup"><span data-stu-id="bd89c-138">deletedIds</span></span>|<span data-ttu-id="bd89c-139">String collection</span><span class="sxs-lookup"><span data-stu-id="bd89c-139">String collection</span></span>|<span data-ttu-id="bd89c-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bd89c-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bd89c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd89c-141">Response</span></span>
<span data-ttu-id="bd89c-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bd89c-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bd89c-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd89c-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd89c-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd89c-144">Request</span></span>
<span data-ttu-id="bd89c-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd89c-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bd89c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd89c-146">Response</span></span>
<span data-ttu-id="bd89c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd89c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




