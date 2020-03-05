---
title: Excluir windowsPhone81VpnConfiguration
description: Exclui windowsPhone81VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ff642555da1dd7b6e65f5c693dafb6cb29cfc9e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42474253"
---
# <a name="delete-windowsphone81vpnconfiguration"></a><span data-ttu-id="b60db-103">Excluir windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b60db-103">Delete windowsPhone81VpnConfiguration</span></span>

<span data-ttu-id="b60db-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b60db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b60db-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b60db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b60db-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b60db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b60db-107">Exclui [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b60db-107">Deletes a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b60db-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b60db-108">Prerequisites</span></span>
<span data-ttu-id="b60db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b60db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b60db-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b60db-111">Permission type</span></span>|<span data-ttu-id="b60db-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b60db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b60db-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b60db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b60db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b60db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b60db-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b60db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b60db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b60db-116">Not supported.</span></span>|
|<span data-ttu-id="b60db-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b60db-117">Application</span></span>|<span data-ttu-id="b60db-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b60db-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b60db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b60db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b60db-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b60db-120">Request headers</span></span>
|<span data-ttu-id="b60db-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b60db-121">Header</span></span>|<span data-ttu-id="b60db-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b60db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b60db-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b60db-123">Authorization</span></span>|<span data-ttu-id="b60db-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b60db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b60db-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b60db-125">Accept</span></span>|<span data-ttu-id="b60db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b60db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b60db-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b60db-127">Request body</span></span>
<span data-ttu-id="b60db-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b60db-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b60db-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b60db-129">Response</span></span>
<span data-ttu-id="b60db-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b60db-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b60db-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b60db-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b60db-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b60db-132">Request</span></span>
<span data-ttu-id="b60db-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b60db-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b60db-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b60db-134">Response</span></span>
<span data-ttu-id="b60db-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b60db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





