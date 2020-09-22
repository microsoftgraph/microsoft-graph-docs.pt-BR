---
title: Excluir deviceManagementComplexSettingInstance
description: Exclui deviceManagementComplexSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d691cf5c2d139f46218ae595ef09b8180a60917c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088234"
---
# <a name="delete-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="7f059-103">Excluir deviceManagementComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="7f059-103">Delete deviceManagementComplexSettingInstance</span></span>

<span data-ttu-id="7f059-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f059-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f059-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f059-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f059-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f059-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f059-107">Exclui [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="7f059-107">Deletes a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f059-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7f059-108">Prerequisites</span></span>
<span data-ttu-id="7f059-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f059-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f059-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f059-111">Permission type</span></span>|<span data-ttu-id="7f059-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7f059-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f059-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f059-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f059-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f059-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f059-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f059-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f059-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f059-116">Not supported.</span></span>|
|<span data-ttu-id="7f059-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f059-117">Application</span></span>|<span data-ttu-id="7f059-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f059-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f059-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f059-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
DELETE /deviceManagement/templates/{deviceManagementTemplateId}/settings/{deviceManagementSettingInstanceId}
DELETE /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/{deviceManagementSettingInstanceId}
DELETE /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings/{deviceManagementSettingInstanceId}
```

## <a name="request-headers"></a><span data-ttu-id="7f059-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f059-120">Request headers</span></span>
|<span data-ttu-id="7f059-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f059-121">Header</span></span>|<span data-ttu-id="7f059-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7f059-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f059-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f059-123">Authorization</span></span>|<span data-ttu-id="7f059-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f059-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f059-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7f059-125">Accept</span></span>|<span data-ttu-id="7f059-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f059-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f059-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f059-127">Request body</span></span>
<span data-ttu-id="7f059-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f059-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f059-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f059-129">Response</span></span>
<span data-ttu-id="7f059-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7f059-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7f059-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f059-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f059-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f059-132">Request</span></span>
<span data-ttu-id="7f059-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f059-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="7f059-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f059-134">Response</span></span>
<span data-ttu-id="7f059-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f059-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






