---
title: Atualizar groupPolicyPresentationDropdownList
description: Atualiza as propriedades de um objeto groupPolicyPresentationDropdownList.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8706a55d7776c71f695e5e0b716a70bb78871f99
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464712"
---
# <a name="update-grouppolicypresentationdropdownlist"></a><span data-ttu-id="51cc0-103">Atualizar groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="51cc0-103">Update groupPolicyPresentationDropdownList</span></span>

<span data-ttu-id="51cc0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="51cc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51cc0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="51cc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51cc0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51cc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51cc0-107">Atualiza as propriedades de um objeto [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="51cc0-107">Update the properties of a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51cc0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51cc0-108">Prerequisites</span></span>
<span data-ttu-id="51cc0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51cc0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51cc0-111">Permission type</span></span>|<span data-ttu-id="51cc0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51cc0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51cc0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51cc0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51cc0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51cc0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="51cc0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51cc0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51cc0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51cc0-116">Not supported.</span></span>|
|<span data-ttu-id="51cc0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51cc0-117">Application</span></span>|<span data-ttu-id="51cc0-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51cc0-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51cc0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51cc0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="51cc0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51cc0-120">Request headers</span></span>
|<span data-ttu-id="51cc0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51cc0-121">Header</span></span>|<span data-ttu-id="51cc0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="51cc0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51cc0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="51cc0-123">Authorization</span></span>|<span data-ttu-id="51cc0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51cc0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51cc0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51cc0-125">Accept</span></span>|<span data-ttu-id="51cc0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51cc0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51cc0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51cc0-127">Request body</span></span>
<span data-ttu-id="51cc0-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="51cc0-128">In the request body, supply a JSON representation for the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

<span data-ttu-id="51cc0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span><span class="sxs-lookup"><span data-stu-id="51cc0-129">The following table shows the properties that are required when you create the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span></span>

|<span data-ttu-id="51cc0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51cc0-130">Property</span></span>|<span data-ttu-id="51cc0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="51cc0-131">Type</span></span>|<span data-ttu-id="51cc0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="51cc0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51cc0-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="51cc0-133">label</span></span>|<span data-ttu-id="51cc0-134">String</span><span class="sxs-lookup"><span data-stu-id="51cc0-134">String</span></span>|<span data-ttu-id="51cc0-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="51cc0-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="51cc0-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="51cc0-136">The default value is empty.</span></span> <span data-ttu-id="51cc0-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="51cc0-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="51cc0-138">id</span><span class="sxs-lookup"><span data-stu-id="51cc0-138">id</span></span>|<span data-ttu-id="51cc0-139">String</span><span class="sxs-lookup"><span data-stu-id="51cc0-139">String</span></span>|<span data-ttu-id="51cc0-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="51cc0-140">Key of the entity.</span></span> <span data-ttu-id="51cc0-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="51cc0-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="51cc0-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51cc0-142">lastModifiedDateTime</span></span>|<span data-ttu-id="51cc0-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51cc0-143">DateTimeOffset</span></span>|<span data-ttu-id="51cc0-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="51cc0-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="51cc0-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="51cc0-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="51cc0-146">DefaultItem</span><span class="sxs-lookup"><span data-stu-id="51cc0-146">defaultItem</span></span>|[<span data-ttu-id="51cc0-147">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="51cc0-147">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="51cc0-148">O valor da cadeia de caracteres localizada que identifica a opção padrão da lista de itens.</span><span class="sxs-lookup"><span data-stu-id="51cc0-148">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="51cc0-149">items</span><span class="sxs-lookup"><span data-stu-id="51cc0-149">items</span></span>|<span data-ttu-id="51cc0-150">coleção [groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)</span><span class="sxs-lookup"><span data-stu-id="51cc0-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="51cc0-151">Representa um conjunto de nomes de exibição localizados e seus valores associados.</span><span class="sxs-lookup"><span data-stu-id="51cc0-151">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="51cc0-152">obrigatório</span><span class="sxs-lookup"><span data-stu-id="51cc0-152">required</span></span>|<span data-ttu-id="51cc0-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="51cc0-153">Boolean</span></span>|<span data-ttu-id="51cc0-154">Requisito para inserir um valor na caixa parâmetro.</span><span class="sxs-lookup"><span data-stu-id="51cc0-154">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="51cc0-155">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="51cc0-155">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="51cc0-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="51cc0-156">Response</span></span>
<span data-ttu-id="51cc0-157">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51cc0-157">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51cc0-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51cc0-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="51cc0-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51cc0-159">Request</span></span>
<span data-ttu-id="51cc0-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51cc0-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="51cc0-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="51cc0-161">Response</span></span>
<span data-ttu-id="51cc0-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51cc0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





