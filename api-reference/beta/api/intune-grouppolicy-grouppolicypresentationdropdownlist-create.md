---
title: Criar groupPolicyPresentationDropdownList
description: Criar um novo objeto groupPolicyPresentationDropdownList.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53614e7171476acd1383bfc6ec96f6b339846569
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790876"
---
# <a name="create-grouppolicypresentationdropdownlist"></a><span data-ttu-id="67c29-103">Criar groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="67c29-103">Create groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="67c29-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67c29-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67c29-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67c29-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67c29-106">Criar um novo objeto [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="67c29-106">Create a new [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67c29-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67c29-107">Prerequisites</span></span>
<span data-ttu-id="67c29-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67c29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67c29-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67c29-110">Permission type</span></span>|<span data-ttu-id="67c29-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67c29-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67c29-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67c29-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67c29-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67c29-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="67c29-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67c29-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67c29-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67c29-115">Not supported.</span></span>|
|<span data-ttu-id="67c29-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67c29-116">Application</span></span>|<span data-ttu-id="67c29-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67c29-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67c29-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67c29-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="67c29-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67c29-119">Request headers</span></span>
|<span data-ttu-id="67c29-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67c29-120">Header</span></span>|<span data-ttu-id="67c29-121">Valor</span><span class="sxs-lookup"><span data-stu-id="67c29-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67c29-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="67c29-122">Authorization</span></span>|<span data-ttu-id="67c29-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67c29-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67c29-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67c29-124">Accept</span></span>|<span data-ttu-id="67c29-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67c29-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67c29-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67c29-126">Request body</span></span>
<span data-ttu-id="67c29-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationDropdownList.</span><span class="sxs-lookup"><span data-stu-id="67c29-127">In the request body, supply a JSON representation for the groupPolicyPresentationDropdownList object.</span></span>

<span data-ttu-id="67c29-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationDropdownList.</span><span class="sxs-lookup"><span data-stu-id="67c29-128">The following table shows the properties that are required when you create the groupPolicyPresentationDropdownList.</span></span>

|<span data-ttu-id="67c29-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67c29-129">Property</span></span>|<span data-ttu-id="67c29-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="67c29-130">Type</span></span>|<span data-ttu-id="67c29-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="67c29-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67c29-132">rótulo</span><span class="sxs-lookup"><span data-stu-id="67c29-132">label</span></span>|<span data-ttu-id="67c29-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67c29-133">String</span></span>|<span data-ttu-id="67c29-134">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="67c29-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="67c29-135">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="67c29-135">The default value is empty.</span></span> <span data-ttu-id="67c29-136">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="67c29-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="67c29-137">id</span><span class="sxs-lookup"><span data-stu-id="67c29-137">id</span></span>|<span data-ttu-id="67c29-138">String</span><span class="sxs-lookup"><span data-stu-id="67c29-138">String</span></span>|<span data-ttu-id="67c29-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="67c29-139">Key of the entity.</span></span> <span data-ttu-id="67c29-140">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="67c29-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="67c29-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67c29-141">lastModifiedDateTime</span></span>|<span data-ttu-id="67c29-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67c29-142">DateTimeOffset</span></span>|<span data-ttu-id="67c29-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="67c29-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="67c29-144">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="67c29-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="67c29-145">DefaultItem</span><span class="sxs-lookup"><span data-stu-id="67c29-145">defaultItem</span></span>|[<span data-ttu-id="67c29-146">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="67c29-146">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="67c29-147">O valor da cadeia de caracteres localizada que identifica a opção padrão da lista de itens.</span><span class="sxs-lookup"><span data-stu-id="67c29-147">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="67c29-148">items</span><span class="sxs-lookup"><span data-stu-id="67c29-148">items</span></span>|<span data-ttu-id="67c29-149">coleção [groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)</span><span class="sxs-lookup"><span data-stu-id="67c29-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="67c29-150">Representa um conjunto de nomes de exibição localizados e seus valores associados.</span><span class="sxs-lookup"><span data-stu-id="67c29-150">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="67c29-151">obrigatório</span><span class="sxs-lookup"><span data-stu-id="67c29-151">required</span></span>|<span data-ttu-id="67c29-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="67c29-152">Boolean</span></span>|<span data-ttu-id="67c29-153">Requisito para inserir um valor na caixa parâmetro.</span><span class="sxs-lookup"><span data-stu-id="67c29-153">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="67c29-154">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="67c29-154">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="67c29-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="67c29-155">Response</span></span>
<span data-ttu-id="67c29-156">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67c29-156">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67c29-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67c29-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="67c29-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67c29-158">Request</span></span>
<span data-ttu-id="67c29-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67c29-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="67c29-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="67c29-160">Response</span></span>
<span data-ttu-id="67c29-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67c29-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





