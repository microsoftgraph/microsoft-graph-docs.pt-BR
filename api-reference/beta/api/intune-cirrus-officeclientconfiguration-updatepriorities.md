---
title: ação updatePriorities
description: Atualizar prioridades de política.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ce00442a7aead88e2f5d17f1de772ae46801b8ba
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730259"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="1b972-103">ação updatePriorities</span><span class="sxs-lookup"><span data-stu-id="1b972-103">updatePriorities action</span></span>

<span data-ttu-id="1b972-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b972-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b972-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1b972-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b972-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1b972-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b972-107">Atualizar prioridades de política.</span><span class="sxs-lookup"><span data-stu-id="1b972-107">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b972-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1b972-108">Prerequisites</span></span>
<span data-ttu-id="1b972-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b972-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b972-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b972-111">Permission type</span></span>|<span data-ttu-id="1b972-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1b972-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b972-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b972-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b972-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b972-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b972-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b972-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b972-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b972-116">Not supported.</span></span>|
|<span data-ttu-id="1b972-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b972-117">Application</span></span>|<span data-ttu-id="1b972-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b972-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b972-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b972-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="1b972-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b972-120">Request headers</span></span>
|<span data-ttu-id="1b972-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b972-121">Header</span></span>|<span data-ttu-id="1b972-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1b972-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b972-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b972-123">Authorization</span></span>|<span data-ttu-id="1b972-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b972-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b972-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1b972-125">Accept</span></span>|<span data-ttu-id="1b972-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b972-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b972-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b972-127">Request body</span></span>
<span data-ttu-id="1b972-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1b972-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1b972-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="1b972-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1b972-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b972-130">Property</span></span>|<span data-ttu-id="1b972-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b972-131">Type</span></span>|<span data-ttu-id="1b972-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b972-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b972-133">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="1b972-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="1b972-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b972-134">String collection</span></span>|<span data-ttu-id="1b972-135">Lista de IDs de política de configuração do Office</span><span class="sxs-lookup"><span data-stu-id="1b972-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="1b972-136">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="1b972-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="1b972-137">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="1b972-137">Int32 collection</span></span>|<span data-ttu-id="1b972-138">Lista de prioridades de configuração do Office</span><span class="sxs-lookup"><span data-stu-id="1b972-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="1b972-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b972-139">Response</span></span>
<span data-ttu-id="1b972-140">Se tiver êxito, esta ação retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="1b972-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1b972-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b972-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b972-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b972-142">Request</span></span>
<span data-ttu-id="1b972-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b972-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1b972-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b972-144">Response</span></span>
<span data-ttu-id="1b972-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b972-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```





