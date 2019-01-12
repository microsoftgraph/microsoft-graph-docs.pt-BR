---
title: ação de updatePriorities
description: Atualize as prioridades de política.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 15c57de2077842ff2115770859fc34357e0f6a22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940474"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="3c064-103">ação de updatePriorities</span><span class="sxs-lookup"><span data-stu-id="3c064-103">updatePriorities action</span></span>

> <span data-ttu-id="3c064-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3c064-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c064-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3c064-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c064-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3c064-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c064-107">Atualize as prioridades de política.</span><span class="sxs-lookup"><span data-stu-id="3c064-107">Update policy priorities.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c064-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c064-108">Prerequisites</span></span>
<span data-ttu-id="3c064-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c064-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c064-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c064-111">Permission type</span></span>|<span data-ttu-id="3c064-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c064-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c064-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c064-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c064-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c064-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c064-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c064-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c064-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c064-116">Not supported.</span></span>|
|<span data-ttu-id="3c064-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c064-117">Application</span></span>|<span data-ttu-id="3c064-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c064-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c064-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c064-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="3c064-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c064-120">Request headers</span></span>
|<span data-ttu-id="3c064-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c064-121">Header</span></span>|<span data-ttu-id="3c064-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3c064-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c064-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c064-123">Authorization</span></span>|<span data-ttu-id="3c064-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c064-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c064-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c064-125">Accept</span></span>|<span data-ttu-id="3c064-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c064-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c064-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c064-127">Request body</span></span>
<span data-ttu-id="3c064-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3c064-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3c064-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3c064-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3c064-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c064-130">Property</span></span>|<span data-ttu-id="3c064-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c064-131">Type</span></span>|<span data-ttu-id="3c064-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c064-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c064-133">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="3c064-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="3c064-134">String collection</span><span class="sxs-lookup"><span data-stu-id="3c064-134">String collection</span></span>|<span data-ttu-id="3c064-135">Lista de ids de política de configuração do office</span><span class="sxs-lookup"><span data-stu-id="3c064-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="3c064-136">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="3c064-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="3c064-137">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="3c064-137">Int32 collection</span></span>|<span data-ttu-id="3c064-138">Lista de prioridades de configuração do office</span><span class="sxs-lookup"><span data-stu-id="3c064-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="3c064-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c064-139">Response</span></span>
<span data-ttu-id="3c064-140">Se tiver êxito, esta ação retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="3c064-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3c064-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c064-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c064-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c064-142">Request</span></span>
<span data-ttu-id="3c064-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c064-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3c064-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c064-144">Response</span></span>
<span data-ttu-id="3c064-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c064-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



