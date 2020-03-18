---
title: Atualizar groupPolicyPresentationCheckBox
description: Atualiza as propriedades de um objeto groupPolicyPresentationCheckBox.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26de37d645174d60dbfaf0717f236ec15ce0f31e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804328"
---
# <a name="update-grouppolicypresentationcheckbox"></a><span data-ttu-id="daa81-103">Atualizar groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="daa81-103">Update groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="daa81-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="daa81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="daa81-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="daa81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daa81-106">Atualiza as propriedades de um objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="daa81-106">Update the properties of a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="daa81-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="daa81-107">Prerequisites</span></span>
<span data-ttu-id="daa81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daa81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daa81-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="daa81-110">Permission type</span></span>|<span data-ttu-id="daa81-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="daa81-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daa81-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="daa81-112">Delegated (work or school account)</span></span>|<span data-ttu-id="daa81-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daa81-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="daa81-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="daa81-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="daa81-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daa81-115">Not supported.</span></span>|
|<span data-ttu-id="daa81-116">Application</span><span class="sxs-lookup"><span data-stu-id="daa81-116">Application</span></span>|<span data-ttu-id="daa81-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daa81-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="daa81-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="daa81-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="daa81-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="daa81-119">Request headers</span></span>
|<span data-ttu-id="daa81-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="daa81-120">Header</span></span>|<span data-ttu-id="daa81-121">Valor</span><span class="sxs-lookup"><span data-stu-id="daa81-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="daa81-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="daa81-122">Authorization</span></span>|<span data-ttu-id="daa81-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="daa81-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="daa81-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="daa81-124">Accept</span></span>|<span data-ttu-id="daa81-125">application/json</span><span class="sxs-lookup"><span data-stu-id="daa81-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="daa81-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="daa81-126">Request body</span></span>
<span data-ttu-id="daa81-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="daa81-127">In the request body, supply a JSON representation for the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

<span data-ttu-id="daa81-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span><span class="sxs-lookup"><span data-stu-id="daa81-128">The following table shows the properties that are required when you create the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span></span>

|<span data-ttu-id="daa81-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="daa81-129">Property</span></span>|<span data-ttu-id="daa81-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="daa81-130">Type</span></span>|<span data-ttu-id="daa81-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="daa81-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daa81-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="daa81-132">label</span></span>|<span data-ttu-id="daa81-133">String</span><span class="sxs-lookup"><span data-stu-id="daa81-133">String</span></span>|<span data-ttu-id="daa81-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="daa81-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="daa81-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="daa81-135">The default value is empty.</span></span> <span data-ttu-id="daa81-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="daa81-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="daa81-137">id</span><span class="sxs-lookup"><span data-stu-id="daa81-137">id</span></span>|<span data-ttu-id="daa81-138">String</span><span class="sxs-lookup"><span data-stu-id="daa81-138">String</span></span>|<span data-ttu-id="daa81-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="daa81-139">Key of the entity.</span></span> <span data-ttu-id="daa81-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="daa81-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="daa81-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="daa81-141">lastModifiedDateTime</span></span>|<span data-ttu-id="daa81-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="daa81-142">DateTimeOffset</span></span>|<span data-ttu-id="daa81-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="daa81-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="daa81-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="daa81-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="daa81-145">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="daa81-145">defaultChecked</span></span>|<span data-ttu-id="daa81-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="daa81-146">Boolean</span></span>|<span data-ttu-id="daa81-147">Valor padrão da caixa de seleção.</span><span class="sxs-lookup"><span data-stu-id="daa81-147">Default value for the check box.</span></span> <span data-ttu-id="daa81-148">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="daa81-148">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="daa81-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="daa81-149">Response</span></span>
<span data-ttu-id="daa81-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="daa81-150">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daa81-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="daa81-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="daa81-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="daa81-152">Request</span></span>
<span data-ttu-id="daa81-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="daa81-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="daa81-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="daa81-154">Response</span></span>
<span data-ttu-id="daa81-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="daa81-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




