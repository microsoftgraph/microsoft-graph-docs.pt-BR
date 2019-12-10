---
title: Excluir windowsAutopilotDeploymentProfilePolicySetItem
description: Exclui windowsAutopilotDeploymentProfilePolicySetItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb01deb318cb163c6cec997a686febe127639756
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940809"
---
# <a name="delete-windowsautopilotdeploymentprofilepolicysetitem"></a><span data-ttu-id="1cfdf-103">Excluir windowsAutopilotDeploymentProfilePolicySetItem</span><span class="sxs-lookup"><span data-stu-id="1cfdf-103">Delete windowsAutopilotDeploymentProfilePolicySetItem</span></span>

> <span data-ttu-id="1cfdf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1cfdf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cfdf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1cfdf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cfdf-106">Exclui [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="1cfdf-106">Deletes a [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1cfdf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1cfdf-107">Prerequisites</span></span>
<span data-ttu-id="1cfdf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cfdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cfdf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cfdf-110">Permission type</span></span>|<span data-ttu-id="1cfdf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1cfdf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cfdf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cfdf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1cfdf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cfdf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1cfdf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cfdf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cfdf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cfdf-115">Not supported.</span></span>|
|<span data-ttu-id="1cfdf-116">Application</span><span class="sxs-lookup"><span data-stu-id="1cfdf-116">Application</span></span>|<span data-ttu-id="1cfdf-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cfdf-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cfdf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cfdf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="1cfdf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cfdf-119">Request headers</span></span>
|<span data-ttu-id="1cfdf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1cfdf-120">Header</span></span>|<span data-ttu-id="1cfdf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1cfdf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cfdf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cfdf-122">Authorization</span></span>|<span data-ttu-id="1cfdf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cfdf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cfdf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1cfdf-124">Accept</span></span>|<span data-ttu-id="1cfdf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1cfdf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cfdf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cfdf-126">Request body</span></span>
<span data-ttu-id="1cfdf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1cfdf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cfdf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cfdf-128">Response</span></span>
<span data-ttu-id="1cfdf-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1cfdf-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1cfdf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1cfdf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cfdf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cfdf-131">Request</span></span>
<span data-ttu-id="1cfdf-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cfdf-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="1cfdf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cfdf-133">Response</span></span>
<span data-ttu-id="1cfdf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1cfdf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





