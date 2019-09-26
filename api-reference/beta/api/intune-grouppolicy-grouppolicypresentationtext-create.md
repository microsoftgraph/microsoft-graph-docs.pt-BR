---
title: Criar groupPolicyPresentationText
description: Criar um novo objeto groupPolicyPresentationText.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a2b3568b6959819cbbf9e81821f129d7174086f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194065"
---
# <a name="create-grouppolicypresentationtext"></a><span data-ttu-id="2820e-103">Criar groupPolicyPresentationText</span><span class="sxs-lookup"><span data-stu-id="2820e-103">Create groupPolicyPresentationText</span></span>

> <span data-ttu-id="2820e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2820e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2820e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2820e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2820e-106">Criar um novo objeto [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .</span><span class="sxs-lookup"><span data-stu-id="2820e-106">Create a new [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2820e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2820e-107">Prerequisites</span></span>
<span data-ttu-id="2820e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2820e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2820e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2820e-110">Permission type</span></span>|<span data-ttu-id="2820e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2820e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2820e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2820e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2820e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2820e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2820e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2820e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2820e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2820e-115">Not supported.</span></span>|
|<span data-ttu-id="2820e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2820e-116">Application</span></span>|<span data-ttu-id="2820e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2820e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2820e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2820e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="2820e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2820e-119">Request headers</span></span>
|<span data-ttu-id="2820e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2820e-120">Header</span></span>|<span data-ttu-id="2820e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2820e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2820e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2820e-122">Authorization</span></span>|<span data-ttu-id="2820e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2820e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2820e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2820e-124">Accept</span></span>|<span data-ttu-id="2820e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2820e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2820e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2820e-126">Request body</span></span>
<span data-ttu-id="2820e-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationText.</span><span class="sxs-lookup"><span data-stu-id="2820e-127">In the request body, supply a JSON representation for the groupPolicyPresentationText object.</span></span>

<span data-ttu-id="2820e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationText.</span><span class="sxs-lookup"><span data-stu-id="2820e-128">The following table shows the properties that are required when you create the groupPolicyPresentationText.</span></span>

|<span data-ttu-id="2820e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2820e-129">Property</span></span>|<span data-ttu-id="2820e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2820e-130">Type</span></span>|<span data-ttu-id="2820e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2820e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2820e-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="2820e-132">label</span></span>|<span data-ttu-id="2820e-133">String</span><span class="sxs-lookup"><span data-stu-id="2820e-133">String</span></span>|<span data-ttu-id="2820e-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="2820e-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="2820e-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="2820e-135">The default value is empty.</span></span> <span data-ttu-id="2820e-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2820e-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="2820e-137">id</span><span class="sxs-lookup"><span data-stu-id="2820e-137">id</span></span>|<span data-ttu-id="2820e-138">String</span><span class="sxs-lookup"><span data-stu-id="2820e-138">String</span></span>|<span data-ttu-id="2820e-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2820e-139">Key of the entity.</span></span> <span data-ttu-id="2820e-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2820e-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="2820e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2820e-141">lastModifiedDateTime</span></span>|<span data-ttu-id="2820e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2820e-142">DateTimeOffset</span></span>|<span data-ttu-id="2820e-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2820e-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="2820e-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2820e-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2820e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="2820e-145">Response</span></span>
<span data-ttu-id="2820e-146">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2820e-146">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2820e-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2820e-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="2820e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2820e-148">Request</span></span>
<span data-ttu-id="2820e-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2820e-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="2820e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="2820e-150">Response</span></span>
<span data-ttu-id="2820e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2820e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 209

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value",
  "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




