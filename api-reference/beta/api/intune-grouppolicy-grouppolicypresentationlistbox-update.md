---
title: Atualizar groupPolicyPresentationListBox
description: Atualiza as propriedades de um objeto groupPolicyPresentationListBox.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8876cc7185ce8c7a2ab0ae1db84ff1bc0bd506a9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33904787"
---
# <a name="update-grouppolicypresentationlistbox"></a><span data-ttu-id="4533c-103">Atualizar groupPolicyPresentationListBox</span><span class="sxs-lookup"><span data-stu-id="4533c-103">Update groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="4533c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4533c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4533c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4533c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4533c-106">Atualiza as propriedades de um objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="4533c-106">Update the properties of a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4533c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4533c-107">Prerequisites</span></span>
<span data-ttu-id="4533c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4533c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4533c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4533c-110">Permission type</span></span>|<span data-ttu-id="4533c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4533c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4533c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4533c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4533c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4533c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4533c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4533c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4533c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4533c-115">Not supported.</span></span>|
|<span data-ttu-id="4533c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4533c-116">Application</span></span>|<span data-ttu-id="4533c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4533c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4533c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4533c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="4533c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4533c-119">Request headers</span></span>
|<span data-ttu-id="4533c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4533c-120">Header</span></span>|<span data-ttu-id="4533c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4533c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4533c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4533c-122">Authorization</span></span>|<span data-ttu-id="4533c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4533c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4533c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4533c-124">Accept</span></span>|<span data-ttu-id="4533c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4533c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4533c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4533c-126">Request body</span></span>
<span data-ttu-id="4533c-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="4533c-127">In the request body, supply a JSON representation for the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

<span data-ttu-id="4533c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span><span class="sxs-lookup"><span data-stu-id="4533c-128">The following table shows the properties that are required when you create the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span></span>

|<span data-ttu-id="4533c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4533c-129">Property</span></span>|<span data-ttu-id="4533c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4533c-130">Type</span></span>|<span data-ttu-id="4533c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4533c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4533c-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="4533c-132">label</span></span>|<span data-ttu-id="4533c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4533c-133">String</span></span>|<span data-ttu-id="4533c-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="4533c-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="4533c-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="4533c-135">The default value is empty.</span></span> <span data-ttu-id="4533c-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="4533c-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="4533c-137">id</span><span class="sxs-lookup"><span data-stu-id="4533c-137">id</span></span>|<span data-ttu-id="4533c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4533c-138">String</span></span>|<span data-ttu-id="4533c-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4533c-139">Key of the entity.</span></span> <span data-ttu-id="4533c-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="4533c-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="4533c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4533c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="4533c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4533c-142">DateTimeOffset</span></span>|<span data-ttu-id="4533c-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4533c-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="4533c-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="4533c-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="4533c-145">explicitValue</span><span class="sxs-lookup"><span data-stu-id="4533c-145">explicitValue</span></span>|<span data-ttu-id="4533c-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="4533c-146">Boolean</span></span>|<span data-ttu-id="4533c-147">Se essa opção for especificada true, o usuário deverá especificar o valor da subchave do registro e o nome da subchave do registro.</span><span class="sxs-lookup"><span data-stu-id="4533c-147">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="4533c-148">A caixa de listagem mostra duas colunas, uma para o nome e outra para os dados.</span><span class="sxs-lookup"><span data-stu-id="4533c-148">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="4533c-149">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="4533c-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="4533c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="4533c-150">Response</span></span>
<span data-ttu-id="4533c-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4533c-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4533c-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4533c-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="4533c-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4533c-153">Request</span></span>
<span data-ttu-id="4533c-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4533c-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true
}
```

### <a name="response"></a><span data-ttu-id="4533c-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="4533c-155">Response</span></span>
<span data-ttu-id="4533c-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4533c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "id": "2e074c87-4c87-2e07-874c-072e874c072e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "explicitValue": true
}
```




