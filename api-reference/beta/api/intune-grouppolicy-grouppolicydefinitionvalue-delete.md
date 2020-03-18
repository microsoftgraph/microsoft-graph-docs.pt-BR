---
title: Excluir groupPolicyDefinitionValue
description: Exclui groupPolicyDefinitionValue.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 789df517610a5dae5e618b3d5329f93cedb5ed07
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804398"
---
# <a name="delete-grouppolicydefinitionvalue"></a><span data-ttu-id="2f3ab-103">Excluir groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="2f3ab-103">Delete groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="2f3ab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f3ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f3ab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f3ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f3ab-106">Exclui [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span><span class="sxs-lookup"><span data-stu-id="2f3ab-106">Deletes a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f3ab-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f3ab-107">Prerequisites</span></span>
<span data-ttu-id="2f3ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f3ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f3ab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f3ab-110">Permission type</span></span>|<span data-ttu-id="2f3ab-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f3ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f3ab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f3ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f3ab-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f3ab-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2f3ab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f3ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f3ab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f3ab-115">Not supported.</span></span>|
|<span data-ttu-id="2f3ab-116">Application</span><span class="sxs-lookup"><span data-stu-id="2f3ab-116">Application</span></span>|<span data-ttu-id="2f3ab-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f3ab-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f3ab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f3ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="2f3ab-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f3ab-119">Request headers</span></span>
|<span data-ttu-id="2f3ab-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f3ab-120">Header</span></span>|<span data-ttu-id="2f3ab-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2f3ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f3ab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f3ab-122">Authorization</span></span>|<span data-ttu-id="2f3ab-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f3ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f3ab-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f3ab-124">Accept</span></span>|<span data-ttu-id="2f3ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f3ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f3ab-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f3ab-126">Request body</span></span>
<span data-ttu-id="2f3ab-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f3ab-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f3ab-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f3ab-128">Response</span></span>
<span data-ttu-id="2f3ab-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2f3ab-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2f3ab-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f3ab-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f3ab-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f3ab-131">Request</span></span>
<span data-ttu-id="2f3ab-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f3ab-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
```

### <a name="response"></a><span data-ttu-id="2f3ab-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f3ab-133">Response</span></span>
<span data-ttu-id="2f3ab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f3ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




