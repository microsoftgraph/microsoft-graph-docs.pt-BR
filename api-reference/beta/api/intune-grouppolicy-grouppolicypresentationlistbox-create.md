---
title: Criar groupPolicyPresentationListBox
description: Criar um novo objeto groupPolicyPresentationListBox.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5de84a8867e14737611b6d10ab7d2c69159e22b2
ms.sourcegitcommit: 705b32b9a64516d8138fab34c173b7df4f78a6ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/05/2019
ms.locfileid: "35576470"
---
# <a name="create-grouppolicypresentationlistbox"></a><span data-ttu-id="6fa20-103">Criar groupPolicyPresentationListBox</span><span class="sxs-lookup"><span data-stu-id="6fa20-103">Create groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="6fa20-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6fa20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fa20-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6fa20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fa20-106">Criar um novo objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="6fa20-106">Create a new [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fa20-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6fa20-107">Prerequisites</span></span>
<span data-ttu-id="6fa20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fa20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fa20-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fa20-110">Permission type</span></span>|<span data-ttu-id="6fa20-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6fa20-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fa20-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fa20-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6fa20-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fa20-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6fa20-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fa20-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fa20-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fa20-115">Not supported.</span></span>|
|<span data-ttu-id="6fa20-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fa20-116">Application</span></span>|<span data-ttu-id="6fa20-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fa20-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fa20-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fa20-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="6fa20-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fa20-119">Request headers</span></span>
|<span data-ttu-id="6fa20-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6fa20-120">Header</span></span>|<span data-ttu-id="6fa20-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6fa20-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fa20-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fa20-122">Authorization</span></span>|<span data-ttu-id="6fa20-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fa20-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fa20-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6fa20-124">Accept</span></span>|<span data-ttu-id="6fa20-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6fa20-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fa20-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fa20-126">Request body</span></span>
<span data-ttu-id="6fa20-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationListBox.</span><span class="sxs-lookup"><span data-stu-id="6fa20-127">In the request body, supply a JSON representation for the groupPolicyPresentationListBox object.</span></span>

<span data-ttu-id="6fa20-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationListBox.</span><span class="sxs-lookup"><span data-stu-id="6fa20-128">The following table shows the properties that are required when you create the groupPolicyPresentationListBox.</span></span>

|<span data-ttu-id="6fa20-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fa20-129">Property</span></span>|<span data-ttu-id="6fa20-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fa20-130">Type</span></span>|<span data-ttu-id="6fa20-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fa20-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fa20-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="6fa20-132">label</span></span>|<span data-ttu-id="6fa20-133">String</span><span class="sxs-lookup"><span data-stu-id="6fa20-133">String</span></span>|<span data-ttu-id="6fa20-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="6fa20-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="6fa20-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="6fa20-135">The default value is empty.</span></span> <span data-ttu-id="6fa20-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6fa20-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6fa20-137">id</span><span class="sxs-lookup"><span data-stu-id="6fa20-137">id</span></span>|<span data-ttu-id="6fa20-138">String</span><span class="sxs-lookup"><span data-stu-id="6fa20-138">String</span></span>|<span data-ttu-id="6fa20-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6fa20-139">Key of the entity.</span></span> <span data-ttu-id="6fa20-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6fa20-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6fa20-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fa20-141">lastModifiedDateTime</span></span>|<span data-ttu-id="6fa20-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fa20-142">DateTimeOffset</span></span>|<span data-ttu-id="6fa20-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6fa20-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="6fa20-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6fa20-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6fa20-145">explicitValue</span><span class="sxs-lookup"><span data-stu-id="6fa20-145">explicitValue</span></span>|<span data-ttu-id="6fa20-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="6fa20-146">Boolean</span></span>|<span data-ttu-id="6fa20-147">Se essa opção for especificada true, o usuário deverá especificar o valor da subchave do registro e o nome da subchave do registro.</span><span class="sxs-lookup"><span data-stu-id="6fa20-147">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="6fa20-148">A caixa de listagem mostra duas colunas, uma para o nome e outra para os dados.</span><span class="sxs-lookup"><span data-stu-id="6fa20-148">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="6fa20-149">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="6fa20-149">The default value is false.</span></span>|
|<span data-ttu-id="6fa20-150">valuePrefix</span><span class="sxs-lookup"><span data-stu-id="6fa20-150">valuePrefix</span></span>|<span data-ttu-id="6fa20-151">String</span><span class="sxs-lookup"><span data-stu-id="6fa20-151">String</span></span>|<span data-ttu-id="6fa20-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6fa20-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6fa20-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fa20-153">Response</span></span>
<span data-ttu-id="6fa20-154">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fa20-154">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fa20-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fa20-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fa20-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fa20-156">Request</span></span>
<span data-ttu-id="6fa20-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fa20-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6fa20-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fa20-158">Response</span></span>
<span data-ttu-id="6fa20-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6fa20-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



