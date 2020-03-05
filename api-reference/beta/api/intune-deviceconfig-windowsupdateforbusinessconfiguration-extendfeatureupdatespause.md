---
title: ação extendFeatureUpdatesPause
description: Estender as atualizações de recurso pausar para um toque do Windows Update para empresas.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 09d3a12bdcb58b6f88f316c5461f435f7866e819
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42473735"
---
# <a name="extendfeatureupdatespause-action"></a><span data-ttu-id="57b96-103">ação extendFeatureUpdatesPause</span><span class="sxs-lookup"><span data-stu-id="57b96-103">extendFeatureUpdatesPause action</span></span>

<span data-ttu-id="57b96-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="57b96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57b96-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57b96-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57b96-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57b96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57b96-107">Estender as atualizações de recurso pausar para um toque do Windows Update para empresas.</span><span class="sxs-lookup"><span data-stu-id="57b96-107">Extend Feature Updates Pause for a Windows Update for Business ring.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57b96-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57b96-108">Prerequisites</span></span>
<span data-ttu-id="57b96-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57b96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57b96-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57b96-111">Permission type</span></span>|<span data-ttu-id="57b96-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57b96-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57b96-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57b96-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57b96-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57b96-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57b96-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57b96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57b96-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57b96-116">Not supported.</span></span>|
|<span data-ttu-id="57b96-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57b96-117">Application</span></span>|<span data-ttu-id="57b96-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57b96-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57b96-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57b96-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendFeatureUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/extendFeatureUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/extendFeatureUpdatesPause
```

## <a name="request-headers"></a><span data-ttu-id="57b96-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57b96-120">Request headers</span></span>
|<span data-ttu-id="57b96-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57b96-121">Header</span></span>|<span data-ttu-id="57b96-122">Valor</span><span class="sxs-lookup"><span data-stu-id="57b96-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57b96-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="57b96-123">Authorization</span></span>|<span data-ttu-id="57b96-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57b96-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57b96-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57b96-125">Accept</span></span>|<span data-ttu-id="57b96-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57b96-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57b96-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57b96-127">Request body</span></span>
<span data-ttu-id="57b96-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57b96-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57b96-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="57b96-129">Response</span></span>
<span data-ttu-id="57b96-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="57b96-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="57b96-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57b96-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="57b96-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57b96-132">Request</span></span>
<span data-ttu-id="57b96-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57b96-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendFeatureUpdatesPause
```

### <a name="response"></a><span data-ttu-id="57b96-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="57b96-134">Response</span></span>
<span data-ttu-id="57b96-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57b96-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





