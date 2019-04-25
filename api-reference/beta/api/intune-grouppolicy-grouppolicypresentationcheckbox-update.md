---
title: Atualizar groupPolicyPresentationCheckBox
description: Atualiza as propriedades de um objeto groupPolicyPresentationCheckBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a00c21cf6fdd177432b5aa5a28e4e816a3b9ffea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32531156"
---
# <a name="update-grouppolicypresentationcheckbox"></a><span data-ttu-id="70ba1-103">Atualizar groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="70ba1-103">Update groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="70ba1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="70ba1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70ba1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="70ba1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70ba1-106">Atualiza as propriedades de um objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="70ba1-106">Update the properties of a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70ba1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="70ba1-107">Prerequisites</span></span>
<span data-ttu-id="70ba1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70ba1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70ba1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70ba1-110">Permission type</span></span>|<span data-ttu-id="70ba1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="70ba1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70ba1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70ba1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70ba1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70ba1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="70ba1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70ba1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70ba1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70ba1-115">Not supported.</span></span>|
|<span data-ttu-id="70ba1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70ba1-116">Application</span></span>|<span data-ttu-id="70ba1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70ba1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70ba1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70ba1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="70ba1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70ba1-119">Request headers</span></span>
|<span data-ttu-id="70ba1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="70ba1-120">Header</span></span>|<span data-ttu-id="70ba1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="70ba1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70ba1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="70ba1-122">Authorization</span></span>|<span data-ttu-id="70ba1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70ba1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70ba1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="70ba1-124">Accept</span></span>|<span data-ttu-id="70ba1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="70ba1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70ba1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70ba1-126">Request body</span></span>
<span data-ttu-id="70ba1-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="70ba1-127">In the request body, supply a JSON representation for the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

<span data-ttu-id="70ba1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span><span class="sxs-lookup"><span data-stu-id="70ba1-128">The following table shows the properties that are required when you create the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span></span>

|<span data-ttu-id="70ba1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70ba1-129">Property</span></span>|<span data-ttu-id="70ba1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="70ba1-130">Type</span></span>|<span data-ttu-id="70ba1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="70ba1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70ba1-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="70ba1-132">label</span></span>|<span data-ttu-id="70ba1-133">String</span><span class="sxs-lookup"><span data-stu-id="70ba1-133">String</span></span>|<span data-ttu-id="70ba1-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="70ba1-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="70ba1-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="70ba1-135">The default value is empty.</span></span> <span data-ttu-id="70ba1-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="70ba1-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="70ba1-137">id</span><span class="sxs-lookup"><span data-stu-id="70ba1-137">id</span></span>|<span data-ttu-id="70ba1-138">String</span><span class="sxs-lookup"><span data-stu-id="70ba1-138">String</span></span>|<span data-ttu-id="70ba1-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="70ba1-139">Key of the entity.</span></span> <span data-ttu-id="70ba1-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="70ba1-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="70ba1-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70ba1-141">lastModifiedDateTime</span></span>|<span data-ttu-id="70ba1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70ba1-142">DateTimeOffset</span></span>|<span data-ttu-id="70ba1-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="70ba1-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="70ba1-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="70ba1-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="70ba1-145">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="70ba1-145">defaultChecked</span></span>|<span data-ttu-id="70ba1-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="70ba1-146">Boolean</span></span>|<span data-ttu-id="70ba1-147">Valor padrão da caixa de seleção.</span><span class="sxs-lookup"><span data-stu-id="70ba1-147">Default value for the check box.</span></span> <span data-ttu-id="70ba1-148">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="70ba1-148">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="70ba1-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="70ba1-149">Response</span></span>
<span data-ttu-id="70ba1-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70ba1-150">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70ba1-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70ba1-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="70ba1-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70ba1-152">Request</span></span>
<span data-ttu-id="70ba1-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70ba1-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="70ba1-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="70ba1-154">Response</span></span>
<span data-ttu-id="70ba1-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70ba1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





