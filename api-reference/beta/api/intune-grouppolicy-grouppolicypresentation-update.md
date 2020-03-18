---
title: Atualizar groupPolicyPresentation
description: Atualiza as propriedades de um objeto groupPolicyPresentation.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cd1c11317b86bfd06fa0bb486f95ec8ee2bcb82e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804363"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="565a8-103">Atualizar groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="565a8-103">Update groupPolicyPresentation</span></span>

> <span data-ttu-id="565a8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="565a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="565a8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="565a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="565a8-106">Atualiza as propriedades de um objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="565a8-106">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="565a8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="565a8-107">Prerequisites</span></span>
<span data-ttu-id="565a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="565a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="565a8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="565a8-110">Permission type</span></span>|<span data-ttu-id="565a8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="565a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="565a8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="565a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="565a8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="565a8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="565a8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="565a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="565a8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="565a8-115">Not supported.</span></span>|
|<span data-ttu-id="565a8-116">Application</span><span class="sxs-lookup"><span data-stu-id="565a8-116">Application</span></span>|<span data-ttu-id="565a8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="565a8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="565a8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="565a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="565a8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="565a8-119">Request headers</span></span>
|<span data-ttu-id="565a8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="565a8-120">Header</span></span>|<span data-ttu-id="565a8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="565a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="565a8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="565a8-122">Authorization</span></span>|<span data-ttu-id="565a8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="565a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="565a8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="565a8-124">Accept</span></span>|<span data-ttu-id="565a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="565a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="565a8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="565a8-126">Request body</span></span>
<span data-ttu-id="565a8-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="565a8-127">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="565a8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span><span class="sxs-lookup"><span data-stu-id="565a8-128">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="565a8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="565a8-129">Property</span></span>|<span data-ttu-id="565a8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="565a8-130">Type</span></span>|<span data-ttu-id="565a8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="565a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="565a8-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="565a8-132">label</span></span>|<span data-ttu-id="565a8-133">String</span><span class="sxs-lookup"><span data-stu-id="565a8-133">String</span></span>|<span data-ttu-id="565a8-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="565a8-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="565a8-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="565a8-135">The default value is empty.</span></span>|
|<span data-ttu-id="565a8-136">id</span><span class="sxs-lookup"><span data-stu-id="565a8-136">id</span></span>|<span data-ttu-id="565a8-137">String</span><span class="sxs-lookup"><span data-stu-id="565a8-137">String</span></span>|<span data-ttu-id="565a8-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="565a8-138">Key of the entity.</span></span>|
|<span data-ttu-id="565a8-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="565a8-139">lastModifiedDateTime</span></span>|<span data-ttu-id="565a8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="565a8-140">DateTimeOffset</span></span>|<span data-ttu-id="565a8-141">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="565a8-141">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="565a8-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="565a8-142">Response</span></span>
<span data-ttu-id="565a8-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="565a8-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="565a8-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="565a8-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="565a8-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="565a8-145">Request</span></span>
<span data-ttu-id="565a8-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="565a8-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="565a8-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="565a8-147">Response</span></span>
<span data-ttu-id="565a8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="565a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 205

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value",
  "id": "a33caa6a-aa6a-a33c-6aaa-3ca36aaa3ca3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




