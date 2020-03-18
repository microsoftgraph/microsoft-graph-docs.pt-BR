---
title: Atualizar groupPolicyUploadedCategory
description: Atualiza as propriedades de um objeto groupPolicyUploadedCategory.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 148c698c6bbc466fc4aef10bb62b09f61386f362
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803768"
---
# <a name="update-grouppolicyuploadedcategory"></a><span data-ttu-id="df0cf-103">Atualizar groupPolicyUploadedCategory</span><span class="sxs-lookup"><span data-stu-id="df0cf-103">Update groupPolicyUploadedCategory</span></span>

> <span data-ttu-id="df0cf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="df0cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df0cf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df0cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df0cf-106">Atualiza as propriedades de um objeto [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="df0cf-106">Update the properties of a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df0cf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df0cf-107">Prerequisites</span></span>
<span data-ttu-id="df0cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df0cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df0cf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df0cf-110">Permission type</span></span>|<span data-ttu-id="df0cf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df0cf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df0cf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df0cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df0cf-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df0cf-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="df0cf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df0cf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df0cf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df0cf-115">Not supported.</span></span>|
|<span data-ttu-id="df0cf-116">Application</span><span class="sxs-lookup"><span data-stu-id="df0cf-116">Application</span></span>|<span data-ttu-id="df0cf-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df0cf-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df0cf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df0cf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/parent
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/children/{groupPolicyCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="df0cf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df0cf-119">Request headers</span></span>
|<span data-ttu-id="df0cf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df0cf-120">Header</span></span>|<span data-ttu-id="df0cf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="df0cf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df0cf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="df0cf-122">Authorization</span></span>|<span data-ttu-id="df0cf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df0cf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df0cf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df0cf-124">Accept</span></span>|<span data-ttu-id="df0cf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df0cf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df0cf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df0cf-126">Request body</span></span>
<span data-ttu-id="df0cf-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="df0cf-127">In the request body, supply a JSON representation for the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

<span data-ttu-id="df0cf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span><span class="sxs-lookup"><span data-stu-id="df0cf-128">The following table shows the properties that are required when you create the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span></span>

|<span data-ttu-id="df0cf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df0cf-129">Property</span></span>|<span data-ttu-id="df0cf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="df0cf-130">Type</span></span>|<span data-ttu-id="df0cf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="df0cf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df0cf-132">displayName</span><span class="sxs-lookup"><span data-stu-id="df0cf-132">displayName</span></span>|<span data-ttu-id="df0cf-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df0cf-133">String</span></span>|<span data-ttu-id="df0cf-134">A ID da cadeia de caracteres do nome de exibição da categoria herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="df0cf-134">The string id of the category's display name Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="df0cf-135">IsRoot</span><span class="sxs-lookup"><span data-stu-id="df0cf-135">isRoot</span></span>|<span data-ttu-id="df0cf-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="df0cf-136">Boolean</span></span>|<span data-ttu-id="df0cf-137">Define se a categoria é uma categoria raiz herdada de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="df0cf-137">Defines if the category is a root category Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="df0cf-138">id</span><span class="sxs-lookup"><span data-stu-id="df0cf-138">id</span></span>|<span data-ttu-id="df0cf-139">String</span><span class="sxs-lookup"><span data-stu-id="df0cf-139">String</span></span>|<span data-ttu-id="df0cf-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="df0cf-140">Key of the entity.</span></span> <span data-ttu-id="df0cf-141">Herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="df0cf-141">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="df0cf-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df0cf-142">lastModifiedDateTime</span></span>|<span data-ttu-id="df0cf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df0cf-143">DateTimeOffset</span></span>|<span data-ttu-id="df0cf-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="df0cf-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="df0cf-145">Herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="df0cf-145">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="df0cf-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="df0cf-146">Response</span></span>
<span data-ttu-id="df0cf-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df0cf-147">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df0cf-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df0cf-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="df0cf-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df0cf-149">Request</span></span>
<span data-ttu-id="df0cf-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df0cf-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
  "displayName": "Display Name value",
  "isRoot": true
}
```

### <a name="response"></a><span data-ttu-id="df0cf-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="df0cf-151">Response</span></span>
<span data-ttu-id="df0cf-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df0cf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 241

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
  "displayName": "Display Name value",
  "isRoot": true,
  "id": "7e373e80-3e80-7e37-803e-377e803e377e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




