---
title: Criar groupPolicyPresentationListBox
description: Crie um novo objeto groupPolicyPresentationListBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 561a591e61ef5d6872f2eec63c24964b7827ce43
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135387"
---
# <a name="create-grouppolicypresentationlistbox"></a><span data-ttu-id="54dd0-103">Criar groupPolicyPresentationListBox</span><span class="sxs-lookup"><span data-stu-id="54dd0-103">Create groupPolicyPresentationListBox</span></span>

<span data-ttu-id="54dd0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54dd0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54dd0-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54dd0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54dd0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54dd0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54dd0-107">Crie um novo [objeto groupPolicyPresentationListBox.](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)</span><span class="sxs-lookup"><span data-stu-id="54dd0-107">Create a new [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54dd0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54dd0-108">Prerequisites</span></span>
<span data-ttu-id="54dd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54dd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54dd0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54dd0-111">Permission type</span></span>|<span data-ttu-id="54dd0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54dd0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54dd0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54dd0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54dd0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54dd0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54dd0-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54dd0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54dd0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54dd0-116">Not supported.</span></span>|
|<span data-ttu-id="54dd0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54dd0-117">Application</span></span>|<span data-ttu-id="54dd0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54dd0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54dd0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54dd0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="54dd0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54dd0-120">Request headers</span></span>
|<span data-ttu-id="54dd0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54dd0-121">Header</span></span>|<span data-ttu-id="54dd0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="54dd0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54dd0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="54dd0-123">Authorization</span></span>|<span data-ttu-id="54dd0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54dd0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54dd0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54dd0-125">Accept</span></span>|<span data-ttu-id="54dd0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54dd0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54dd0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54dd0-127">Request body</span></span>
<span data-ttu-id="54dd0-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationListBox.</span><span class="sxs-lookup"><span data-stu-id="54dd0-128">In the request body, supply a JSON representation for the groupPolicyPresentationListBox object.</span></span>

<span data-ttu-id="54dd0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyPresentationListBox.</span><span class="sxs-lookup"><span data-stu-id="54dd0-129">The following table shows the properties that are required when you create the groupPolicyPresentationListBox.</span></span>

|<span data-ttu-id="54dd0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54dd0-130">Property</span></span>|<span data-ttu-id="54dd0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="54dd0-131">Type</span></span>|<span data-ttu-id="54dd0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="54dd0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54dd0-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="54dd0-133">label</span></span>|<span data-ttu-id="54dd0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54dd0-134">String</span></span>|<span data-ttu-id="54dd0-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="54dd0-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="54dd0-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="54dd0-136">The default value is empty.</span></span> <span data-ttu-id="54dd0-137">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="54dd0-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="54dd0-138">id</span><span class="sxs-lookup"><span data-stu-id="54dd0-138">id</span></span>|<span data-ttu-id="54dd0-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54dd0-139">String</span></span>|<span data-ttu-id="54dd0-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="54dd0-140">Key of the entity.</span></span> <span data-ttu-id="54dd0-141">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="54dd0-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="54dd0-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54dd0-142">lastModifiedDateTime</span></span>|<span data-ttu-id="54dd0-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54dd0-143">DateTimeOffset</span></span>|<span data-ttu-id="54dd0-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="54dd0-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="54dd0-145">Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="54dd0-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="54dd0-146">explicitValue</span><span class="sxs-lookup"><span data-stu-id="54dd0-146">explicitValue</span></span>|<span data-ttu-id="54dd0-147">Booleano</span><span class="sxs-lookup"><span data-stu-id="54dd0-147">Boolean</span></span>|<span data-ttu-id="54dd0-148">Se essa opção for especificada como true, o usuário deverá especificar o valor da sub-chave do Registro e o nome da sub-chave do Registro.</span><span class="sxs-lookup"><span data-stu-id="54dd0-148">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="54dd0-149">A caixa de listagem mostra duas colunas, uma para o nome e outra para os dados.</span><span class="sxs-lookup"><span data-stu-id="54dd0-149">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="54dd0-150">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="54dd0-150">The default value is false.</span></span>|
|<span data-ttu-id="54dd0-151">valuePrefix</span><span class="sxs-lookup"><span data-stu-id="54dd0-151">valuePrefix</span></span>|<span data-ttu-id="54dd0-152">String</span><span class="sxs-lookup"><span data-stu-id="54dd0-152">String</span></span>|<span data-ttu-id="54dd0-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="54dd0-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="54dd0-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="54dd0-154">Response</span></span>
<span data-ttu-id="54dd0-155">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54dd0-155">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54dd0-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54dd0-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="54dd0-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54dd0-157">Request</span></span>
<span data-ttu-id="54dd0-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54dd0-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true,
  "valuePrefix": "Value Prefix value"
}
```

### <a name="response"></a><span data-ttu-id="54dd0-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="54dd0-159">Response</span></span>
<span data-ttu-id="54dd0-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54dd0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




