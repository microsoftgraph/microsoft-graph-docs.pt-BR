---
title: Atualizar groupPolicyPresentationDropdownList
description: Atualiza as propriedades de um objeto groupPolicyPresentationDropdownList.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f42445ac5fec2f52aa2d51f560d7c29f0f6ebcc9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457825"
---
# <a name="update-grouppolicypresentationdropdownlist"></a><span data-ttu-id="850cf-103">Atualizar groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="850cf-103">Update groupPolicyPresentationDropdownList</span></span>

<span data-ttu-id="850cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="850cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="850cf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="850cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="850cf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="850cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="850cf-107">Atualiza as propriedades de um objeto [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="850cf-107">Update the properties of a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="850cf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="850cf-108">Prerequisites</span></span>
<span data-ttu-id="850cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="850cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="850cf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="850cf-111">Permission type</span></span>|<span data-ttu-id="850cf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="850cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="850cf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="850cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="850cf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="850cf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="850cf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="850cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="850cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="850cf-116">Not supported.</span></span>|
|<span data-ttu-id="850cf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="850cf-117">Application</span></span>|<span data-ttu-id="850cf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="850cf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="850cf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="850cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="850cf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="850cf-120">Request headers</span></span>
|<span data-ttu-id="850cf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="850cf-121">Header</span></span>|<span data-ttu-id="850cf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="850cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="850cf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="850cf-123">Authorization</span></span>|<span data-ttu-id="850cf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="850cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="850cf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="850cf-125">Accept</span></span>|<span data-ttu-id="850cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="850cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="850cf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="850cf-127">Request body</span></span>
<span data-ttu-id="850cf-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="850cf-128">In the request body, supply a JSON representation for the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

<span data-ttu-id="850cf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span><span class="sxs-lookup"><span data-stu-id="850cf-129">The following table shows the properties that are required when you create the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span></span>

|<span data-ttu-id="850cf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="850cf-130">Property</span></span>|<span data-ttu-id="850cf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="850cf-131">Type</span></span>|<span data-ttu-id="850cf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="850cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="850cf-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="850cf-133">label</span></span>|<span data-ttu-id="850cf-134">String</span><span class="sxs-lookup"><span data-stu-id="850cf-134">String</span></span>|<span data-ttu-id="850cf-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="850cf-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="850cf-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="850cf-136">The default value is empty.</span></span> <span data-ttu-id="850cf-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="850cf-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="850cf-138">id</span><span class="sxs-lookup"><span data-stu-id="850cf-138">id</span></span>|<span data-ttu-id="850cf-139">String</span><span class="sxs-lookup"><span data-stu-id="850cf-139">String</span></span>|<span data-ttu-id="850cf-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="850cf-140">Key of the entity.</span></span> <span data-ttu-id="850cf-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="850cf-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="850cf-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="850cf-142">lastModifiedDateTime</span></span>|<span data-ttu-id="850cf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="850cf-143">DateTimeOffset</span></span>|<span data-ttu-id="850cf-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="850cf-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="850cf-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="850cf-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="850cf-146">DefaultItem</span><span class="sxs-lookup"><span data-stu-id="850cf-146">defaultItem</span></span>|[<span data-ttu-id="850cf-147">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="850cf-147">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="850cf-148">O valor da cadeia de caracteres localizada que identifica a opção padrão da lista de itens.</span><span class="sxs-lookup"><span data-stu-id="850cf-148">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="850cf-149">items</span><span class="sxs-lookup"><span data-stu-id="850cf-149">items</span></span>|<span data-ttu-id="850cf-150">coleção [groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)</span><span class="sxs-lookup"><span data-stu-id="850cf-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="850cf-151">Representa um conjunto de nomes de exibição localizados e seus valores associados.</span><span class="sxs-lookup"><span data-stu-id="850cf-151">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="850cf-152">obrigatório</span><span class="sxs-lookup"><span data-stu-id="850cf-152">required</span></span>|<span data-ttu-id="850cf-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="850cf-153">Boolean</span></span>|<span data-ttu-id="850cf-154">Requisito para inserir um valor na caixa parâmetro.</span><span class="sxs-lookup"><span data-stu-id="850cf-154">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="850cf-155">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="850cf-155">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="850cf-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="850cf-156">Response</span></span>
<span data-ttu-id="850cf-157">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="850cf-157">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="850cf-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="850cf-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="850cf-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="850cf-159">Request</span></span>
<span data-ttu-id="850cf-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="850cf-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
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

### <a name="response"></a><span data-ttu-id="850cf-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="850cf-161">Response</span></span>
<span data-ttu-id="850cf-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="850cf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



