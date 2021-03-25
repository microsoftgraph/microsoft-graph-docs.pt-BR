---
title: ação extendQualityUpdatesPause
description: Estender Atualizações de Qualidade Pausar para um toque do Windows Update para Empresas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc3d4208d76b1cd4c0c48e649126d2c6e1994491
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150868"
---
# <a name="extendqualityupdatespause-action"></a><span data-ttu-id="8e33b-103">ação extendQualityUpdatesPause</span><span class="sxs-lookup"><span data-stu-id="8e33b-103">extendQualityUpdatesPause action</span></span>

<span data-ttu-id="8e33b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e33b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e33b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e33b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e33b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e33b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e33b-107">Estender Atualizações de Qualidade Pausar para um toque do Windows Update para Empresas.</span><span class="sxs-lookup"><span data-stu-id="8e33b-107">Extend Quality Updates Pause for a Windows Update for Business ring.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e33b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e33b-108">Prerequisites</span></span>
<span data-ttu-id="8e33b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e33b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e33b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e33b-111">Permission type</span></span>|<span data-ttu-id="8e33b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e33b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e33b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e33b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e33b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e33b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e33b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e33b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e33b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e33b-116">Not supported.</span></span>|
|<span data-ttu-id="8e33b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e33b-117">Application</span></span>|<span data-ttu-id="8e33b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e33b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e33b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e33b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/extendQualityUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
```

## <a name="request-headers"></a><span data-ttu-id="8e33b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e33b-120">Request headers</span></span>
|<span data-ttu-id="8e33b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e33b-121">Header</span></span>|<span data-ttu-id="8e33b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8e33b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e33b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e33b-123">Authorization</span></span>|<span data-ttu-id="8e33b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e33b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e33b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e33b-125">Accept</span></span>|<span data-ttu-id="8e33b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e33b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e33b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e33b-127">Request body</span></span>
<span data-ttu-id="8e33b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e33b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e33b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e33b-129">Response</span></span>
<span data-ttu-id="8e33b-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8e33b-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8e33b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e33b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e33b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e33b-132">Request</span></span>
<span data-ttu-id="8e33b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e33b-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
```

### <a name="response"></a><span data-ttu-id="8e33b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e33b-134">Response</span></span>
<span data-ttu-id="8e33b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e33b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




