---
title: ação extendFeatureUpdatesPause
description: Estender as atualizações de recurso pausar para um toque do Windows Update para empresas.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aef0e53d4b9a68a54f967a7f5cdce5dd18282dea
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917405"
---
# <a name="extendfeatureupdatespause-action"></a><span data-ttu-id="498ad-103">ação extendFeatureUpdatesPause</span><span class="sxs-lookup"><span data-stu-id="498ad-103">extendFeatureUpdatesPause action</span></span>

> <span data-ttu-id="498ad-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="498ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="498ad-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="498ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="498ad-106">Estender as atualizações de recurso pausar para um toque do Windows Update para empresas.</span><span class="sxs-lookup"><span data-stu-id="498ad-106">Extend Feature Updates Pause for a Windows Update for Business ring.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="498ad-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="498ad-107">Prerequisites</span></span>
<span data-ttu-id="498ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="498ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="498ad-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="498ad-110">Permission type</span></span>|<span data-ttu-id="498ad-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="498ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="498ad-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="498ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="498ad-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="498ad-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="498ad-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="498ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="498ad-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="498ad-115">Not supported.</span></span>|
|<span data-ttu-id="498ad-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="498ad-116">Application</span></span>|<span data-ttu-id="498ad-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="498ad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="498ad-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="498ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendFeatureUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/extendFeatureUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/extendFeatureUpdatesPause
```

## <a name="request-headers"></a><span data-ttu-id="498ad-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="498ad-119">Request headers</span></span>
|<span data-ttu-id="498ad-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="498ad-120">Header</span></span>|<span data-ttu-id="498ad-121">Valor</span><span class="sxs-lookup"><span data-stu-id="498ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="498ad-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="498ad-122">Authorization</span></span>|<span data-ttu-id="498ad-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="498ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="498ad-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="498ad-124">Accept</span></span>|<span data-ttu-id="498ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="498ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="498ad-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="498ad-126">Request body</span></span>
<span data-ttu-id="498ad-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="498ad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="498ad-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="498ad-128">Response</span></span>
<span data-ttu-id="498ad-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="498ad-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="498ad-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="498ad-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="498ad-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="498ad-131">Request</span></span>
<span data-ttu-id="498ad-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="498ad-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendFeatureUpdatesPause
```

### <a name="response"></a><span data-ttu-id="498ad-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="498ad-133">Response</span></span>
<span data-ttu-id="498ad-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="498ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




