---
title: Excluir sharedPCConfiguration
description: Exclui sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 425e0baf42a2955f6c6e445b587f5ff86155b5e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518167"
---
# <a name="delete-sharedpcconfiguration"></a><span data-ttu-id="8ff21-103">Excluir sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ff21-103">Delete sharedPCConfiguration</span></span>

> <span data-ttu-id="8ff21-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8ff21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ff21-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ff21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ff21-106">Exclui [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff21-106">Deletes a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ff21-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ff21-107">Prerequisites</span></span>
<span data-ttu-id="8ff21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ff21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ff21-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ff21-110">Permission type</span></span>|<span data-ttu-id="8ff21-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8ff21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ff21-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ff21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8ff21-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff21-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ff21-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ff21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ff21-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ff21-115">Not supported.</span></span>|
|<span data-ttu-id="8ff21-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ff21-116">Application</span></span>|<span data-ttu-id="8ff21-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ff21-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ff21-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ff21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8ff21-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff21-119">Request headers</span></span>
|<span data-ttu-id="8ff21-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ff21-120">Header</span></span>|<span data-ttu-id="8ff21-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8ff21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ff21-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ff21-122">Authorization</span></span>|<span data-ttu-id="8ff21-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ff21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ff21-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8ff21-124">Accept</span></span>|<span data-ttu-id="8ff21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8ff21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ff21-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff21-126">Request body</span></span>
<span data-ttu-id="8ff21-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ff21-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ff21-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff21-128">Response</span></span>
<span data-ttu-id="8ff21-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8ff21-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8ff21-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ff21-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ff21-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff21-131">Request</span></span>
<span data-ttu-id="8ff21-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ff21-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8ff21-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff21-133">Response</span></span>
<span data-ttu-id="8ff21-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ff21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





