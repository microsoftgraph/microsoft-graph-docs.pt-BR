---
title: Excluir Propriedadesdeviceconfigurationconflictsummary
description: Exclui Propriedadesdeviceconfigurationconflictsummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fa33a5f9e77c5d8291b2d69fe53d72a5fc65e1e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927570"
---
# <a name="delete-deviceconfigurationconflictsummary"></a><span data-ttu-id="d69d3-103">Excluir Propriedadesdeviceconfigurationconflictsummary</span><span class="sxs-lookup"><span data-stu-id="d69d3-103">Delete deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="d69d3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d69d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d69d3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d69d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d69d3-106">Exclui [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="d69d3-106">Deletes a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d69d3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d69d3-107">Prerequisites</span></span>
<span data-ttu-id="d69d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d69d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d69d3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d69d3-110">Permission type</span></span>|<span data-ttu-id="d69d3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d69d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d69d3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d69d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d69d3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d69d3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d69d3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d69d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d69d3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d69d3-115">Not supported.</span></span>|
|<span data-ttu-id="d69d3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d69d3-116">Application</span></span>|<span data-ttu-id="d69d3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d69d3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d69d3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d69d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="d69d3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d69d3-119">Request headers</span></span>
|<span data-ttu-id="d69d3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d69d3-120">Header</span></span>|<span data-ttu-id="d69d3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d69d3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d69d3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d69d3-122">Authorization</span></span>|<span data-ttu-id="d69d3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d69d3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d69d3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d69d3-124">Accept</span></span>|<span data-ttu-id="d69d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d69d3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d69d3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d69d3-126">Request body</span></span>
<span data-ttu-id="d69d3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d69d3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d69d3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d69d3-128">Response</span></span>
<span data-ttu-id="d69d3-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d69d3-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d69d3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d69d3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d69d3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d69d3-131">Request</span></span>
<span data-ttu-id="d69d3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d69d3-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

### <a name="response"></a><span data-ttu-id="d69d3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d69d3-133">Response</span></span>
<span data-ttu-id="d69d3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d69d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




