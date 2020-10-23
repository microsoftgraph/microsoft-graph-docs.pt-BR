---
title: Excluir windowsDomainJoinConfiguration
description: Exclui windowsDomainJoinConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 019c8e273c29321b54308c2e7a7fa65d6ccc9877
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702793"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="50425-103">Excluir windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="50425-103">Delete windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="50425-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50425-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50425-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="50425-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="50425-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="50425-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50425-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50425-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50425-108">Exclui [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50425-108">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50425-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50425-109">Prerequisites</span></span>
<span data-ttu-id="50425-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50425-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50425-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50425-112">Permission type</span></span>|<span data-ttu-id="50425-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50425-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50425-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50425-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="50425-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="50425-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="50425-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50425-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="50425-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50425-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50425-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50425-118">Not supported.</span></span>|
|<span data-ttu-id="50425-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50425-119">Application</span></span>||
| <span data-ttu-id="50425-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="50425-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="50425-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50425-121">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50425-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50425-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="50425-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50425-123">Request headers</span></span>
|<span data-ttu-id="50425-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50425-124">Header</span></span>|<span data-ttu-id="50425-125">Valor</span><span class="sxs-lookup"><span data-stu-id="50425-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50425-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="50425-126">Authorization</span></span>|<span data-ttu-id="50425-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50425-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50425-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50425-128">Accept</span></span>|<span data-ttu-id="50425-129">application/json</span><span class="sxs-lookup"><span data-stu-id="50425-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50425-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50425-130">Request body</span></span>
<span data-ttu-id="50425-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50425-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50425-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="50425-132">Response</span></span>
<span data-ttu-id="50425-133">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="50425-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="50425-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50425-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="50425-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50425-135">Request</span></span>
<span data-ttu-id="50425-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50425-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="50425-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="50425-137">Response</span></span>
<span data-ttu-id="50425-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50425-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```











