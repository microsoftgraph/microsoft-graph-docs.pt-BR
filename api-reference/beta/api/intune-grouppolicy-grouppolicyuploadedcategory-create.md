---
title: Criar groupPolicyUploadedCategory
description: Criar um novo objeto groupPolicyUploadedCategory.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 534086805e82808a5e9c908fd6313b9659e07733
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444695"
---
# <a name="create-grouppolicyuploadedcategory"></a><span data-ttu-id="6d404-103">Criar groupPolicyUploadedCategory</span><span class="sxs-lookup"><span data-stu-id="6d404-103">Create groupPolicyUploadedCategory</span></span>

<span data-ttu-id="6d404-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d404-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d404-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d404-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d404-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d404-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d404-107">Criar um novo objeto [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="6d404-107">Create a new [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d404-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d404-108">Prerequisites</span></span>
<span data-ttu-id="6d404-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d404-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d404-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d404-111">Permission type</span></span>|<span data-ttu-id="6d404-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d404-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d404-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d404-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d404-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d404-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d404-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d404-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d404-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d404-116">Not supported.</span></span>|
|<span data-ttu-id="6d404-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d404-117">Application</span></span>|<span data-ttu-id="6d404-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d404-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d404-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d404-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyCategories
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/children
```

## <a name="request-headers"></a><span data-ttu-id="6d404-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d404-120">Request headers</span></span>
|<span data-ttu-id="6d404-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d404-121">Header</span></span>|<span data-ttu-id="6d404-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6d404-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d404-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d404-123">Authorization</span></span>|<span data-ttu-id="6d404-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d404-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d404-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d404-125">Accept</span></span>|<span data-ttu-id="6d404-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d404-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d404-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d404-127">Request body</span></span>
<span data-ttu-id="6d404-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyUploadedCategory.</span><span class="sxs-lookup"><span data-stu-id="6d404-128">In the request body, supply a JSON representation for the groupPolicyUploadedCategory object.</span></span>

<span data-ttu-id="6d404-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyUploadedCategory.</span><span class="sxs-lookup"><span data-stu-id="6d404-129">The following table shows the properties that are required when you create the groupPolicyUploadedCategory.</span></span>

|<span data-ttu-id="6d404-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d404-130">Property</span></span>|<span data-ttu-id="6d404-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d404-131">Type</span></span>|<span data-ttu-id="6d404-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d404-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d404-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6d404-133">displayName</span></span>|<span data-ttu-id="6d404-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d404-134">String</span></span>|<span data-ttu-id="6d404-135">A ID da cadeia de caracteres do nome de exibição da categoria herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="6d404-135">The string id of the category's display name Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="6d404-136">IsRoot</span><span class="sxs-lookup"><span data-stu-id="6d404-136">isRoot</span></span>|<span data-ttu-id="6d404-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d404-137">Boolean</span></span>|<span data-ttu-id="6d404-138">Define se a categoria é uma categoria raiz herdada de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="6d404-138">Defines if the category is a root category Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="6d404-139">id</span><span class="sxs-lookup"><span data-stu-id="6d404-139">id</span></span>|<span data-ttu-id="6d404-140">String</span><span class="sxs-lookup"><span data-stu-id="6d404-140">String</span></span>|<span data-ttu-id="6d404-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6d404-141">Key of the entity.</span></span> <span data-ttu-id="6d404-142">Herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="6d404-142">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="6d404-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d404-143">lastModifiedDateTime</span></span>|<span data-ttu-id="6d404-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d404-144">DateTimeOffset</span></span>|<span data-ttu-id="6d404-145">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6d404-145">The date and time the entity was last modified.</span></span> <span data-ttu-id="6d404-146">Herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="6d404-146">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6d404-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d404-147">Response</span></span>
<span data-ttu-id="6d404-148">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d404-148">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d404-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d404-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d404-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d404-150">Request</span></span>
<span data-ttu-id="6d404-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d404-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6d404-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d404-152">Response</span></span>
<span data-ttu-id="6d404-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d404-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



