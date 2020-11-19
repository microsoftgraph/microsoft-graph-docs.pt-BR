---
title: Excluir windowsDefenderAdvancedThreatProtectionConfiguration
description: Exclui windowsDefenderAdvancedThreatProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2ebf4796732e21b90e7763c70aeacbd466eac8a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49235879"
---
# <a name="delete-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="d6b68-103">Excluir windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="d6b68-103">Delete windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

<span data-ttu-id="d6b68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6b68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6b68-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6b68-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6b68-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6b68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6b68-107">Exclui [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6b68-107">Deletes a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6b68-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6b68-108">Prerequisites</span></span>
<span data-ttu-id="d6b68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6b68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6b68-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6b68-111">Permission type</span></span>|<span data-ttu-id="d6b68-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6b68-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6b68-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6b68-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6b68-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6b68-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6b68-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6b68-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6b68-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6b68-116">Not supported.</span></span>|
|<span data-ttu-id="d6b68-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6b68-117">Application</span></span>|<span data-ttu-id="d6b68-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6b68-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6b68-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6b68-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d6b68-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6b68-120">Request headers</span></span>
|<span data-ttu-id="d6b68-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6b68-121">Header</span></span>|<span data-ttu-id="d6b68-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d6b68-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6b68-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6b68-123">Authorization</span></span>|<span data-ttu-id="d6b68-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6b68-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6b68-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6b68-125">Accept</span></span>|<span data-ttu-id="d6b68-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6b68-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6b68-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6b68-127">Request body</span></span>
<span data-ttu-id="d6b68-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6b68-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6b68-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6b68-129">Response</span></span>
<span data-ttu-id="d6b68-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d6b68-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d6b68-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6b68-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6b68-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6b68-132">Request</span></span>
<span data-ttu-id="d6b68-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6b68-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d6b68-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6b68-134">Response</span></span>
<span data-ttu-id="d6b68-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6b68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




