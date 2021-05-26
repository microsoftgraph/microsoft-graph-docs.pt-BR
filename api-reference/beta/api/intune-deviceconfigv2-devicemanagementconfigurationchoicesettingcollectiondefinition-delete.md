---
title: Excluir deviceManagementConfigurationChoiceSettingCollectionDefinition
description: Exclui um deviceManagementConfigurationChoiceSettingCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4e696387e3bff3e79116ad8accae3f6c66b83114
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666159"
---
# <a name="delete-devicemanagementconfigurationchoicesettingcollectiondefinition"></a><span data-ttu-id="b6cfe-103">Excluir deviceManagementConfigurationChoiceSettingCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="b6cfe-103">Delete deviceManagementConfigurationChoiceSettingCollectionDefinition</span></span>

<span data-ttu-id="b6cfe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6cfe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6cfe-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6cfe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6cfe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6cfe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6cfe-107">Exclui um [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b6cfe-107">Deletes a [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6cfe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6cfe-108">Prerequisites</span></span>
<span data-ttu-id="b6cfe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6cfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6cfe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6cfe-111">Permission type</span></span>|<span data-ttu-id="b6cfe-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6cfe-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6cfe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6cfe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6cfe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6cfe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6cfe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6cfe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6cfe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6cfe-116">Not supported.</span></span>|
|<span data-ttu-id="b6cfe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6cfe-117">Application</span></span>|<span data-ttu-id="b6cfe-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6cfe-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6cfe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6cfe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
DELETE /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
DELETE /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
DELETE /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="b6cfe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6cfe-120">Request headers</span></span>
|<span data-ttu-id="b6cfe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6cfe-121">Header</span></span>|<span data-ttu-id="b6cfe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6cfe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6cfe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6cfe-123">Authorization</span></span>|<span data-ttu-id="b6cfe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6cfe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6cfe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6cfe-125">Accept</span></span>|<span data-ttu-id="b6cfe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6cfe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6cfe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6cfe-127">Request body</span></span>
<span data-ttu-id="b6cfe-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6cfe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6cfe-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6cfe-129">Response</span></span>
<span data-ttu-id="b6cfe-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b6cfe-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b6cfe-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6cfe-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6cfe-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6cfe-132">Request</span></span>
<span data-ttu-id="b6cfe-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6cfe-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="b6cfe-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6cfe-134">Response</span></span>
<span data-ttu-id="b6cfe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6cfe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




