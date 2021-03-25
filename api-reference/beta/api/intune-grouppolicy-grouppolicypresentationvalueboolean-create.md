---
title: Criar groupPolicyPresentationValueBoolean
description: Crie um novo objeto groupPolicyPresentationValueBoolean.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 204ab6e117cd6a5b6f1e4084fd3673b403ba4e56
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157325"
---
# <a name="create-grouppolicypresentationvalueboolean"></a><span data-ttu-id="d6878-103">Criar groupPolicyPresentationValueBoolean</span><span class="sxs-lookup"><span data-stu-id="d6878-103">Create groupPolicyPresentationValueBoolean</span></span>

<span data-ttu-id="d6878-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6878-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6878-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6878-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6878-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6878-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6878-107">Crie um novo [objeto groupPolicyPresentationValueBoolean.](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)</span><span class="sxs-lookup"><span data-stu-id="d6878-107">Create a new [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6878-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6878-108">Prerequisites</span></span>
<span data-ttu-id="d6878-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6878-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6878-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6878-111">Permission type</span></span>|<span data-ttu-id="d6878-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6878-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6878-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6878-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6878-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6878-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6878-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6878-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6878-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6878-116">Not supported.</span></span>|
|<span data-ttu-id="d6878-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6878-117">Application</span></span>|<span data-ttu-id="d6878-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6878-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6878-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6878-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="d6878-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6878-120">Request headers</span></span>
|<span data-ttu-id="d6878-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6878-121">Header</span></span>|<span data-ttu-id="d6878-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d6878-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6878-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6878-123">Authorization</span></span>|<span data-ttu-id="d6878-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6878-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6878-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6878-125">Accept</span></span>|<span data-ttu-id="d6878-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6878-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6878-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6878-127">Request body</span></span>
<span data-ttu-id="d6878-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationValueBoolean.</span><span class="sxs-lookup"><span data-stu-id="d6878-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueBoolean object.</span></span>

<span data-ttu-id="d6878-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyPresentationValueBoolean.</span><span class="sxs-lookup"><span data-stu-id="d6878-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueBoolean.</span></span>

|<span data-ttu-id="d6878-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6878-130">Property</span></span>|<span data-ttu-id="d6878-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6878-131">Type</span></span>|<span data-ttu-id="d6878-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6878-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6878-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6878-133">lastModifiedDateTime</span></span>|<span data-ttu-id="d6878-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6878-134">DateTimeOffset</span></span>|<span data-ttu-id="d6878-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d6878-135">The date and time the object was last modified.</span></span> <span data-ttu-id="d6878-136">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d6878-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="d6878-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6878-137">createdDateTime</span></span>|<span data-ttu-id="d6878-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6878-138">DateTimeOffset</span></span>|<span data-ttu-id="d6878-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d6878-139">The date and time the object was created.</span></span> <span data-ttu-id="d6878-140">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d6878-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="d6878-141">id</span><span class="sxs-lookup"><span data-stu-id="d6878-141">id</span></span>|<span data-ttu-id="d6878-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6878-142">String</span></span>|<span data-ttu-id="d6878-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d6878-143">Key of the entity.</span></span> <span data-ttu-id="d6878-144">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d6878-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="d6878-145">value</span><span class="sxs-lookup"><span data-stu-id="d6878-145">value</span></span>|<span data-ttu-id="d6878-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6878-146">Boolean</span></span>|<span data-ttu-id="d6878-147">Um valor booleano para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="d6878-147">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="d6878-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6878-148">Response</span></span>
<span data-ttu-id="d6878-149">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6878-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6878-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6878-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6878-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6878-151">Request</span></span>
<span data-ttu-id="d6878-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6878-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="d6878-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6878-153">Response</span></span>
<span data-ttu-id="d6878-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6878-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 267

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "be61344f-344f-be61-4f34-61be4f3461be",
  "value": true
}
```




