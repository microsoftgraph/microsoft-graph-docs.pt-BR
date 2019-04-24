---
title: ação updatePriorities
description: Atualizar prioridades de política.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6422cd3f40270f6502a58551e6c5c1b739219e00
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32483163"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="4724f-103">ação updatePriorities</span><span class="sxs-lookup"><span data-stu-id="4724f-103">updatePriorities action</span></span>

> <span data-ttu-id="4724f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4724f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4724f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4724f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4724f-106">Atualizar prioridades de política.</span><span class="sxs-lookup"><span data-stu-id="4724f-106">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4724f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4724f-107">Prerequisites</span></span>
<span data-ttu-id="4724f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4724f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4724f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4724f-110">Permission type</span></span>|<span data-ttu-id="4724f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4724f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4724f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4724f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4724f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4724f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4724f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4724f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4724f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4724f-115">Not supported.</span></span>|
|<span data-ttu-id="4724f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4724f-116">Application</span></span>|<span data-ttu-id="4724f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4724f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4724f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4724f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="4724f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4724f-119">Request headers</span></span>
|<span data-ttu-id="4724f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4724f-120">Header</span></span>|<span data-ttu-id="4724f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4724f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4724f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4724f-122">Authorization</span></span>|<span data-ttu-id="4724f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4724f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4724f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4724f-124">Accept</span></span>|<span data-ttu-id="4724f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4724f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4724f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4724f-126">Request body</span></span>
<span data-ttu-id="4724f-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="4724f-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4724f-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="4724f-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4724f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4724f-129">Property</span></span>|<span data-ttu-id="4724f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4724f-130">Type</span></span>|<span data-ttu-id="4724f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4724f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4724f-132">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="4724f-132">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="4724f-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4724f-133">String collection</span></span>|<span data-ttu-id="4724f-134">Lista de IDs de política de configuração do Office</span><span class="sxs-lookup"><span data-stu-id="4724f-134">List of office configuration policy ids</span></span>|
|<span data-ttu-id="4724f-135">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="4724f-135">officeConfigurationPriorities</span></span>|<span data-ttu-id="4724f-136">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="4724f-136">Int32 collection</span></span>|<span data-ttu-id="4724f-137">Lista de prioridades de configuração do Office</span><span class="sxs-lookup"><span data-stu-id="4724f-137">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="4724f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4724f-138">Response</span></span>
<span data-ttu-id="4724f-139">Se tiver êxito, esta ação retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4724f-139">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4724f-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4724f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="4724f-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4724f-141">Request</span></span>
<span data-ttu-id="4724f-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4724f-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4724f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4724f-143">Response</span></span>
<span data-ttu-id="4724f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4724f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



