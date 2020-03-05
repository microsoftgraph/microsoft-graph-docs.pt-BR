---
title: Excluir groupPolicyPresentationValueList
description: Exclui groupPolicyPresentationValueList.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: baa184e79ff956a193627532dbb46cf694f3b406
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464250"
---
# <a name="delete-grouppolicypresentationvaluelist"></a><span data-ttu-id="acecf-103">Excluir groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="acecf-103">Delete groupPolicyPresentationValueList</span></span>

<span data-ttu-id="acecf-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="acecf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="acecf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="acecf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="acecf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="acecf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acecf-107">Exclui [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span><span class="sxs-lookup"><span data-stu-id="acecf-107">Deletes a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acecf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="acecf-108">Prerequisites</span></span>
<span data-ttu-id="acecf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acecf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acecf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="acecf-111">Permission type</span></span>|<span data-ttu-id="acecf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="acecf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acecf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="acecf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="acecf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acecf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="acecf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="acecf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acecf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acecf-116">Not supported.</span></span>|
|<span data-ttu-id="acecf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="acecf-117">Application</span></span>|<span data-ttu-id="acecf-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acecf-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="acecf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="acecf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="acecf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="acecf-120">Request headers</span></span>
|<span data-ttu-id="acecf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="acecf-121">Header</span></span>|<span data-ttu-id="acecf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="acecf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acecf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="acecf-123">Authorization</span></span>|<span data-ttu-id="acecf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="acecf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acecf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="acecf-125">Accept</span></span>|<span data-ttu-id="acecf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="acecf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acecf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="acecf-127">Request body</span></span>
<span data-ttu-id="acecf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="acecf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acecf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="acecf-129">Response</span></span>
<span data-ttu-id="acecf-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="acecf-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="acecf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="acecf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="acecf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="acecf-132">Request</span></span>
<span data-ttu-id="acecf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="acecf-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="acecf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="acecf-134">Response</span></span>
<span data-ttu-id="acecf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="acecf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





