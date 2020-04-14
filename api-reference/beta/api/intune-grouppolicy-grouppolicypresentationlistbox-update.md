---
title: Atualizar groupPolicyPresentationListBox
description: Atualiza as propriedades de um objeto groupPolicyPresentationListBox.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 30f5c01eb9d8d89be4d89d5877b4d4611585fd30
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43375268"
---
# <a name="update-grouppolicypresentationlistbox"></a><span data-ttu-id="8d4a8-103">Atualizar groupPolicyPresentationListBox</span><span class="sxs-lookup"><span data-stu-id="8d4a8-103">Update groupPolicyPresentationListBox</span></span>

<span data-ttu-id="8d4a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d4a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d4a8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8d4a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d4a8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8d4a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d4a8-107">Atualiza as propriedades de um objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="8d4a8-107">Update the properties of a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d4a8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8d4a8-108">Prerequisites</span></span>
<span data-ttu-id="8d4a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d4a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d4a8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d4a8-111">Permission type</span></span>|<span data-ttu-id="8d4a8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8d4a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d4a8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d4a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d4a8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d4a8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d4a8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d4a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d4a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d4a8-116">Not supported.</span></span>|
|<span data-ttu-id="8d4a8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d4a8-117">Application</span></span>|<span data-ttu-id="8d4a8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d4a8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d4a8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d4a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="8d4a8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d4a8-120">Request headers</span></span>
|<span data-ttu-id="8d4a8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d4a8-121">Header</span></span>|<span data-ttu-id="8d4a8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8d4a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d4a8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d4a8-123">Authorization</span></span>|<span data-ttu-id="8d4a8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d4a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d4a8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8d4a8-125">Accept</span></span>|<span data-ttu-id="8d4a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d4a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d4a8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d4a8-127">Request body</span></span>
<span data-ttu-id="8d4a8-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="8d4a8-128">In the request body, supply a JSON representation for the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

<span data-ttu-id="8d4a8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span><span class="sxs-lookup"><span data-stu-id="8d4a8-129">The following table shows the properties that are required when you create the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span></span>

|<span data-ttu-id="8d4a8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d4a8-130">Property</span></span>|<span data-ttu-id="8d4a8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d4a8-131">Type</span></span>|<span data-ttu-id="8d4a8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d4a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d4a8-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="8d4a8-133">label</span></span>|<span data-ttu-id="8d4a8-134">String</span><span class="sxs-lookup"><span data-stu-id="8d4a8-134">String</span></span>|<span data-ttu-id="8d4a8-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="8d4a8-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="8d4a8-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="8d4a8-136">The default value is empty.</span></span> <span data-ttu-id="8d4a8-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8d4a8-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8d4a8-138">id</span><span class="sxs-lookup"><span data-stu-id="8d4a8-138">id</span></span>|<span data-ttu-id="8d4a8-139">String</span><span class="sxs-lookup"><span data-stu-id="8d4a8-139">String</span></span>|<span data-ttu-id="8d4a8-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8d4a8-140">Key of the entity.</span></span> <span data-ttu-id="8d4a8-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8d4a8-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8d4a8-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d4a8-142">lastModifiedDateTime</span></span>|<span data-ttu-id="8d4a8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d4a8-143">DateTimeOffset</span></span>|<span data-ttu-id="8d4a8-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8d4a8-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="8d4a8-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8d4a8-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8d4a8-146">explicitValue</span><span class="sxs-lookup"><span data-stu-id="8d4a8-146">explicitValue</span></span>|<span data-ttu-id="8d4a8-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d4a8-147">Boolean</span></span>|<span data-ttu-id="8d4a8-148">Se essa opção for especificada true, o usuário deverá especificar o valor da subchave do registro e o nome da subchave do registro.</span><span class="sxs-lookup"><span data-stu-id="8d4a8-148">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="8d4a8-149">A caixa de listagem mostra duas colunas, uma para o nome e outra para os dados.</span><span class="sxs-lookup"><span data-stu-id="8d4a8-149">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="8d4a8-150">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="8d4a8-150">The default value is false.</span></span>|
|<span data-ttu-id="8d4a8-151">valuePrefix</span><span class="sxs-lookup"><span data-stu-id="8d4a8-151">valuePrefix</span></span>|<span data-ttu-id="8d4a8-152">String</span><span class="sxs-lookup"><span data-stu-id="8d4a8-152">String</span></span>|<span data-ttu-id="8d4a8-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8d4a8-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8d4a8-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d4a8-154">Response</span></span>
<span data-ttu-id="8d4a8-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d4a8-155">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d4a8-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d4a8-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d4a8-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d4a8-157">Request</span></span>
<span data-ttu-id="8d4a8-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d4a8-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true,
  "valuePrefix": "Value Prefix value"
}
```

### <a name="response"></a><span data-ttu-id="8d4a8-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d4a8-159">Response</span></span>
<span data-ttu-id="8d4a8-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d4a8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "id": "2e074c87-4c87-2e07-874c-072e874c072e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "explicitValue": true,
  "valuePrefix": "Value Prefix value"
}
```



