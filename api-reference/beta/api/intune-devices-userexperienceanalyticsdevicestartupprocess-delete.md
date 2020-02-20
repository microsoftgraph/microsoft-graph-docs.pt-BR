---
title: Excluir userExperienceAnalyticsDeviceStartupProcess
description: Exclui userExperienceAnalyticsDeviceStartupProcess.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5cb35e518c619df5f1e0ccfaacd46951d9d373d9
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161998"
---
# <a name="delete-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="f1255-103">Excluir userExperienceAnalyticsDeviceStartupProcess</span><span class="sxs-lookup"><span data-stu-id="f1255-103">Delete userExperienceAnalyticsDeviceStartupProcess</span></span>

> <span data-ttu-id="f1255-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f1255-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1255-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1255-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1255-106">Exclui [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span><span class="sxs-lookup"><span data-stu-id="f1255-106">Deletes a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1255-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1255-107">Prerequisites</span></span>
<span data-ttu-id="f1255-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1255-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1255-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1255-110">Permission type</span></span>|<span data-ttu-id="f1255-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1255-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1255-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1255-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1255-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1255-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f1255-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1255-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1255-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1255-115">Not supported.</span></span>|
|<span data-ttu-id="f1255-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1255-116">Application</span></span>|<span data-ttu-id="f1255-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1255-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1255-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1255-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

## <a name="request-headers"></a><span data-ttu-id="f1255-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1255-119">Request headers</span></span>
|<span data-ttu-id="f1255-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1255-120">Header</span></span>|<span data-ttu-id="f1255-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f1255-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1255-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1255-122">Authorization</span></span>|<span data-ttu-id="f1255-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1255-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1255-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1255-124">Accept</span></span>|<span data-ttu-id="f1255-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1255-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1255-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1255-126">Request body</span></span>
<span data-ttu-id="f1255-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1255-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1255-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1255-128">Response</span></span>
<span data-ttu-id="f1255-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f1255-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f1255-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1255-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1255-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1255-131">Request</span></span>
<span data-ttu-id="f1255-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1255-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

### <a name="response"></a><span data-ttu-id="f1255-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1255-133">Response</span></span>
<span data-ttu-id="f1255-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1255-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





