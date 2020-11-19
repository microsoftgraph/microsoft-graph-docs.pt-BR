---
title: Atualizar groupPolicyPresentation
description: Atualiza as propriedades de um objeto groupPolicyPresentation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 38b80f055369354e4e73c74a44220940999142f9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212135"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="5ec95-103">Atualizar groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="5ec95-103">Update groupPolicyPresentation</span></span>

<span data-ttu-id="5ec95-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ec95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ec95-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ec95-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ec95-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ec95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ec95-107">Atualiza as propriedades de um objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="5ec95-107">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ec95-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ec95-108">Prerequisites</span></span>
<span data-ttu-id="5ec95-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ec95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ec95-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ec95-111">Permission type</span></span>|<span data-ttu-id="5ec95-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ec95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ec95-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ec95-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ec95-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ec95-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ec95-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ec95-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ec95-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ec95-116">Not supported.</span></span>|
|<span data-ttu-id="5ec95-117">Application</span><span class="sxs-lookup"><span data-stu-id="5ec95-117">Application</span></span>|<span data-ttu-id="5ec95-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ec95-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ec95-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ec95-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="5ec95-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ec95-120">Request headers</span></span>
|<span data-ttu-id="5ec95-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ec95-121">Header</span></span>|<span data-ttu-id="5ec95-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5ec95-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ec95-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ec95-123">Authorization</span></span>|<span data-ttu-id="5ec95-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ec95-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ec95-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ec95-125">Accept</span></span>|<span data-ttu-id="5ec95-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ec95-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ec95-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ec95-127">Request body</span></span>
<span data-ttu-id="5ec95-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="5ec95-128">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="5ec95-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span><span class="sxs-lookup"><span data-stu-id="5ec95-129">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="5ec95-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ec95-130">Property</span></span>|<span data-ttu-id="5ec95-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ec95-131">Type</span></span>|<span data-ttu-id="5ec95-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ec95-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ec95-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="5ec95-133">label</span></span>|<span data-ttu-id="5ec95-134">String</span><span class="sxs-lookup"><span data-stu-id="5ec95-134">String</span></span>|<span data-ttu-id="5ec95-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="5ec95-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="5ec95-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="5ec95-136">The default value is empty.</span></span>|
|<span data-ttu-id="5ec95-137">id</span><span class="sxs-lookup"><span data-stu-id="5ec95-137">id</span></span>|<span data-ttu-id="5ec95-138">String</span><span class="sxs-lookup"><span data-stu-id="5ec95-138">String</span></span>|<span data-ttu-id="5ec95-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ec95-139">Key of the entity.</span></span>|
|<span data-ttu-id="5ec95-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ec95-140">lastModifiedDateTime</span></span>|<span data-ttu-id="5ec95-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ec95-141">DateTimeOffset</span></span>|<span data-ttu-id="5ec95-142">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5ec95-142">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="5ec95-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ec95-143">Response</span></span>
<span data-ttu-id="5ec95-144">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ec95-144">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ec95-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ec95-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ec95-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ec95-146">Request</span></span>
<span data-ttu-id="5ec95-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ec95-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="5ec95-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ec95-148">Response</span></span>
<span data-ttu-id="5ec95-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ec95-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




