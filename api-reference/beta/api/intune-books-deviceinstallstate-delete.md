---
title: Excluir deviceInstallState
description: Exclui deviceInstallState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 161042a36068a9f9b4a4224f49e54c9485709bea
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48716954"
---
# <a name="delete-deviceinstallstate"></a><span data-ttu-id="d0449-103">Excluir deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="d0449-103">Delete deviceInstallState</span></span>

<span data-ttu-id="d0449-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0449-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0449-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d0449-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0449-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0449-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0449-107">Exclui [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="d0449-107">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0449-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d0449-108">Prerequisites</span></span>
<span data-ttu-id="d0449-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0449-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0449-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0449-111">Permission type</span></span>|<span data-ttu-id="d0449-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d0449-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0449-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0449-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0449-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0449-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d0449-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0449-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0449-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0449-116">Not supported.</span></span>|
|<span data-ttu-id="d0449-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0449-117">Application</span></span>|<span data-ttu-id="d0449-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0449-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0449-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0449-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="d0449-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0449-120">Request headers</span></span>
|<span data-ttu-id="d0449-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0449-121">Header</span></span>|<span data-ttu-id="d0449-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d0449-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0449-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0449-123">Authorization</span></span>|<span data-ttu-id="d0449-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0449-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0449-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d0449-125">Accept</span></span>|<span data-ttu-id="d0449-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0449-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0449-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0449-127">Request body</span></span>
<span data-ttu-id="d0449-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0449-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0449-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0449-129">Response</span></span>
<span data-ttu-id="d0449-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d0449-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d0449-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0449-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0449-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0449-132">Request</span></span>
<span data-ttu-id="d0449-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0449-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="d0449-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0449-134">Response</span></span>
<span data-ttu-id="d0449-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0449-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





