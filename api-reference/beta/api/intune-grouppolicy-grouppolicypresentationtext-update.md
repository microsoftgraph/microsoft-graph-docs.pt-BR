---
title: Atualizar groupPolicyPresentationText
description: Atualize as propriedades de um objeto groupPolicyPresentationText.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: edab3145c9618c0c298cd1502c6aed5965394713
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149433"
---
# <a name="update-grouppolicypresentationtext"></a><span data-ttu-id="d6995-103">Atualizar groupPolicyPresentationText</span><span class="sxs-lookup"><span data-stu-id="d6995-103">Update groupPolicyPresentationText</span></span>

<span data-ttu-id="d6995-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6995-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6995-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6995-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6995-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6995-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6995-107">Atualize as propriedades de [um objeto groupPolicyPresentationText.](../resources/intune-grouppolicy-grouppolicypresentationtext.md)</span><span class="sxs-lookup"><span data-stu-id="d6995-107">Update the properties of a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6995-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6995-108">Prerequisites</span></span>
<span data-ttu-id="d6995-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6995-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6995-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6995-111">Permission type</span></span>|<span data-ttu-id="d6995-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6995-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6995-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6995-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6995-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6995-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6995-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6995-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6995-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6995-116">Not supported.</span></span>|
|<span data-ttu-id="d6995-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6995-117">Application</span></span>|<span data-ttu-id="d6995-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6995-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6995-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6995-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="d6995-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6995-120">Request headers</span></span>
|<span data-ttu-id="d6995-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6995-121">Header</span></span>|<span data-ttu-id="d6995-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d6995-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6995-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6995-123">Authorization</span></span>|<span data-ttu-id="d6995-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6995-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6995-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6995-125">Accept</span></span>|<span data-ttu-id="d6995-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6995-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6995-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6995-127">Request body</span></span>
<span data-ttu-id="d6995-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicyPresentationText.](../resources/intune-grouppolicy-grouppolicypresentationtext.md)</span><span class="sxs-lookup"><span data-stu-id="d6995-128">In the request body, supply a JSON representation for the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

<span data-ttu-id="d6995-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).</span><span class="sxs-lookup"><span data-stu-id="d6995-129">The following table shows the properties that are required when you create the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).</span></span>

|<span data-ttu-id="d6995-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6995-130">Property</span></span>|<span data-ttu-id="d6995-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6995-131">Type</span></span>|<span data-ttu-id="d6995-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6995-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6995-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="d6995-133">label</span></span>|<span data-ttu-id="d6995-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6995-134">String</span></span>|<span data-ttu-id="d6995-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="d6995-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="d6995-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="d6995-136">The default value is empty.</span></span> <span data-ttu-id="d6995-137">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d6995-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d6995-138">id</span><span class="sxs-lookup"><span data-stu-id="d6995-138">id</span></span>|<span data-ttu-id="d6995-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6995-139">String</span></span>|<span data-ttu-id="d6995-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d6995-140">Key of the entity.</span></span> <span data-ttu-id="d6995-141">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d6995-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d6995-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6995-142">lastModifiedDateTime</span></span>|<span data-ttu-id="d6995-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6995-143">DateTimeOffset</span></span>|<span data-ttu-id="d6995-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d6995-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="d6995-145">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d6995-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d6995-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6995-146">Response</span></span>
<span data-ttu-id="d6995-147">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6995-147">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6995-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6995-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6995-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6995-149">Request</span></span>
<span data-ttu-id="d6995-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6995-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="d6995-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6995-151">Response</span></span>
<span data-ttu-id="d6995-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6995-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 209

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value",
  "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




