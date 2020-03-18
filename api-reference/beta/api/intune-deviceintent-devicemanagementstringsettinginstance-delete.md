---
title: Excluir deviceManagementStringSettingInstance
description: Exclui deviceManagementStringSettingInstance.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8f04e98f5be1422b382437cffc4068814e8dcfde
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815041"
---
# <a name="delete-devicemanagementstringsettinginstance"></a><span data-ttu-id="90039-103">Excluir deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="90039-103">Delete deviceManagementStringSettingInstance</span></span>

> <span data-ttu-id="90039-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="90039-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90039-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90039-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90039-106">Exclui [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="90039-106">Deletes a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90039-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90039-107">Prerequisites</span></span>
<span data-ttu-id="90039-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90039-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90039-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90039-110">Permission type</span></span>|<span data-ttu-id="90039-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90039-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90039-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90039-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90039-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90039-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90039-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90039-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90039-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90039-115">Not supported.</span></span>|
|<span data-ttu-id="90039-116">Application</span><span class="sxs-lookup"><span data-stu-id="90039-116">Application</span></span>|<span data-ttu-id="90039-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90039-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90039-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90039-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="90039-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90039-119">Request headers</span></span>
|<span data-ttu-id="90039-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90039-120">Header</span></span>|<span data-ttu-id="90039-121">Valor</span><span class="sxs-lookup"><span data-stu-id="90039-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90039-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="90039-122">Authorization</span></span>|<span data-ttu-id="90039-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90039-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90039-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90039-124">Accept</span></span>|<span data-ttu-id="90039-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90039-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90039-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90039-126">Request body</span></span>
<span data-ttu-id="90039-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90039-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90039-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="90039-128">Response</span></span>
<span data-ttu-id="90039-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="90039-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="90039-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90039-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="90039-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90039-131">Request</span></span>
<span data-ttu-id="90039-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90039-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="90039-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="90039-133">Response</span></span>
<span data-ttu-id="90039-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90039-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




