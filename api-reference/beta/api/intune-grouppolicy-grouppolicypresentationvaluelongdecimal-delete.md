---
title: Excluir groupPolicyPresentationValueLongDecimal
description: Exclui groupPolicyPresentationValueLongDecimal.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a76d47f0b1f4b55d76631d6f2fd618ac1539e59c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460239"
---
# <a name="delete-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="c0db4-103">Excluir groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="c0db4-103">Delete groupPolicyPresentationValueLongDecimal</span></span>

<span data-ttu-id="c0db4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0db4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0db4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0db4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0db4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0db4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0db4-107">Exclui [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span><span class="sxs-lookup"><span data-stu-id="c0db4-107">Deletes a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0db4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0db4-108">Prerequisites</span></span>
<span data-ttu-id="c0db4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0db4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0db4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0db4-111">Permission type</span></span>|<span data-ttu-id="c0db4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0db4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0db4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0db4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0db4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0db4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0db4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0db4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0db4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0db4-116">Not supported.</span></span>|
|<span data-ttu-id="c0db4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0db4-117">Application</span></span>|<span data-ttu-id="c0db4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0db4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0db4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0db4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="c0db4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0db4-120">Request headers</span></span>
|<span data-ttu-id="c0db4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0db4-121">Header</span></span>|<span data-ttu-id="c0db4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c0db4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0db4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0db4-123">Authorization</span></span>|<span data-ttu-id="c0db4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0db4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0db4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0db4-125">Accept</span></span>|<span data-ttu-id="c0db4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0db4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0db4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0db4-127">Request body</span></span>
<span data-ttu-id="c0db4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0db4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0db4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0db4-129">Response</span></span>
<span data-ttu-id="c0db4-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c0db4-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c0db4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0db4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0db4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0db4-132">Request</span></span>
<span data-ttu-id="c0db4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0db4-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="c0db4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0db4-134">Response</span></span>
<span data-ttu-id="c0db4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0db4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



