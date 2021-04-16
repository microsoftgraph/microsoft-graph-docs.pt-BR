---
title: Excluir deviceManagementReusablePolicySetting
description: Exclui um deviceManagementReusablePolicySetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca16a5e1f980ffdea6e797fd2868110bb6a68927
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868373"
---
# <a name="delete-devicemanagementreusablepolicysetting"></a><span data-ttu-id="f11cb-103">Excluir deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="f11cb-103">Delete deviceManagementReusablePolicySetting</span></span>

<span data-ttu-id="f11cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f11cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f11cb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f11cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f11cb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f11cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f11cb-107">Exclui um [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md).</span><span class="sxs-lookup"><span data-stu-id="f11cb-107">Deletes a [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f11cb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f11cb-108">Prerequisites</span></span>
<span data-ttu-id="f11cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f11cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f11cb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f11cb-111">Permission type</span></span>|<span data-ttu-id="f11cb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f11cb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f11cb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f11cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f11cb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f11cb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f11cb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f11cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f11cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f11cb-116">Not supported.</span></span>|
|<span data-ttu-id="f11cb-117">Application</span><span class="sxs-lookup"><span data-stu-id="f11cb-117">Application</span></span>|<span data-ttu-id="f11cb-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f11cb-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f11cb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f11cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}
```

## <a name="request-headers"></a><span data-ttu-id="f11cb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f11cb-120">Request headers</span></span>
|<span data-ttu-id="f11cb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f11cb-121">Header</span></span>|<span data-ttu-id="f11cb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f11cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f11cb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f11cb-123">Authorization</span></span>|<span data-ttu-id="f11cb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f11cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f11cb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f11cb-125">Accept</span></span>|<span data-ttu-id="f11cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f11cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f11cb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f11cb-127">Request body</span></span>
<span data-ttu-id="f11cb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f11cb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f11cb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f11cb-129">Response</span></span>
<span data-ttu-id="f11cb-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f11cb-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f11cb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f11cb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f11cb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f11cb-132">Request</span></span>
<span data-ttu-id="f11cb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f11cb-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}
```

### <a name="response"></a><span data-ttu-id="f11cb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f11cb-134">Response</span></span>
<span data-ttu-id="f11cb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f11cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




