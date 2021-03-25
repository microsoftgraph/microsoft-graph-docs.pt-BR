---
title: Atualizar groupPolicyUploadedCategory
description: Atualize as propriedades de um objeto groupPolicyUploadedCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 907df2881555cf651442bffd29c2cd98b0e25d0e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157014"
---
# <a name="update-grouppolicyuploadedcategory"></a><span data-ttu-id="f6f79-103">Atualizar groupPolicyUploadedCategory</span><span class="sxs-lookup"><span data-stu-id="f6f79-103">Update groupPolicyUploadedCategory</span></span>

<span data-ttu-id="f6f79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6f79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6f79-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6f79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6f79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6f79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6f79-107">Atualize as propriedades de [um objeto groupPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)</span><span class="sxs-lookup"><span data-stu-id="f6f79-107">Update the properties of a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6f79-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f6f79-108">Prerequisites</span></span>
<span data-ttu-id="f6f79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6f79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6f79-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6f79-111">Permission type</span></span>|<span data-ttu-id="f6f79-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6f79-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6f79-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6f79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6f79-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6f79-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6f79-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6f79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6f79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6f79-116">Not supported.</span></span>|
|<span data-ttu-id="f6f79-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6f79-117">Application</span></span>|<span data-ttu-id="f6f79-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6f79-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6f79-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6f79-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f6f79-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6f79-120">Request headers</span></span>
|<span data-ttu-id="f6f79-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6f79-121">Header</span></span>|<span data-ttu-id="f6f79-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f6f79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6f79-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6f79-123">Authorization</span></span>|<span data-ttu-id="f6f79-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6f79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6f79-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f6f79-125">Accept</span></span>|<span data-ttu-id="f6f79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6f79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6f79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6f79-127">Request body</span></span>
<span data-ttu-id="f6f79-128">No corpo da solicitação, fornece uma representação JSON para [o objeto groupPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)</span><span class="sxs-lookup"><span data-stu-id="f6f79-128">In the request body, supply a JSON representation for the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

<span data-ttu-id="f6f79-129">A tabela a seguir mostra as propriedades necessárias ao criar [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span><span class="sxs-lookup"><span data-stu-id="f6f79-129">The following table shows the properties that are required when you create the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span></span>

|<span data-ttu-id="f6f79-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6f79-130">Property</span></span>|<span data-ttu-id="f6f79-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6f79-131">Type</span></span>|<span data-ttu-id="f6f79-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6f79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6f79-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f6f79-133">displayName</span></span>|<span data-ttu-id="f6f79-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6f79-134">String</span></span>|<span data-ttu-id="f6f79-135">A id de cadeia de caracteres do nome de exibição da categoria Herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="f6f79-135">The string id of the category's display name Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="f6f79-136">isRoot</span><span class="sxs-lookup"><span data-stu-id="f6f79-136">isRoot</span></span>|<span data-ttu-id="f6f79-137">Booleano</span><span class="sxs-lookup"><span data-stu-id="f6f79-137">Boolean</span></span>|<span data-ttu-id="f6f79-138">Define se a categoria é uma categoria raiz Herdada de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="f6f79-138">Defines if the category is a root category Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="f6f79-139">id</span><span class="sxs-lookup"><span data-stu-id="f6f79-139">id</span></span>|<span data-ttu-id="f6f79-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6f79-140">String</span></span>|<span data-ttu-id="f6f79-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f6f79-141">Key of the entity.</span></span> <span data-ttu-id="f6f79-142">Herdado [de groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="f6f79-142">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="f6f79-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6f79-143">lastModifiedDateTime</span></span>|<span data-ttu-id="f6f79-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6f79-144">DateTimeOffset</span></span>|<span data-ttu-id="f6f79-145">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f6f79-145">The date and time the entity was last modified.</span></span> <span data-ttu-id="f6f79-146">Herdado [de groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="f6f79-146">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f6f79-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6f79-147">Response</span></span>
<span data-ttu-id="f6f79-148">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6f79-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6f79-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6f79-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6f79-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6f79-150">Request</span></span>
<span data-ttu-id="f6f79-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6f79-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f6f79-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6f79-152">Response</span></span>
<span data-ttu-id="f6f79-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6f79-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




