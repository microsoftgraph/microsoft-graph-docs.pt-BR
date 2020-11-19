---
title: Excluir groupPolicyPresentationLongDecimalTextBox
description: Exclui groupPolicyPresentationLongDecimalTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1e08564e431666bf9b7fd46cc728cc049ba0ef11
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49225121"
---
# <a name="delete-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="45b53-103">Excluir groupPolicyPresentationLongDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="45b53-103">Delete groupPolicyPresentationLongDecimalTextBox</span></span>

<span data-ttu-id="45b53-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45b53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45b53-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45b53-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45b53-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45b53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45b53-107">Exclui [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span><span class="sxs-lookup"><span data-stu-id="45b53-107">Deletes a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45b53-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45b53-108">Prerequisites</span></span>
<span data-ttu-id="45b53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45b53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45b53-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45b53-111">Permission type</span></span>|<span data-ttu-id="45b53-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45b53-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45b53-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45b53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45b53-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45b53-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45b53-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45b53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45b53-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45b53-116">Not supported.</span></span>|
|<span data-ttu-id="45b53-117">Application</span><span class="sxs-lookup"><span data-stu-id="45b53-117">Application</span></span>|<span data-ttu-id="45b53-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45b53-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45b53-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45b53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="45b53-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45b53-120">Request headers</span></span>
|<span data-ttu-id="45b53-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45b53-121">Header</span></span>|<span data-ttu-id="45b53-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45b53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45b53-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45b53-123">Authorization</span></span>|<span data-ttu-id="45b53-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45b53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45b53-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45b53-125">Accept</span></span>|<span data-ttu-id="45b53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45b53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45b53-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45b53-127">Request body</span></span>
<span data-ttu-id="45b53-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45b53-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45b53-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="45b53-129">Response</span></span>
<span data-ttu-id="45b53-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="45b53-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="45b53-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45b53-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="45b53-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45b53-132">Request</span></span>
<span data-ttu-id="45b53-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45b53-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="45b53-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="45b53-134">Response</span></span>
<span data-ttu-id="45b53-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45b53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




