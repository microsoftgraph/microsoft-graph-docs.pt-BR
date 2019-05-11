---
title: ação updatePriorities
description: Atualizar prioridades de política.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 1a237ac20154e9356ff999bc5c671b02c15c7028
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934051"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="c2da5-103">ação updatePriorities</span><span class="sxs-lookup"><span data-stu-id="c2da5-103">updatePriorities action</span></span>

> <span data-ttu-id="c2da5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c2da5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2da5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c2da5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2da5-106">Atualizar prioridades de política.</span><span class="sxs-lookup"><span data-stu-id="c2da5-106">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2da5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c2da5-107">Prerequisites</span></span>
<span data-ttu-id="c2da5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2da5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2da5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2da5-110">Permission type</span></span>|<span data-ttu-id="c2da5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c2da5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2da5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2da5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c2da5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2da5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2da5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2da5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2da5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2da5-115">Not supported.</span></span>|
|<span data-ttu-id="c2da5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2da5-116">Application</span></span>|<span data-ttu-id="c2da5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2da5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2da5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2da5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="c2da5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2da5-119">Request headers</span></span>
|<span data-ttu-id="c2da5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c2da5-120">Header</span></span>|<span data-ttu-id="c2da5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c2da5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2da5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2da5-122">Authorization</span></span>|<span data-ttu-id="c2da5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2da5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2da5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c2da5-124">Accept</span></span>|<span data-ttu-id="c2da5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c2da5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2da5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2da5-126">Request body</span></span>
<span data-ttu-id="c2da5-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c2da5-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c2da5-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c2da5-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c2da5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2da5-129">Property</span></span>|<span data-ttu-id="c2da5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2da5-130">Type</span></span>|<span data-ttu-id="c2da5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2da5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2da5-132">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="c2da5-132">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="c2da5-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2da5-133">String collection</span></span>|<span data-ttu-id="c2da5-134">Lista de IDs de política de configuração do Office</span><span class="sxs-lookup"><span data-stu-id="c2da5-134">List of office configuration policy ids</span></span>|
|<span data-ttu-id="c2da5-135">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="c2da5-135">officeConfigurationPriorities</span></span>|<span data-ttu-id="c2da5-136">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="c2da5-136">Int32 collection</span></span>|<span data-ttu-id="c2da5-137">Lista de prioridades de configuração do Office</span><span class="sxs-lookup"><span data-stu-id="c2da5-137">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="c2da5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2da5-138">Response</span></span>
<span data-ttu-id="c2da5-139">Se tiver êxito, esta ação retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="c2da5-139">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c2da5-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2da5-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2da5-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2da5-141">Request</span></span>
<span data-ttu-id="c2da5-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2da5-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c2da5-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2da5-143">Response</span></span>
<span data-ttu-id="c2da5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2da5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



