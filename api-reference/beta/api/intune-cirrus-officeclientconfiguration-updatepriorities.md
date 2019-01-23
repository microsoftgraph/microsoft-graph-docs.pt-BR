---
title: ação de updatePriorities
description: Atualize as prioridades de política.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a78ec2801522354709643dfdd88da0e6dd9756c8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412972"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="43017-103">ação de updatePriorities</span><span class="sxs-lookup"><span data-stu-id="43017-103">updatePriorities action</span></span>

> <span data-ttu-id="43017-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="43017-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="43017-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="43017-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43017-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="43017-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43017-107">Atualize as prioridades de política.</span><span class="sxs-lookup"><span data-stu-id="43017-107">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43017-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43017-108">Prerequisites</span></span>
<span data-ttu-id="43017-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43017-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43017-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43017-111">Permission type</span></span>|<span data-ttu-id="43017-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="43017-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43017-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43017-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43017-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43017-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43017-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43017-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43017-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43017-116">Not supported.</span></span>|
|<span data-ttu-id="43017-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43017-117">Application</span></span>|<span data-ttu-id="43017-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43017-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43017-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43017-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="43017-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43017-120">Request headers</span></span>
|<span data-ttu-id="43017-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43017-121">Header</span></span>|<span data-ttu-id="43017-122">Valor</span><span class="sxs-lookup"><span data-stu-id="43017-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43017-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="43017-123">Authorization</span></span>|<span data-ttu-id="43017-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43017-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43017-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43017-125">Accept</span></span>|<span data-ttu-id="43017-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43017-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43017-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43017-127">Request body</span></span>
<span data-ttu-id="43017-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="43017-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="43017-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="43017-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="43017-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43017-130">Property</span></span>|<span data-ttu-id="43017-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="43017-131">Type</span></span>|<span data-ttu-id="43017-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="43017-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43017-133">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="43017-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="43017-134">String collection</span><span class="sxs-lookup"><span data-stu-id="43017-134">String collection</span></span>|<span data-ttu-id="43017-135">Lista de ids de política de configuração do office</span><span class="sxs-lookup"><span data-stu-id="43017-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="43017-136">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="43017-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="43017-137">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="43017-137">Int32 collection</span></span>|<span data-ttu-id="43017-138">Lista de prioridades de configuração do office</span><span class="sxs-lookup"><span data-stu-id="43017-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="43017-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="43017-139">Response</span></span>
<span data-ttu-id="43017-140">Se tiver êxito, esta ação retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="43017-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="43017-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43017-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="43017-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43017-142">Request</span></span>
<span data-ttu-id="43017-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43017-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="43017-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="43017-144">Response</span></span>
<span data-ttu-id="43017-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43017-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



