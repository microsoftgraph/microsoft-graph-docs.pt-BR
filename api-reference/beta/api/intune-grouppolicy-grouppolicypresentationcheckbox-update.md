---
title: Atualizar groupPolicyPresentationCheckBox
description: Atualiza as propriedades de um objeto groupPolicyPresentationCheckBox.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1581a59291006fd4ca693fa573c735f8097d7f56
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35989739"
---
# <a name="update-grouppolicypresentationcheckbox"></a><span data-ttu-id="4df54-103">Atualizar groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="4df54-103">Update groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="4df54-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4df54-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4df54-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4df54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4df54-106">Atualiza as propriedades de um objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="4df54-106">Update the properties of a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4df54-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4df54-107">Prerequisites</span></span>
<span data-ttu-id="4df54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4df54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4df54-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4df54-110">Permission type</span></span>|<span data-ttu-id="4df54-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4df54-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4df54-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4df54-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4df54-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4df54-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4df54-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4df54-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4df54-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4df54-115">Not supported.</span></span>|
|<span data-ttu-id="4df54-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4df54-116">Application</span></span>|<span data-ttu-id="4df54-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4df54-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4df54-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4df54-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="4df54-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4df54-119">Request headers</span></span>
|<span data-ttu-id="4df54-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4df54-120">Header</span></span>|<span data-ttu-id="4df54-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4df54-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4df54-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4df54-122">Authorization</span></span>|<span data-ttu-id="4df54-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4df54-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4df54-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4df54-124">Accept</span></span>|<span data-ttu-id="4df54-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4df54-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4df54-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4df54-126">Request body</span></span>
<span data-ttu-id="4df54-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="4df54-127">In the request body, supply a JSON representation for the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

<span data-ttu-id="4df54-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span><span class="sxs-lookup"><span data-stu-id="4df54-128">The following table shows the properties that are required when you create the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span></span>

|<span data-ttu-id="4df54-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4df54-129">Property</span></span>|<span data-ttu-id="4df54-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4df54-130">Type</span></span>|<span data-ttu-id="4df54-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4df54-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4df54-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="4df54-132">label</span></span>|<span data-ttu-id="4df54-133">String</span><span class="sxs-lookup"><span data-stu-id="4df54-133">String</span></span>|<span data-ttu-id="4df54-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="4df54-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="4df54-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="4df54-135">The default value is empty.</span></span> <span data-ttu-id="4df54-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="4df54-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="4df54-137">id</span><span class="sxs-lookup"><span data-stu-id="4df54-137">id</span></span>|<span data-ttu-id="4df54-138">String</span><span class="sxs-lookup"><span data-stu-id="4df54-138">String</span></span>|<span data-ttu-id="4df54-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4df54-139">Key of the entity.</span></span> <span data-ttu-id="4df54-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="4df54-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="4df54-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4df54-141">lastModifiedDateTime</span></span>|<span data-ttu-id="4df54-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4df54-142">DateTimeOffset</span></span>|<span data-ttu-id="4df54-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4df54-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="4df54-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="4df54-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="4df54-145">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="4df54-145">defaultChecked</span></span>|<span data-ttu-id="4df54-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="4df54-146">Boolean</span></span>|<span data-ttu-id="4df54-147">Valor padrão da caixa de seleção.</span><span class="sxs-lookup"><span data-stu-id="4df54-147">Default value for the check box.</span></span> <span data-ttu-id="4df54-148">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="4df54-148">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="4df54-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="4df54-149">Response</span></span>
<span data-ttu-id="4df54-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4df54-150">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4df54-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4df54-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="4df54-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4df54-152">Request</span></span>
<span data-ttu-id="4df54-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4df54-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
}
```

### <a name="response"></a><span data-ttu-id="4df54-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="4df54-154">Response</span></span>
<span data-ttu-id="4df54-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4df54-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "id": "7748190f-190f-7748-0f19-48770f194877",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultChecked": true
}
```





