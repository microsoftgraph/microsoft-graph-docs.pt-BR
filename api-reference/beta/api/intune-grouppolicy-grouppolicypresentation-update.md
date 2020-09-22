---
title: Atualizar groupPolicyPresentation
description: Atualiza as propriedades de um objeto groupPolicyPresentation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e18c2e2cbc7669f82d43dd4ac01676f2630b5382
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48043252"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="f5dca-103">Atualizar groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="f5dca-103">Update groupPolicyPresentation</span></span>

<span data-ttu-id="f5dca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5dca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5dca-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f5dca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5dca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f5dca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5dca-107">Atualiza as propriedades de um objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="f5dca-107">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5dca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5dca-108">Prerequisites</span></span>
<span data-ttu-id="f5dca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5dca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5dca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5dca-111">Permission type</span></span>|<span data-ttu-id="f5dca-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f5dca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5dca-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5dca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5dca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5dca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5dca-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5dca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5dca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5dca-116">Not supported.</span></span>|
|<span data-ttu-id="f5dca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5dca-117">Application</span></span>|<span data-ttu-id="f5dca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5dca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5dca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5dca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="f5dca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5dca-120">Request headers</span></span>
|<span data-ttu-id="f5dca-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5dca-121">Header</span></span>|<span data-ttu-id="f5dca-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f5dca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5dca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5dca-123">Authorization</span></span>|<span data-ttu-id="f5dca-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5dca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5dca-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5dca-125">Accept</span></span>|<span data-ttu-id="f5dca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5dca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5dca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5dca-127">Request body</span></span>
<span data-ttu-id="f5dca-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="f5dca-128">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="f5dca-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span><span class="sxs-lookup"><span data-stu-id="f5dca-129">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="f5dca-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5dca-130">Property</span></span>|<span data-ttu-id="f5dca-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5dca-131">Type</span></span>|<span data-ttu-id="f5dca-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5dca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5dca-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="f5dca-133">label</span></span>|<span data-ttu-id="f5dca-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5dca-134">String</span></span>|<span data-ttu-id="f5dca-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="f5dca-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="f5dca-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="f5dca-136">The default value is empty.</span></span>|
|<span data-ttu-id="f5dca-137">id</span><span class="sxs-lookup"><span data-stu-id="f5dca-137">id</span></span>|<span data-ttu-id="f5dca-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5dca-138">String</span></span>|<span data-ttu-id="f5dca-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f5dca-139">Key of the entity.</span></span>|
|<span data-ttu-id="f5dca-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5dca-140">lastModifiedDateTime</span></span>|<span data-ttu-id="f5dca-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5dca-141">DateTimeOffset</span></span>|<span data-ttu-id="f5dca-142">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f5dca-142">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="f5dca-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5dca-143">Response</span></span>
<span data-ttu-id="f5dca-144">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5dca-144">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5dca-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5dca-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5dca-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5dca-146">Request</span></span>
<span data-ttu-id="f5dca-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5dca-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="f5dca-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5dca-148">Response</span></span>
<span data-ttu-id="f5dca-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5dca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






