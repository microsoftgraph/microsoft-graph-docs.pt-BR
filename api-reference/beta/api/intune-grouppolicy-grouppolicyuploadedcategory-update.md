---
title: Atualizar groupPolicyUploadedCategory
description: Atualiza as propriedades de um objeto groupPolicyUploadedCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 03d6bdffff214ad7e095475adbd116644029a5bd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735404"
---
# <a name="update-grouppolicyuploadedcategory"></a><span data-ttu-id="5e137-103">Atualizar groupPolicyUploadedCategory</span><span class="sxs-lookup"><span data-stu-id="5e137-103">Update groupPolicyUploadedCategory</span></span>

<span data-ttu-id="5e137-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e137-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e137-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5e137-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e137-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e137-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e137-107">Atualiza as propriedades de um objeto [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="5e137-107">Update the properties of a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e137-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e137-108">Prerequisites</span></span>
<span data-ttu-id="5e137-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e137-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e137-111">Permission type</span></span>|<span data-ttu-id="5e137-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5e137-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e137-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e137-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e137-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e137-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5e137-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e137-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e137-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e137-116">Not supported.</span></span>|
|<span data-ttu-id="5e137-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e137-117">Application</span></span>|<span data-ttu-id="5e137-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e137-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e137-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e137-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5e137-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e137-120">Request headers</span></span>
|<span data-ttu-id="5e137-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e137-121">Header</span></span>|<span data-ttu-id="5e137-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5e137-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e137-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e137-123">Authorization</span></span>|<span data-ttu-id="5e137-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e137-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e137-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5e137-125">Accept</span></span>|<span data-ttu-id="5e137-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e137-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e137-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e137-127">Request body</span></span>
<span data-ttu-id="5e137-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="5e137-128">In the request body, supply a JSON representation for the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

<span data-ttu-id="5e137-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span><span class="sxs-lookup"><span data-stu-id="5e137-129">The following table shows the properties that are required when you create the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span></span>

|<span data-ttu-id="5e137-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e137-130">Property</span></span>|<span data-ttu-id="5e137-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e137-131">Type</span></span>|<span data-ttu-id="5e137-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e137-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e137-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5e137-133">displayName</span></span>|<span data-ttu-id="5e137-134">String</span><span class="sxs-lookup"><span data-stu-id="5e137-134">String</span></span>|<span data-ttu-id="5e137-135">A ID da cadeia de caracteres do nome de exibição da categoria herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="5e137-135">The string id of the category's display name Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="5e137-136">IsRoot</span><span class="sxs-lookup"><span data-stu-id="5e137-136">isRoot</span></span>|<span data-ttu-id="5e137-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="5e137-137">Boolean</span></span>|<span data-ttu-id="5e137-138">Define se a categoria é uma categoria raiz herdada de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="5e137-138">Defines if the category is a root category Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="5e137-139">id</span><span class="sxs-lookup"><span data-stu-id="5e137-139">id</span></span>|<span data-ttu-id="5e137-140">String</span><span class="sxs-lookup"><span data-stu-id="5e137-140">String</span></span>|<span data-ttu-id="5e137-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5e137-141">Key of the entity.</span></span> <span data-ttu-id="5e137-142">Herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="5e137-142">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="5e137-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e137-143">lastModifiedDateTime</span></span>|<span data-ttu-id="5e137-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e137-144">DateTimeOffset</span></span>|<span data-ttu-id="5e137-145">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5e137-145">The date and time the entity was last modified.</span></span> <span data-ttu-id="5e137-146">Herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="5e137-146">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5e137-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e137-147">Response</span></span>
<span data-ttu-id="5e137-148">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e137-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e137-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e137-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e137-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e137-150">Request</span></span>
<span data-ttu-id="5e137-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e137-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5e137-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e137-152">Response</span></span>
<span data-ttu-id="5e137-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e137-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





