---
title: Excluir groupPolicyPresentationMultiTextBox
description: Exclui um groupPolicyPresentationMultiTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aef397fd2f179af4a737401d6a163c618eab8300
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153241"
---
# <a name="delete-grouppolicypresentationmultitextbox"></a><span data-ttu-id="30fbb-103">Excluir groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="30fbb-103">Delete groupPolicyPresentationMultiTextBox</span></span>

<span data-ttu-id="30fbb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30fbb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30fbb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="30fbb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30fbb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30fbb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30fbb-107">Exclui um [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span><span class="sxs-lookup"><span data-stu-id="30fbb-107">Deletes a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30fbb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30fbb-108">Prerequisites</span></span>
<span data-ttu-id="30fbb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30fbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30fbb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30fbb-111">Permission type</span></span>|<span data-ttu-id="30fbb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30fbb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30fbb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30fbb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30fbb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30fbb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="30fbb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30fbb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30fbb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30fbb-116">Not supported.</span></span>|
|<span data-ttu-id="30fbb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30fbb-117">Application</span></span>|<span data-ttu-id="30fbb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30fbb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30fbb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30fbb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="30fbb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30fbb-120">Request headers</span></span>
|<span data-ttu-id="30fbb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30fbb-121">Header</span></span>|<span data-ttu-id="30fbb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="30fbb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30fbb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="30fbb-123">Authorization</span></span>|<span data-ttu-id="30fbb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30fbb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30fbb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30fbb-125">Accept</span></span>|<span data-ttu-id="30fbb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30fbb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30fbb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30fbb-127">Request body</span></span>
<span data-ttu-id="30fbb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30fbb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30fbb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="30fbb-129">Response</span></span>
<span data-ttu-id="30fbb-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="30fbb-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="30fbb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30fbb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="30fbb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30fbb-132">Request</span></span>
<span data-ttu-id="30fbb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30fbb-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="30fbb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="30fbb-134">Response</span></span>
<span data-ttu-id="30fbb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30fbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




