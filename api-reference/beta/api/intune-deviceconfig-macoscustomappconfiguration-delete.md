---
title: Excluir macOSCustomAppConfiguration
description: Exclui um macOSCustomAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b03609db6c2aad52215f3a3a2cd40ac288ef197
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137319"
---
# <a name="delete-macoscustomappconfiguration"></a><span data-ttu-id="cd625-103">Excluir macOSCustomAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd625-103">Delete macOSCustomAppConfiguration</span></span>

<span data-ttu-id="cd625-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd625-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd625-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cd625-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd625-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cd625-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd625-107">Exclui um [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd625-107">Deletes a [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd625-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cd625-108">Prerequisites</span></span>
<span data-ttu-id="cd625-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd625-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd625-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd625-111">Permission type</span></span>|<span data-ttu-id="cd625-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd625-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd625-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd625-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cd625-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd625-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cd625-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd625-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd625-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd625-116">Not supported.</span></span>|
|<span data-ttu-id="cd625-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd625-117">Application</span></span>|<span data-ttu-id="cd625-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd625-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd625-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd625-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cd625-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd625-120">Request headers</span></span>
|<span data-ttu-id="cd625-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd625-121">Header</span></span>|<span data-ttu-id="cd625-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cd625-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd625-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd625-123">Authorization</span></span>|<span data-ttu-id="cd625-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd625-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd625-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cd625-125">Accept</span></span>|<span data-ttu-id="cd625-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cd625-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd625-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd625-127">Request body</span></span>
<span data-ttu-id="cd625-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cd625-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd625-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd625-129">Response</span></span>
<span data-ttu-id="cd625-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cd625-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cd625-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd625-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd625-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd625-132">Request</span></span>
<span data-ttu-id="cd625-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd625-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="cd625-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd625-134">Response</span></span>
<span data-ttu-id="cd625-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd625-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




