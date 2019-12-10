---
title: ação updateDefinitionValues
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3dcf16f2d35b0f7968906c38e61cf49fc6c0ca70
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943190"
---
# <a name="updatedefinitionvalues-action"></a><span data-ttu-id="31270-103">ação updateDefinitionValues</span><span class="sxs-lookup"><span data-stu-id="31270-103">updateDefinitionValues action</span></span>

> <span data-ttu-id="31270-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31270-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31270-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31270-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31270-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="31270-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31270-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="31270-107">Prerequisites</span></span>
<span data-ttu-id="31270-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31270-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31270-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31270-110">Permission type</span></span>|<span data-ttu-id="31270-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="31270-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31270-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31270-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31270-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31270-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="31270-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31270-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31270-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31270-115">Not supported.</span></span>|
|<span data-ttu-id="31270-116">Application</span><span class="sxs-lookup"><span data-stu-id="31270-116">Application</span></span>|<span data-ttu-id="31270-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31270-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31270-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31270-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues
```

## <a name="request-headers"></a><span data-ttu-id="31270-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31270-119">Request headers</span></span>
|<span data-ttu-id="31270-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31270-120">Header</span></span>|<span data-ttu-id="31270-121">Valor</span><span class="sxs-lookup"><span data-stu-id="31270-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31270-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="31270-122">Authorization</span></span>|<span data-ttu-id="31270-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31270-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31270-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="31270-124">Accept</span></span>|<span data-ttu-id="31270-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31270-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31270-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31270-126">Request body</span></span>
<span data-ttu-id="31270-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="31270-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="31270-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="31270-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="31270-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31270-129">Property</span></span>|<span data-ttu-id="31270-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="31270-130">Type</span></span>|<span data-ttu-id="31270-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="31270-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31270-132">adicionado</span><span class="sxs-lookup"><span data-stu-id="31270-132">added</span></span>|<span data-ttu-id="31270-133">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="31270-133">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="31270-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="31270-134">Not yet documented</span></span>|
|<span data-ttu-id="31270-135">atualizado</span><span class="sxs-lookup"><span data-stu-id="31270-135">updated</span></span>|<span data-ttu-id="31270-136">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="31270-136">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="31270-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="31270-137">Not yet documented</span></span>|
|<span data-ttu-id="31270-138">deletedIds</span><span class="sxs-lookup"><span data-stu-id="31270-138">deletedIds</span></span>|<span data-ttu-id="31270-139">String collection</span><span class="sxs-lookup"><span data-stu-id="31270-139">String collection</span></span>|<span data-ttu-id="31270-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="31270-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="31270-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="31270-141">Response</span></span>
<span data-ttu-id="31270-142">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="31270-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="31270-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31270-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="31270-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31270-144">Request</span></span>
<span data-ttu-id="31270-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31270-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="31270-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="31270-146">Response</span></span>
<span data-ttu-id="31270-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31270-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





