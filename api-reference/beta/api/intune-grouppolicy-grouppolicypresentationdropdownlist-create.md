---
title: Criar groupPolicyPresentationDropdownList
description: Criar um novo objeto groupPolicyPresentationDropdownList.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f8d9ade33a1fee4173bd7f5d873a3ee0262566a9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464803"
---
# <a name="create-grouppolicypresentationdropdownlist"></a><span data-ttu-id="3b0f5-103">Criar groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="3b0f5-103">Create groupPolicyPresentationDropdownList</span></span>

<span data-ttu-id="3b0f5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3b0f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b0f5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b0f5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b0f5-107">Criar um novo objeto [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="3b0f5-107">Create a new [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b0f5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b0f5-108">Prerequisites</span></span>
<span data-ttu-id="3b0f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b0f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b0f5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b0f5-111">Permission type</span></span>|<span data-ttu-id="3b0f5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b0f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b0f5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b0f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b0f5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b0f5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3b0f5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b0f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b0f5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-116">Not supported.</span></span>|
|<span data-ttu-id="3b0f5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b0f5-117">Application</span></span>|<span data-ttu-id="3b0f5-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b0f5-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b0f5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b0f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="3b0f5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b0f5-120">Request headers</span></span>
|<span data-ttu-id="3b0f5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b0f5-121">Header</span></span>|<span data-ttu-id="3b0f5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3b0f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b0f5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b0f5-123">Authorization</span></span>|<span data-ttu-id="3b0f5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b0f5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b0f5-125">Accept</span></span>|<span data-ttu-id="3b0f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b0f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b0f5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b0f5-127">Request body</span></span>
<span data-ttu-id="3b0f5-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationDropdownList.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-128">In the request body, supply a JSON representation for the groupPolicyPresentationDropdownList object.</span></span>

<span data-ttu-id="3b0f5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationDropdownList.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-129">The following table shows the properties that are required when you create the groupPolicyPresentationDropdownList.</span></span>

|<span data-ttu-id="3b0f5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b0f5-130">Property</span></span>|<span data-ttu-id="3b0f5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b0f5-131">Type</span></span>|<span data-ttu-id="3b0f5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b0f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b0f5-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="3b0f5-133">label</span></span>|<span data-ttu-id="3b0f5-134">String</span><span class="sxs-lookup"><span data-stu-id="3b0f5-134">String</span></span>|<span data-ttu-id="3b0f5-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="3b0f5-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-136">The default value is empty.</span></span> <span data-ttu-id="3b0f5-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3b0f5-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3b0f5-138">id</span><span class="sxs-lookup"><span data-stu-id="3b0f5-138">id</span></span>|<span data-ttu-id="3b0f5-139">String</span><span class="sxs-lookup"><span data-stu-id="3b0f5-139">String</span></span>|<span data-ttu-id="3b0f5-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-140">Key of the entity.</span></span> <span data-ttu-id="3b0f5-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3b0f5-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3b0f5-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b0f5-142">lastModifiedDateTime</span></span>|<span data-ttu-id="3b0f5-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b0f5-143">DateTimeOffset</span></span>|<span data-ttu-id="3b0f5-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="3b0f5-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3b0f5-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3b0f5-146">DefaultItem</span><span class="sxs-lookup"><span data-stu-id="3b0f5-146">defaultItem</span></span>|[<span data-ttu-id="3b0f5-147">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="3b0f5-147">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="3b0f5-148">O valor da cadeia de caracteres localizada que identifica a opção padrão da lista de itens.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-148">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="3b0f5-149">items</span><span class="sxs-lookup"><span data-stu-id="3b0f5-149">items</span></span>|<span data-ttu-id="3b0f5-150">coleção [groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)</span><span class="sxs-lookup"><span data-stu-id="3b0f5-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="3b0f5-151">Representa um conjunto de nomes de exibição localizados e seus valores associados.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-151">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="3b0f5-152">obrigatório</span><span class="sxs-lookup"><span data-stu-id="3b0f5-152">required</span></span>|<span data-ttu-id="3b0f5-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0f5-153">Boolean</span></span>|<span data-ttu-id="3b0f5-154">Requisito para inserir um valor na caixa parâmetro.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-154">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="3b0f5-155">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-155">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="3b0f5-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b0f5-156">Response</span></span>
<span data-ttu-id="3b0f5-157">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-157">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b0f5-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b0f5-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b0f5-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b0f5-159">Request</span></span>
<span data-ttu-id="3b0f5-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 489

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    }
  ],
  "required": true
}
```

### <a name="response"></a><span data-ttu-id="3b0f5-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b0f5-161">Response</span></span>
<span data-ttu-id="3b0f5-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b0f5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 602

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "id": "ba3ff7c9-f7c9-ba3f-c9f7-3fbac9f73fba",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    }
  ],
  "required": true
}
```





