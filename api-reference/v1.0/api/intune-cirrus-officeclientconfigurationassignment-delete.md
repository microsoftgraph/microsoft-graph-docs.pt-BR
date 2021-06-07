---
title: Excluir officeClientConfigurationAssignment
description: Exclui um officeClientConfigurationAssignment.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4e65a21e402c261d57dd33dcf880aa564d886f9c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752931"
---
# <a name="delete-officeclientconfigurationassignment"></a><span data-ttu-id="31052-103">Excluir officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="31052-103">Delete officeClientConfigurationAssignment</span></span>

<span data-ttu-id="31052-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31052-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31052-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31052-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31052-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31052-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31052-107">Exclui um [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31052-107">Deletes a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31052-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="31052-108">Prerequisites</span></span>
<span data-ttu-id="31052-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31052-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31052-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31052-111">Permission type</span></span>|<span data-ttu-id="31052-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="31052-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31052-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31052-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31052-114">\*\*TODO: Determinar escopos \*\*</span><span class="sxs-lookup"><span data-stu-id="31052-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="31052-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31052-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31052-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31052-116">Not supported.</span></span>|
|<span data-ttu-id="31052-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31052-117">Application</span></span>|<span data-ttu-id="31052-118">\*\*TODO: Determinar escopos \*\*</span><span class="sxs-lookup"><span data-stu-id="31052-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="31052-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31052-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="31052-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31052-120">Request headers</span></span>
|<span data-ttu-id="31052-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31052-121">Header</span></span>|<span data-ttu-id="31052-122">Valor</span><span class="sxs-lookup"><span data-stu-id="31052-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31052-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="31052-123">Authorization</span></span>|<span data-ttu-id="31052-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31052-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31052-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="31052-125">Accept</span></span>|<span data-ttu-id="31052-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31052-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31052-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31052-127">Request body</span></span>
<span data-ttu-id="31052-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31052-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31052-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="31052-129">Response</span></span>
<span data-ttu-id="31052-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="31052-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="31052-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31052-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="31052-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31052-132">Request</span></span>
<span data-ttu-id="31052-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31052-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="31052-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="31052-134">Response</span></span>
<span data-ttu-id="31052-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31052-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




