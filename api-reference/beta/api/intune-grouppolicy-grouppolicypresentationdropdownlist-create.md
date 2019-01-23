---
title: Criar groupPolicyPresentationDropdownList
description: Crie um novo objeto de groupPolicyPresentationDropdownList.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 415ccd634e4206b2849fc5feecc4131d2f417d16
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431291"
---
# <a name="create-grouppolicypresentationdropdownlist"></a><span data-ttu-id="86479-103">Criar groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="86479-103">Create groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="86479-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="86479-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="86479-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="86479-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86479-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="86479-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86479-107">Crie um novo objeto de [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="86479-107">Create a new [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86479-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86479-108">Prerequisites</span></span>
<span data-ttu-id="86479-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="86479-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="86479-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86479-111">Permission type</span></span>|<span data-ttu-id="86479-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86479-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86479-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86479-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86479-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86479-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="86479-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86479-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86479-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86479-116">Not supported.</span></span>|
|<span data-ttu-id="86479-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86479-117">Application</span></span>|<span data-ttu-id="86479-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86479-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86479-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86479-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="86479-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86479-120">Request headers</span></span>
|<span data-ttu-id="86479-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86479-121">Header</span></span>|<span data-ttu-id="86479-122">Valor</span><span class="sxs-lookup"><span data-stu-id="86479-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86479-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="86479-123">Authorization</span></span>|<span data-ttu-id="86479-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86479-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86479-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86479-125">Accept</span></span>|<span data-ttu-id="86479-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86479-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86479-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86479-127">Request body</span></span>
<span data-ttu-id="86479-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationDropdownList.</span><span class="sxs-lookup"><span data-stu-id="86479-128">In the request body, supply a JSON representation for the groupPolicyPresentationDropdownList object.</span></span>

<span data-ttu-id="86479-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o groupPolicyPresentationDropdownList.</span><span class="sxs-lookup"><span data-stu-id="86479-129">The following table shows the properties that are required when you create the groupPolicyPresentationDropdownList.</span></span>

|<span data-ttu-id="86479-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86479-130">Property</span></span>|<span data-ttu-id="86479-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="86479-131">Type</span></span>|<span data-ttu-id="86479-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="86479-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86479-133">rótulo</span><span class="sxs-lookup"><span data-stu-id="86479-133">label</span></span>|<span data-ttu-id="86479-134">String</span><span class="sxs-lookup"><span data-stu-id="86479-134">String</span></span>|<span data-ttu-id="86479-135">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="86479-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="86479-136">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="86479-136">The default value is empty.</span></span> <span data-ttu-id="86479-137">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="86479-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="86479-138">id</span><span class="sxs-lookup"><span data-stu-id="86479-138">id</span></span>|<span data-ttu-id="86479-139">String</span><span class="sxs-lookup"><span data-stu-id="86479-139">String</span></span>|<span data-ttu-id="86479-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="86479-140">Key of the entity.</span></span> <span data-ttu-id="86479-141">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="86479-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="86479-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86479-142">lastModifiedDateTime</span></span>|<span data-ttu-id="86479-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86479-143">DateTimeOffset</span></span>|<span data-ttu-id="86479-144">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="86479-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="86479-145">Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="86479-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="86479-146">defaultItem</span><span class="sxs-lookup"><span data-stu-id="86479-146">defaultItem</span></span>|[<span data-ttu-id="86479-147">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="86479-147">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="86479-148">Valor de cadeia de caracteres localizada que identifica a opção padrão da lista de itens.</span><span class="sxs-lookup"><span data-stu-id="86479-148">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="86479-149">items</span><span class="sxs-lookup"><span data-stu-id="86479-149">items</span></span>|<span data-ttu-id="86479-150">coleção [groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)</span><span class="sxs-lookup"><span data-stu-id="86479-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="86479-151">Representa um conjunto de nomes de exibição localizado e seus valores associados.</span><span class="sxs-lookup"><span data-stu-id="86479-151">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="86479-152">obrigatório</span><span class="sxs-lookup"><span data-stu-id="86479-152">required</span></span>|<span data-ttu-id="86479-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="86479-153">Boolean</span></span>|<span data-ttu-id="86479-154">Requisito para inserir um valor na caixa de parâmetro.</span><span class="sxs-lookup"><span data-stu-id="86479-154">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="86479-155">O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="86479-155">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="86479-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="86479-156">Response</span></span>
<span data-ttu-id="86479-157">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86479-157">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86479-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86479-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="86479-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86479-159">Request</span></span>
<span data-ttu-id="86479-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86479-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="86479-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="86479-161">Response</span></span>
<span data-ttu-id="86479-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86479-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




