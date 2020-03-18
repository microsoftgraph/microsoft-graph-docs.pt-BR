---
title: Atualizar groupPolicyCategory
description: Atualiza as propriedades de um objeto groupPolicyCategory.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 72aec785250fe38f8733964fcf140aacc95a09cd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804524"
---
# <a name="update-grouppolicycategory"></a><span data-ttu-id="9563c-103">Atualizar groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="9563c-103">Update groupPolicyCategory</span></span>

> <span data-ttu-id="9563c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9563c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9563c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9563c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9563c-106">Atualiza as propriedades de um objeto [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="9563c-106">Update the properties of a [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9563c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9563c-107">Prerequisites</span></span>
<span data-ttu-id="9563c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9563c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9563c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9563c-110">Permission type</span></span>|<span data-ttu-id="9563c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9563c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9563c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9563c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9563c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9563c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9563c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9563c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9563c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9563c-115">Not supported.</span></span>|
|<span data-ttu-id="9563c-116">Application</span><span class="sxs-lookup"><span data-stu-id="9563c-116">Application</span></span>|<span data-ttu-id="9563c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9563c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9563c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9563c-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9563c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9563c-119">Request headers</span></span>
|<span data-ttu-id="9563c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9563c-120">Header</span></span>|<span data-ttu-id="9563c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9563c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9563c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9563c-122">Authorization</span></span>|<span data-ttu-id="9563c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9563c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9563c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9563c-124">Accept</span></span>|<span data-ttu-id="9563c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9563c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9563c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9563c-126">Request body</span></span>
<span data-ttu-id="9563c-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="9563c-127">In the request body, supply a JSON representation for the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>

<span data-ttu-id="9563c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md).</span><span class="sxs-lookup"><span data-stu-id="9563c-128">The following table shows the properties that are required when you create the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md).</span></span>

|<span data-ttu-id="9563c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9563c-129">Property</span></span>|<span data-ttu-id="9563c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9563c-130">Type</span></span>|<span data-ttu-id="9563c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9563c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9563c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="9563c-132">displayName</span></span>|<span data-ttu-id="9563c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9563c-133">String</span></span>|<span data-ttu-id="9563c-134">A ID da cadeia de caracteres do nome de exibição da categoria</span><span class="sxs-lookup"><span data-stu-id="9563c-134">The string id of the category's display name</span></span>|
|<span data-ttu-id="9563c-135">IsRoot</span><span class="sxs-lookup"><span data-stu-id="9563c-135">isRoot</span></span>|<span data-ttu-id="9563c-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="9563c-136">Boolean</span></span>|<span data-ttu-id="9563c-137">Define se a categoria é uma categoria raiz</span><span class="sxs-lookup"><span data-stu-id="9563c-137">Defines if the category is a root category</span></span>|
|<span data-ttu-id="9563c-138">id</span><span class="sxs-lookup"><span data-stu-id="9563c-138">id</span></span>|<span data-ttu-id="9563c-139">String</span><span class="sxs-lookup"><span data-stu-id="9563c-139">String</span></span>|<span data-ttu-id="9563c-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9563c-140">Key of the entity.</span></span>|
|<span data-ttu-id="9563c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9563c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="9563c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9563c-142">DateTimeOffset</span></span>|<span data-ttu-id="9563c-143">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9563c-143">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="9563c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9563c-144">Response</span></span>
<span data-ttu-id="9563c-145">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9563c-145">If successful, this method returns a `200 OK` response code and an updated [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9563c-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9563c-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="9563c-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9563c-147">Request</span></span>
<span data-ttu-id="9563c-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9563c-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9563c-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="9563c-149">Response</span></span>
<span data-ttu-id="9563c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9563c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




