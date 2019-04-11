---
title: Excluir deviceManagementComplexSettingInstance
description: Exclui deviceManagementComplexSettingInstance.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f451336fc1535aa1a63201387787c42ee2633050
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783588"
---
# <a name="delete-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="8fba8-103">Excluir deviceManagementComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="8fba8-103">Delete deviceManagementComplexSettingInstance</span></span>

> <span data-ttu-id="8fba8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8fba8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fba8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8fba8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fba8-106">Exclui [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="8fba8-106">Deletes a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fba8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8fba8-107">Prerequisites</span></span>
<span data-ttu-id="8fba8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fba8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fba8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fba8-110">Permission type</span></span>|<span data-ttu-id="8fba8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8fba8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fba8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fba8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8fba8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fba8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8fba8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fba8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fba8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fba8-115">Not supported.</span></span>|
|<span data-ttu-id="8fba8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fba8-116">Application</span></span>|<span data-ttu-id="8fba8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fba8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fba8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fba8-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="8fba8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8fba8-119">Request headers</span></span>
|<span data-ttu-id="8fba8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8fba8-120">Header</span></span>|<span data-ttu-id="8fba8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8fba8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fba8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fba8-122">Authorization</span></span>|<span data-ttu-id="8fba8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8fba8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fba8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8fba8-124">Accept</span></span>|<span data-ttu-id="8fba8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8fba8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fba8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fba8-126">Request body</span></span>
<span data-ttu-id="8fba8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8fba8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fba8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fba8-128">Response</span></span>
<span data-ttu-id="8fba8-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8fba8-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8fba8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8fba8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fba8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fba8-131">Request</span></span>
<span data-ttu-id="8fba8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8fba8-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="8fba8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fba8-133">Response</span></span>
<span data-ttu-id="8fba8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8fba8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





