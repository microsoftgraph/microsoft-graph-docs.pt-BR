---
title: ação updatePriorities
description: Atualizar prioridades de política.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b1ed9ad9d44502a32387452d789db8581e95f2ca
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752934"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="01224-103">ação updatePriorities</span><span class="sxs-lookup"><span data-stu-id="01224-103">updatePriorities action</span></span>

<span data-ttu-id="01224-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01224-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01224-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01224-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01224-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01224-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01224-107">Atualizar prioridades de política.</span><span class="sxs-lookup"><span data-stu-id="01224-107">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01224-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01224-108">Prerequisites</span></span>
<span data-ttu-id="01224-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01224-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01224-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01224-111">Permission type</span></span>|<span data-ttu-id="01224-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01224-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01224-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01224-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01224-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01224-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01224-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01224-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01224-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01224-116">Not supported.</span></span>|
|<span data-ttu-id="01224-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01224-117">Application</span></span>|<span data-ttu-id="01224-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01224-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01224-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01224-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="01224-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01224-120">Request headers</span></span>
|<span data-ttu-id="01224-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01224-121">Header</span></span>|<span data-ttu-id="01224-122">Valor</span><span class="sxs-lookup"><span data-stu-id="01224-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01224-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="01224-123">Authorization</span></span>|<span data-ttu-id="01224-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01224-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01224-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01224-125">Accept</span></span>|<span data-ttu-id="01224-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01224-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01224-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01224-127">Request body</span></span>
<span data-ttu-id="01224-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="01224-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="01224-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="01224-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="01224-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01224-130">Property</span></span>|<span data-ttu-id="01224-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="01224-131">Type</span></span>|<span data-ttu-id="01224-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="01224-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01224-133">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="01224-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="01224-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="01224-134">String collection</span></span>|<span data-ttu-id="01224-135">Lista de ids de política de configuração do office</span><span class="sxs-lookup"><span data-stu-id="01224-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="01224-136">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="01224-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="01224-137">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="01224-137">Int32 collection</span></span>|<span data-ttu-id="01224-138">Lista de prioridades de configuração do office</span><span class="sxs-lookup"><span data-stu-id="01224-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="01224-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="01224-139">Response</span></span>
<span data-ttu-id="01224-140">Se tiver êxito, esta ação retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="01224-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="01224-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01224-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="01224-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01224-142">Request</span></span>
<span data-ttu-id="01224-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01224-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01224-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="01224-144">Response</span></span>
<span data-ttu-id="01224-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01224-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```




