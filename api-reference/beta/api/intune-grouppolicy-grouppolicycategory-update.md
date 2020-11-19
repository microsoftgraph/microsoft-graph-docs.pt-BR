---
title: Atualizar groupPolicyCategory
description: Atualiza as propriedades de um objeto groupPolicyCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9e766f9742a04197ea5750ee727040754c034f3e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49309113"
---
# <a name="update-grouppolicycategory"></a><span data-ttu-id="3cd70-103">Atualizar groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="3cd70-103">Update groupPolicyCategory</span></span>

<span data-ttu-id="3cd70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cd70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3cd70-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3cd70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cd70-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3cd70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cd70-107">Atualiza as propriedades de um objeto [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="3cd70-107">Update the properties of a [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3cd70-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3cd70-108">Prerequisites</span></span>
<span data-ttu-id="3cd70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cd70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cd70-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cd70-111">Permission type</span></span>|<span data-ttu-id="3cd70-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3cd70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cd70-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cd70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3cd70-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cd70-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3cd70-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cd70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cd70-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cd70-116">Not supported.</span></span>|
|<span data-ttu-id="3cd70-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cd70-117">Application</span></span>|<span data-ttu-id="3cd70-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cd70-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cd70-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cd70-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="3cd70-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd70-120">Request headers</span></span>
|<span data-ttu-id="3cd70-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3cd70-121">Header</span></span>|<span data-ttu-id="3cd70-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3cd70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cd70-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cd70-123">Authorization</span></span>|<span data-ttu-id="3cd70-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cd70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cd70-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3cd70-125">Accept</span></span>|<span data-ttu-id="3cd70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3cd70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cd70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd70-127">Request body</span></span>
<span data-ttu-id="3cd70-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="3cd70-128">In the request body, supply a JSON representation for the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>

<span data-ttu-id="3cd70-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md).</span><span class="sxs-lookup"><span data-stu-id="3cd70-129">The following table shows the properties that are required when you create the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md).</span></span>

|<span data-ttu-id="3cd70-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cd70-130">Property</span></span>|<span data-ttu-id="3cd70-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cd70-131">Type</span></span>|<span data-ttu-id="3cd70-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cd70-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cd70-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3cd70-133">displayName</span></span>|<span data-ttu-id="3cd70-134">String</span><span class="sxs-lookup"><span data-stu-id="3cd70-134">String</span></span>|<span data-ttu-id="3cd70-135">A ID da cadeia de caracteres do nome de exibição da categoria</span><span class="sxs-lookup"><span data-stu-id="3cd70-135">The string id of the category's display name</span></span>|
|<span data-ttu-id="3cd70-136">IsRoot</span><span class="sxs-lookup"><span data-stu-id="3cd70-136">isRoot</span></span>|<span data-ttu-id="3cd70-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="3cd70-137">Boolean</span></span>|<span data-ttu-id="3cd70-138">Define se a categoria é uma categoria raiz</span><span class="sxs-lookup"><span data-stu-id="3cd70-138">Defines if the category is a root category</span></span>|
|<span data-ttu-id="3cd70-139">id</span><span class="sxs-lookup"><span data-stu-id="3cd70-139">id</span></span>|<span data-ttu-id="3cd70-140">String</span><span class="sxs-lookup"><span data-stu-id="3cd70-140">String</span></span>|<span data-ttu-id="3cd70-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3cd70-141">Key of the entity.</span></span>|
|<span data-ttu-id="3cd70-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3cd70-142">lastModifiedDateTime</span></span>|<span data-ttu-id="3cd70-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cd70-143">DateTimeOffset</span></span>|<span data-ttu-id="3cd70-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3cd70-144">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="3cd70-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cd70-145">Response</span></span>
<span data-ttu-id="3cd70-146">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cd70-146">If successful, this method returns a `200 OK` response code and an updated [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cd70-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cd70-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cd70-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd70-148">Request</span></span>
<span data-ttu-id="3cd70-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cd70-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "Display Name value",
  "isRoot": true
}
```

### <a name="response"></a><span data-ttu-id="3cd70-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cd70-150">Response</span></span>
<span data-ttu-id="3cd70-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3cd70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "Display Name value",
  "isRoot": true,
  "id": "d0641e36-1e36-d064-361e-64d0361e64d0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




