---
title: ação updatePriorities
description: Atualizar prioridades de política.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07bbff5017523849d3be81b800bb2ea37eab1cd8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392057"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="32586-103">ação updatePriorities</span><span class="sxs-lookup"><span data-stu-id="32586-103">updatePriorities action</span></span>

<span data-ttu-id="32586-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32586-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32586-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="32586-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32586-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32586-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32586-107">Atualizar prioridades de política.</span><span class="sxs-lookup"><span data-stu-id="32586-107">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32586-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32586-108">Prerequisites</span></span>
<span data-ttu-id="32586-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32586-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32586-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32586-111">Permission type</span></span>|<span data-ttu-id="32586-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="32586-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32586-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32586-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32586-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32586-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32586-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32586-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32586-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32586-116">Not supported.</span></span>|
|<span data-ttu-id="32586-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32586-117">Application</span></span>|<span data-ttu-id="32586-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32586-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32586-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32586-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="32586-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32586-120">Request headers</span></span>
|<span data-ttu-id="32586-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32586-121">Header</span></span>|<span data-ttu-id="32586-122">Valor</span><span class="sxs-lookup"><span data-stu-id="32586-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32586-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="32586-123">Authorization</span></span>|<span data-ttu-id="32586-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32586-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32586-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="32586-125">Accept</span></span>|<span data-ttu-id="32586-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32586-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32586-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32586-127">Request body</span></span>
<span data-ttu-id="32586-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="32586-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="32586-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="32586-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="32586-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32586-130">Property</span></span>|<span data-ttu-id="32586-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="32586-131">Type</span></span>|<span data-ttu-id="32586-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="32586-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32586-133">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="32586-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="32586-134">Coleção String</span><span class="sxs-lookup"><span data-stu-id="32586-134">String collection</span></span>|<span data-ttu-id="32586-135">Lista de IDs de política de configuração do Office</span><span class="sxs-lookup"><span data-stu-id="32586-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="32586-136">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="32586-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="32586-137">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="32586-137">Int32 collection</span></span>|<span data-ttu-id="32586-138">Lista de prioridades de configuração do Office</span><span class="sxs-lookup"><span data-stu-id="32586-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="32586-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="32586-139">Response</span></span>
<span data-ttu-id="32586-140">Se tiver êxito, esta ação retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="32586-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="32586-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32586-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="32586-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32586-142">Request</span></span>
<span data-ttu-id="32586-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32586-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities

Content-type: application/json
Content-length: 143

{
  "officeConfigurationPolicyIds": [
    "Office Configuration Policy Ids value"
  ],
  "officeConfigurationPriorities": [
    13
  ]
}
```

### <a name="response"></a><span data-ttu-id="32586-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="32586-144">Response</span></span>
<span data-ttu-id="32586-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32586-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



