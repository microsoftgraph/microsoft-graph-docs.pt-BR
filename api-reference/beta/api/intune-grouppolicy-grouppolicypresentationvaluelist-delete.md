---
title: Excluir groupPolicyPresentationValueList
description: Exclui groupPolicyPresentationValueList.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26400b504c4a6f1e5fa98f8adf02ed63b19c558c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734326"
---
# <a name="delete-grouppolicypresentationvaluelist"></a><span data-ttu-id="8a9dc-103">Excluir groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="8a9dc-103">Delete groupPolicyPresentationValueList</span></span>

<span data-ttu-id="8a9dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a9dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a9dc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8a9dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a9dc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8a9dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a9dc-107">Exclui [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span><span class="sxs-lookup"><span data-stu-id="8a9dc-107">Deletes a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a9dc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a9dc-108">Prerequisites</span></span>
<span data-ttu-id="8a9dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a9dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a9dc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a9dc-111">Permission type</span></span>|<span data-ttu-id="8a9dc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8a9dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a9dc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a9dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a9dc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a9dc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8a9dc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a9dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a9dc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a9dc-116">Not supported.</span></span>|
|<span data-ttu-id="8a9dc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a9dc-117">Application</span></span>|<span data-ttu-id="8a9dc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a9dc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a9dc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a9dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="8a9dc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a9dc-120">Request headers</span></span>
|<span data-ttu-id="8a9dc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a9dc-121">Header</span></span>|<span data-ttu-id="8a9dc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8a9dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a9dc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a9dc-123">Authorization</span></span>|<span data-ttu-id="8a9dc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a9dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a9dc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8a9dc-125">Accept</span></span>|<span data-ttu-id="8a9dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a9dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a9dc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a9dc-127">Request body</span></span>
<span data-ttu-id="8a9dc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a9dc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a9dc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a9dc-129">Response</span></span>
<span data-ttu-id="8a9dc-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8a9dc-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8a9dc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a9dc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a9dc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a9dc-132">Request</span></span>
<span data-ttu-id="8a9dc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a9dc-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="8a9dc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a9dc-134">Response</span></span>
<span data-ttu-id="8a9dc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a9dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





