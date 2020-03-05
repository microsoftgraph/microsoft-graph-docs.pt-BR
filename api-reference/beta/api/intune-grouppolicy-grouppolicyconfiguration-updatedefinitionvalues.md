---
title: ação updateDefinitionValues
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c1ec5462365f6c28ff7f72bc47f0bb31f684fb9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465188"
---
# <a name="updatedefinitionvalues-action"></a><span data-ttu-id="6564e-103">ação updateDefinitionValues</span><span class="sxs-lookup"><span data-stu-id="6564e-103">updateDefinitionValues action</span></span>

<span data-ttu-id="6564e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6564e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6564e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6564e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6564e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6564e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6564e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6564e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6564e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6564e-108">Prerequisites</span></span>
<span data-ttu-id="6564e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6564e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6564e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6564e-111">Permission type</span></span>|<span data-ttu-id="6564e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6564e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6564e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6564e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6564e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6564e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6564e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6564e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6564e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6564e-116">Not supported.</span></span>|
|<span data-ttu-id="6564e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6564e-117">Application</span></span>|<span data-ttu-id="6564e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6564e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6564e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6564e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues
```

## <a name="request-headers"></a><span data-ttu-id="6564e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6564e-120">Request headers</span></span>
|<span data-ttu-id="6564e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6564e-121">Header</span></span>|<span data-ttu-id="6564e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6564e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6564e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6564e-123">Authorization</span></span>|<span data-ttu-id="6564e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6564e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6564e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6564e-125">Accept</span></span>|<span data-ttu-id="6564e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6564e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6564e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6564e-127">Request body</span></span>
<span data-ttu-id="6564e-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6564e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6564e-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="6564e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6564e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6564e-130">Property</span></span>|<span data-ttu-id="6564e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6564e-131">Type</span></span>|<span data-ttu-id="6564e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6564e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6564e-133">adicionado</span><span class="sxs-lookup"><span data-stu-id="6564e-133">added</span></span>|<span data-ttu-id="6564e-134">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6564e-134">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="6564e-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6564e-135">Not yet documented</span></span>|
|<span data-ttu-id="6564e-136">atualizado</span><span class="sxs-lookup"><span data-stu-id="6564e-136">updated</span></span>|<span data-ttu-id="6564e-137">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6564e-137">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="6564e-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6564e-138">Not yet documented</span></span>|
|<span data-ttu-id="6564e-139">deletedIds</span><span class="sxs-lookup"><span data-stu-id="6564e-139">deletedIds</span></span>|<span data-ttu-id="6564e-140">String collection</span><span class="sxs-lookup"><span data-stu-id="6564e-140">String collection</span></span>|<span data-ttu-id="6564e-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6564e-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6564e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6564e-142">Response</span></span>
<span data-ttu-id="6564e-143">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6564e-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6564e-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6564e-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="6564e-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6564e-145">Request</span></span>
<span data-ttu-id="6564e-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6564e-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6564e-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6564e-147">Response</span></span>
<span data-ttu-id="6564e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6564e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





