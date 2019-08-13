---
title: Excluir securityBaselineTemplate
description: Exclui securityBaselineTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cbf6d047b6ef882f41b3b8287b5338ab1cdd478c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349002"
---
# <a name="delete-securitybaselinetemplate"></a><span data-ttu-id="4b0fb-103">Excluir securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="4b0fb-103">Delete securityBaselineTemplate</span></span>

> <span data-ttu-id="4b0fb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b0fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b0fb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b0fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b0fb-106">Exclui [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="4b0fb-106">Deletes a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b0fb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b0fb-107">Prerequisites</span></span>
<span data-ttu-id="4b0fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b0fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b0fb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b0fb-110">Permission type</span></span>|<span data-ttu-id="4b0fb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4b0fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b0fb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b0fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b0fb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b0fb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b0fb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b0fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b0fb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b0fb-115">Not supported.</span></span>|
|<span data-ttu-id="4b0fb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b0fb-116">Application</span></span>|<span data-ttu-id="4b0fb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b0fb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b0fb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b0fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/templates/{deviceManagementTemplateId}
DELETE /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="4b0fb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b0fb-119">Request headers</span></span>
|<span data-ttu-id="4b0fb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b0fb-120">Header</span></span>|<span data-ttu-id="4b0fb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4b0fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b0fb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b0fb-122">Authorization</span></span>|<span data-ttu-id="4b0fb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b0fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b0fb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b0fb-124">Accept</span></span>|<span data-ttu-id="4b0fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b0fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b0fb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b0fb-126">Request body</span></span>
<span data-ttu-id="4b0fb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4b0fb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b0fb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b0fb-128">Response</span></span>
<span data-ttu-id="4b0fb-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4b0fb-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4b0fb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b0fb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b0fb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b0fb-131">Request</span></span>
<span data-ttu-id="4b0fb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b0fb-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
```

### <a name="response"></a><span data-ttu-id="4b0fb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b0fb-133">Response</span></span>
<span data-ttu-id="4b0fb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b0fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






