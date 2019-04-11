---
title: Excluir groupPolicyDefinitionValue
description: Exclui groupPolicyDefinitionValue.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09b1a22933e48318dfa19342bbc0d3a51cde04d3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782251"
---
# <a name="delete-grouppolicydefinitionvalue"></a><span data-ttu-id="5f287-103">Excluir groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="5f287-103">Delete groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="5f287-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5f287-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f287-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f287-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f287-106">Exclui [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span><span class="sxs-lookup"><span data-stu-id="5f287-106">Deletes a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f287-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5f287-107">Prerequisites</span></span>
<span data-ttu-id="5f287-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f287-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f287-110">Permission type</span></span>|<span data-ttu-id="5f287-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5f287-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f287-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f287-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f287-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f287-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5f287-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f287-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f287-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f287-115">Not supported.</span></span>|
|<span data-ttu-id="5f287-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f287-116">Application</span></span>|<span data-ttu-id="5f287-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f287-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f287-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f287-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="5f287-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f287-119">Request headers</span></span>
|<span data-ttu-id="5f287-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f287-120">Header</span></span>|<span data-ttu-id="5f287-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5f287-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f287-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f287-122">Authorization</span></span>|<span data-ttu-id="5f287-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f287-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f287-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5f287-124">Accept</span></span>|<span data-ttu-id="5f287-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f287-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f287-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f287-126">Request body</span></span>
<span data-ttu-id="5f287-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f287-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f287-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f287-128">Response</span></span>
<span data-ttu-id="5f287-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5f287-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5f287-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f287-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f287-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f287-131">Request</span></span>
<span data-ttu-id="5f287-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f287-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
```

### <a name="response"></a><span data-ttu-id="5f287-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f287-133">Response</span></span>
<span data-ttu-id="5f287-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f287-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





