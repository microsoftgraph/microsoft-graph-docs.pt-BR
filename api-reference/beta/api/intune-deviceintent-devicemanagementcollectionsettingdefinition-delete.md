---
title: Excluir deviceManagementCollectionSettingDefinition
description: Exclui deviceManagementCollectionSettingDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 85973c5408c9e4faacd4cddcdf08250724692009
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32509958"
---
# <a name="delete-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="afbff-103">Excluir deviceManagementCollectionSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="afbff-103">Delete deviceManagementCollectionSettingDefinition</span></span>

> <span data-ttu-id="afbff-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="afbff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afbff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="afbff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afbff-106">Exclui [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="afbff-106">Deletes a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afbff-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="afbff-107">Prerequisites</span></span>
<span data-ttu-id="afbff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afbff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afbff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afbff-110">Permission type</span></span>|<span data-ttu-id="afbff-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="afbff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afbff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afbff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="afbff-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afbff-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="afbff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afbff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afbff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afbff-115">Not supported.</span></span>|
|<span data-ttu-id="afbff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afbff-116">Application</span></span>|<span data-ttu-id="afbff-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afbff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afbff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afbff-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="afbff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afbff-119">Request headers</span></span>
|<span data-ttu-id="afbff-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="afbff-120">Header</span></span>|<span data-ttu-id="afbff-121">Valor</span><span class="sxs-lookup"><span data-stu-id="afbff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afbff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="afbff-122">Authorization</span></span>|<span data-ttu-id="afbff-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afbff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afbff-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="afbff-124">Accept</span></span>|<span data-ttu-id="afbff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="afbff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afbff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afbff-126">Request body</span></span>
<span data-ttu-id="afbff-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="afbff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afbff-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="afbff-128">Response</span></span>
<span data-ttu-id="afbff-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="afbff-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="afbff-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afbff-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="afbff-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afbff-131">Request</span></span>
<span data-ttu-id="afbff-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="afbff-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="afbff-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="afbff-133">Response</span></span>
<span data-ttu-id="afbff-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afbff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





