---
title: Excluir windowsDomainJoinConfiguration
description: Exclui windowsDomainJoinConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e5cb9759f0a60a371695b4f077e5220d248b1b5b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536837"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="3c47a-103">Excluir windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="3c47a-103">Delete windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="3c47a-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3c47a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3c47a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3c47a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c47a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c47a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c47a-107">Exclui [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c47a-107">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c47a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c47a-108">Prerequisites</span></span>
<span data-ttu-id="3c47a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c47a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c47a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c47a-111">Permission type</span></span>|<span data-ttu-id="3c47a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c47a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c47a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c47a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3c47a-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="3c47a-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3c47a-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c47a-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="3c47a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c47a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c47a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c47a-117">Not supported.</span></span>|
|<span data-ttu-id="3c47a-118">Application</span><span class="sxs-lookup"><span data-stu-id="3c47a-118">Application</span></span>||
| <span data-ttu-id="3c47a-119">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="3c47a-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3c47a-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c47a-120">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c47a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c47a-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3c47a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c47a-122">Request headers</span></span>
|<span data-ttu-id="3c47a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c47a-123">Header</span></span>|<span data-ttu-id="3c47a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3c47a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c47a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c47a-125">Authorization</span></span>|<span data-ttu-id="3c47a-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c47a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c47a-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c47a-127">Accept</span></span>|<span data-ttu-id="3c47a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3c47a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c47a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c47a-129">Request body</span></span>
<span data-ttu-id="3c47a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c47a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c47a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c47a-131">Response</span></span>
<span data-ttu-id="3c47a-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3c47a-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3c47a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c47a-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c47a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c47a-134">Request</span></span>
<span data-ttu-id="3c47a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c47a-135">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3c47a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c47a-136">Response</span></span>
<span data-ttu-id="3c47a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c47a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









