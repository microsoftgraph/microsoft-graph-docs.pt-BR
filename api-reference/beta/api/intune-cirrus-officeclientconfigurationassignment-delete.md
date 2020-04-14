---
title: Excluir officeClientConfigurationAssignment
description: Exclui officeClientConfigurationAssignment.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e6a01d70bcd0a49bfe060d075e7e28a1d17353a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43391995"
---
# <a name="delete-officeclientconfigurationassignment"></a><span data-ttu-id="47bbf-103">Excluir officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="47bbf-103">Delete officeClientConfigurationAssignment</span></span>

<span data-ttu-id="47bbf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47bbf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47bbf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47bbf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47bbf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47bbf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47bbf-107">Exclui [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="47bbf-107">Deletes a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47bbf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47bbf-108">Prerequisites</span></span>
<span data-ttu-id="47bbf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47bbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47bbf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47bbf-111">Permission type</span></span>|<span data-ttu-id="47bbf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47bbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47bbf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47bbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47bbf-114">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="47bbf-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="47bbf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47bbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47bbf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47bbf-116">Not supported.</span></span>|
|<span data-ttu-id="47bbf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47bbf-117">Application</span></span>|<span data-ttu-id="47bbf-118">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="47bbf-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="47bbf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47bbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="47bbf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47bbf-120">Request headers</span></span>
|<span data-ttu-id="47bbf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47bbf-121">Header</span></span>|<span data-ttu-id="47bbf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="47bbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47bbf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="47bbf-123">Authorization</span></span>|<span data-ttu-id="47bbf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47bbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47bbf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47bbf-125">Accept</span></span>|<span data-ttu-id="47bbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47bbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47bbf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47bbf-127">Request body</span></span>
<span data-ttu-id="47bbf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47bbf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47bbf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="47bbf-129">Response</span></span>
<span data-ttu-id="47bbf-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="47bbf-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="47bbf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47bbf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="47bbf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47bbf-132">Request</span></span>
<span data-ttu-id="47bbf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47bbf-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="47bbf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="47bbf-134">Response</span></span>
<span data-ttu-id="47bbf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47bbf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



