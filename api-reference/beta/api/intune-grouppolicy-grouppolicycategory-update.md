---
title: Atualizar groupPolicyCategory
description: Atualize as propriedades de um objeto groupPolicyCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a70edcb1f05ceb19a7dbb7a65d2d4b501a724dc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153479"
---
# <a name="update-grouppolicycategory"></a><span data-ttu-id="96525-103">Atualizar groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="96525-103">Update groupPolicyCategory</span></span>

<span data-ttu-id="96525-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96525-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96525-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="96525-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96525-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96525-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96525-107">Atualize as propriedades de [um objeto groupPolicyCategory.](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="96525-107">Update the properties of a [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96525-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96525-108">Prerequisites</span></span>
<span data-ttu-id="96525-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96525-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96525-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96525-111">Permission type</span></span>|<span data-ttu-id="96525-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96525-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96525-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96525-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96525-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96525-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96525-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96525-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96525-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96525-116">Not supported.</span></span>|
|<span data-ttu-id="96525-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96525-117">Application</span></span>|<span data-ttu-id="96525-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96525-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96525-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96525-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="96525-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96525-120">Request headers</span></span>
|<span data-ttu-id="96525-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96525-121">Header</span></span>|<span data-ttu-id="96525-122">Valor</span><span class="sxs-lookup"><span data-stu-id="96525-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96525-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="96525-123">Authorization</span></span>|<span data-ttu-id="96525-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96525-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96525-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96525-125">Accept</span></span>|<span data-ttu-id="96525-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96525-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96525-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96525-127">Request body</span></span>
<span data-ttu-id="96525-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicyCategory.](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="96525-128">In the request body, supply a JSON representation for the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>

<span data-ttu-id="96525-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md).</span><span class="sxs-lookup"><span data-stu-id="96525-129">The following table shows the properties that are required when you create the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md).</span></span>

|<span data-ttu-id="96525-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96525-130">Property</span></span>|<span data-ttu-id="96525-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="96525-131">Type</span></span>|<span data-ttu-id="96525-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="96525-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96525-133">displayName</span><span class="sxs-lookup"><span data-stu-id="96525-133">displayName</span></span>|<span data-ttu-id="96525-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96525-134">String</span></span>|<span data-ttu-id="96525-135">A id de cadeia de caracteres do nome de exibição da categoria</span><span class="sxs-lookup"><span data-stu-id="96525-135">The string id of the category's display name</span></span>|
|<span data-ttu-id="96525-136">isRoot</span><span class="sxs-lookup"><span data-stu-id="96525-136">isRoot</span></span>|<span data-ttu-id="96525-137">Booleano</span><span class="sxs-lookup"><span data-stu-id="96525-137">Boolean</span></span>|<span data-ttu-id="96525-138">Define se a categoria é uma categoria raiz</span><span class="sxs-lookup"><span data-stu-id="96525-138">Defines if the category is a root category</span></span>|
|<span data-ttu-id="96525-139">id</span><span class="sxs-lookup"><span data-stu-id="96525-139">id</span></span>|<span data-ttu-id="96525-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96525-140">String</span></span>|<span data-ttu-id="96525-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="96525-141">Key of the entity.</span></span>|
|<span data-ttu-id="96525-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96525-142">lastModifiedDateTime</span></span>|<span data-ttu-id="96525-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96525-143">DateTimeOffset</span></span>|<span data-ttu-id="96525-144">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="96525-144">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="96525-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="96525-145">Response</span></span>
<span data-ttu-id="96525-146">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96525-146">If successful, this method returns a `200 OK` response code and an updated [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96525-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96525-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="96525-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96525-148">Request</span></span>
<span data-ttu-id="96525-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96525-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96525-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="96525-150">Response</span></span>
<span data-ttu-id="96525-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96525-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




