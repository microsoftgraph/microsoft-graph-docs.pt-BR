---
title: Excluir deviceManagementAbstractComplexSettingDefinition
description: Exclui deviceManagementAbstractComplexSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 72e110e95f2db6cbf46cc85134e0452ab1fd1243
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47974503"
---
# <a name="delete-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="07a01-103">Excluir deviceManagementAbstractComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="07a01-103">Delete deviceManagementAbstractComplexSettingDefinition</span></span>

<span data-ttu-id="07a01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07a01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07a01-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07a01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07a01-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07a01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07a01-107">Exclui [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="07a01-107">Deletes a [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07a01-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07a01-108">Prerequisites</span></span>
<span data-ttu-id="07a01-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07a01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07a01-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07a01-111">Permission type</span></span>|<span data-ttu-id="07a01-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07a01-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07a01-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07a01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07a01-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07a01-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="07a01-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07a01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07a01-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07a01-116">Not supported.</span></span>|
|<span data-ttu-id="07a01-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07a01-117">Application</span></span>|<span data-ttu-id="07a01-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07a01-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07a01-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07a01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
DELETE /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
DELETE /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
DELETE /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="07a01-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07a01-120">Request headers</span></span>
|<span data-ttu-id="07a01-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07a01-121">Header</span></span>|<span data-ttu-id="07a01-122">Valor</span><span class="sxs-lookup"><span data-stu-id="07a01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07a01-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="07a01-123">Authorization</span></span>|<span data-ttu-id="07a01-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07a01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07a01-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07a01-125">Accept</span></span>|<span data-ttu-id="07a01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07a01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07a01-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07a01-127">Request body</span></span>
<span data-ttu-id="07a01-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07a01-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07a01-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="07a01-129">Response</span></span>
<span data-ttu-id="07a01-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="07a01-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="07a01-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07a01-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="07a01-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07a01-132">Request</span></span>
<span data-ttu-id="07a01-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07a01-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="07a01-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="07a01-134">Response</span></span>
<span data-ttu-id="07a01-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07a01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






