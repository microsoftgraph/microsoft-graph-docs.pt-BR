---
title: Excluir windowsDomainJoinConfiguration
description: Exclui um windowsDomainJoinConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1d99fd2971efb3330d370af6cad99b8137f689ce
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866955"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="8f2f4-103">Excluir windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="8f2f4-103">Delete windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="8f2f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f2f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f2f4-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8f2f4-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8f2f4-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8f2f4-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f2f4-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8f2f4-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f2f4-108">Exclui um [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f2f4-108">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f2f4-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8f2f4-109">Prerequisites</span></span>
<span data-ttu-id="8f2f4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f2f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f2f4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f2f4-112">Permission type</span></span>|<span data-ttu-id="8f2f4-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8f2f4-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f2f4-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f2f4-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8f2f4-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="8f2f4-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8f2f4-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f2f4-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="8f2f4-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f2f4-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f2f4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f2f4-118">Not supported.</span></span>|
|<span data-ttu-id="8f2f4-119">Application</span><span class="sxs-lookup"><span data-stu-id="8f2f4-119">Application</span></span>||
| <span data-ttu-id="8f2f4-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="8f2f4-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8f2f4-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f2f4-121">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f2f4-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f2f4-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8f2f4-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f2f4-123">Request headers</span></span>
|<span data-ttu-id="8f2f4-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f2f4-124">Header</span></span>|<span data-ttu-id="8f2f4-125">Valor</span><span class="sxs-lookup"><span data-stu-id="8f2f4-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f2f4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f2f4-126">Authorization</span></span>|<span data-ttu-id="8f2f4-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f2f4-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f2f4-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8f2f4-128">Accept</span></span>|<span data-ttu-id="8f2f4-129">application/json</span><span class="sxs-lookup"><span data-stu-id="8f2f4-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f2f4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f2f4-130">Request body</span></span>
<span data-ttu-id="8f2f4-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f2f4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f2f4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f2f4-132">Response</span></span>
<span data-ttu-id="8f2f4-133">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8f2f4-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8f2f4-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f2f4-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f2f4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f2f4-135">Request</span></span>
<span data-ttu-id="8f2f4-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f2f4-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8f2f4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f2f4-137">Response</span></span>
<span data-ttu-id="8f2f4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f2f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```










