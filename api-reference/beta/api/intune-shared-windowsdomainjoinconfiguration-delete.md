---
title: Excluir windowsDomainJoinConfiguration
description: Exclui windowsDomainJoinConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af184a56a2391e8fb76cfa61ece292a9fa8af2f2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979523"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="0be37-103">Excluir windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="0be37-103">Delete windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="0be37-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0be37-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0be37-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0be37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0be37-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0be37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0be37-107">Exclui [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0be37-107">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0be37-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0be37-108">Prerequisites</span></span>
<span data-ttu-id="0be37-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0be37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0be37-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0be37-111">Permission type</span></span>|<span data-ttu-id="0be37-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0be37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0be37-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0be37-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0be37-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0be37-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="0be37-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be37-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="0be37-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0be37-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0be37-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0be37-117">Not supported.</span></span>|
|<span data-ttu-id="0be37-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0be37-118">Application</span></span>|<span data-ttu-id="0be37-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0be37-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0be37-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0be37-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0be37-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0be37-121">Request headers</span></span>
|<span data-ttu-id="0be37-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0be37-122">Header</span></span>|<span data-ttu-id="0be37-123">Valor</span><span class="sxs-lookup"><span data-stu-id="0be37-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0be37-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0be37-124">Authorization</span></span>|<span data-ttu-id="0be37-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0be37-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0be37-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0be37-126">Accept</span></span>|<span data-ttu-id="0be37-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0be37-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0be37-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0be37-128">Request body</span></span>
<span data-ttu-id="0be37-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0be37-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0be37-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0be37-130">Response</span></span>
<span data-ttu-id="0be37-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0be37-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0be37-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0be37-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="0be37-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0be37-133">Request</span></span>
<span data-ttu-id="0be37-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0be37-134">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0be37-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0be37-135">Response</span></span>
<span data-ttu-id="0be37-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0be37-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



