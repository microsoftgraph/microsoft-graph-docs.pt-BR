---
title: Criar groupPolicyUploadedCategory
description: Criar um novo objeto groupPolicyUploadedCategory.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6c85e0db90d7015182d90aac060048cea4042242
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803796"
---
# <a name="create-grouppolicyuploadedcategory"></a><span data-ttu-id="522ff-103">Criar groupPolicyUploadedCategory</span><span class="sxs-lookup"><span data-stu-id="522ff-103">Create groupPolicyUploadedCategory</span></span>

> <span data-ttu-id="522ff-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="522ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="522ff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="522ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="522ff-106">Criar um novo objeto [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="522ff-106">Create a new [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="522ff-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="522ff-107">Prerequisites</span></span>
<span data-ttu-id="522ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="522ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="522ff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="522ff-110">Permission type</span></span>|<span data-ttu-id="522ff-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="522ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="522ff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="522ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="522ff-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="522ff-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="522ff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="522ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="522ff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="522ff-115">Not supported.</span></span>|
|<span data-ttu-id="522ff-116">Application</span><span class="sxs-lookup"><span data-stu-id="522ff-116">Application</span></span>|<span data-ttu-id="522ff-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="522ff-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="522ff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="522ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyCategories
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/children
```

## <a name="request-headers"></a><span data-ttu-id="522ff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="522ff-119">Request headers</span></span>
|<span data-ttu-id="522ff-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="522ff-120">Header</span></span>|<span data-ttu-id="522ff-121">Valor</span><span class="sxs-lookup"><span data-stu-id="522ff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="522ff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="522ff-122">Authorization</span></span>|<span data-ttu-id="522ff-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="522ff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="522ff-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="522ff-124">Accept</span></span>|<span data-ttu-id="522ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="522ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="522ff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="522ff-126">Request body</span></span>
<span data-ttu-id="522ff-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyUploadedCategory.</span><span class="sxs-lookup"><span data-stu-id="522ff-127">In the request body, supply a JSON representation for the groupPolicyUploadedCategory object.</span></span>

<span data-ttu-id="522ff-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyUploadedCategory.</span><span class="sxs-lookup"><span data-stu-id="522ff-128">The following table shows the properties that are required when you create the groupPolicyUploadedCategory.</span></span>

|<span data-ttu-id="522ff-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="522ff-129">Property</span></span>|<span data-ttu-id="522ff-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="522ff-130">Type</span></span>|<span data-ttu-id="522ff-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="522ff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="522ff-132">displayName</span><span class="sxs-lookup"><span data-stu-id="522ff-132">displayName</span></span>|<span data-ttu-id="522ff-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="522ff-133">String</span></span>|<span data-ttu-id="522ff-134">A ID da cadeia de caracteres do nome de exibição da categoria herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="522ff-134">The string id of the category's display name Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="522ff-135">IsRoot</span><span class="sxs-lookup"><span data-stu-id="522ff-135">isRoot</span></span>|<span data-ttu-id="522ff-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="522ff-136">Boolean</span></span>|<span data-ttu-id="522ff-137">Define se a categoria é uma categoria raiz herdada de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="522ff-137">Defines if the category is a root category Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="522ff-138">id</span><span class="sxs-lookup"><span data-stu-id="522ff-138">id</span></span>|<span data-ttu-id="522ff-139">String</span><span class="sxs-lookup"><span data-stu-id="522ff-139">String</span></span>|<span data-ttu-id="522ff-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="522ff-140">Key of the entity.</span></span> <span data-ttu-id="522ff-141">Herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="522ff-141">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="522ff-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="522ff-142">lastModifiedDateTime</span></span>|<span data-ttu-id="522ff-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="522ff-143">DateTimeOffset</span></span>|<span data-ttu-id="522ff-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="522ff-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="522ff-145">Herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="522ff-145">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="522ff-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="522ff-146">Response</span></span>
<span data-ttu-id="522ff-147">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="522ff-147">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="522ff-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="522ff-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="522ff-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="522ff-149">Request</span></span>
<span data-ttu-id="522ff-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="522ff-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
  "displayName": "Display Name value",
  "isRoot": true
}
```

### <a name="response"></a><span data-ttu-id="522ff-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="522ff-151">Response</span></span>
<span data-ttu-id="522ff-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="522ff-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




