---
title: Excluir iosEasEmailProfileConfiguration
description: Exclui iosEasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ddadca7734fe178fa65b74356650dd2054610a32
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35948478"
---
# <a name="delete-ioseasemailprofileconfiguration"></a><span data-ttu-id="49dae-103">Excluir iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="49dae-103">Delete iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="49dae-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49dae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49dae-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49dae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49dae-106">Exclui [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49dae-106">Deletes a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49dae-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49dae-107">Prerequisites</span></span>
<span data-ttu-id="49dae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49dae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49dae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49dae-110">Permission type</span></span>|<span data-ttu-id="49dae-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49dae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49dae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49dae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49dae-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49dae-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49dae-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49dae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49dae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49dae-115">Not supported.</span></span>|
|<span data-ttu-id="49dae-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49dae-116">Application</span></span>|<span data-ttu-id="49dae-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49dae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49dae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49dae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="49dae-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49dae-119">Request headers</span></span>
|<span data-ttu-id="49dae-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49dae-120">Header</span></span>|<span data-ttu-id="49dae-121">Valor</span><span class="sxs-lookup"><span data-stu-id="49dae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49dae-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="49dae-122">Authorization</span></span>|<span data-ttu-id="49dae-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49dae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49dae-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49dae-124">Accept</span></span>|<span data-ttu-id="49dae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49dae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49dae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49dae-126">Request body</span></span>
<span data-ttu-id="49dae-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49dae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49dae-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="49dae-128">Response</span></span>
<span data-ttu-id="49dae-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="49dae-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="49dae-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49dae-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="49dae-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49dae-131">Request</span></span>
<span data-ttu-id="49dae-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49dae-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="49dae-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="49dae-133">Response</span></span>
<span data-ttu-id="49dae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49dae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





