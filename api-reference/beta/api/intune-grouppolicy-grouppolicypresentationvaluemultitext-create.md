---
title: Criar groupPolicyPresentationValueMultiText
description: Criar um novo objeto groupPolicyPresentationValueMultiText.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc58ccd51909f70a0ebd9d9b92adbe72782aa2cd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464026"
---
# <a name="create-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="fbf4c-103">Criar groupPolicyPresentationValueMultiText</span><span class="sxs-lookup"><span data-stu-id="fbf4c-103">Create groupPolicyPresentationValueMultiText</span></span>

<span data-ttu-id="fbf4c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fbf4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbf4c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fbf4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbf4c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbf4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbf4c-107">Criar um novo objeto [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .</span><span class="sxs-lookup"><span data-stu-id="fbf4c-107">Create a new [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbf4c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbf4c-108">Prerequisites</span></span>
<span data-ttu-id="fbf4c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbf4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbf4c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbf4c-111">Permission type</span></span>|<span data-ttu-id="fbf4c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbf4c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbf4c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbf4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbf4c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbf4c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fbf4c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbf4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbf4c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbf4c-116">Not supported.</span></span>|
|<span data-ttu-id="fbf4c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbf4c-117">Application</span></span>|<span data-ttu-id="fbf4c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbf4c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbf4c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbf4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="fbf4c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbf4c-120">Request headers</span></span>
|<span data-ttu-id="fbf4c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbf4c-121">Header</span></span>|<span data-ttu-id="fbf4c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fbf4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbf4c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbf4c-123">Authorization</span></span>|<span data-ttu-id="fbf4c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbf4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbf4c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fbf4c-125">Accept</span></span>|<span data-ttu-id="fbf4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbf4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbf4c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbf4c-127">Request body</span></span>
<span data-ttu-id="fbf4c-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationValueMultiText.</span><span class="sxs-lookup"><span data-stu-id="fbf4c-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueMultiText object.</span></span>

<span data-ttu-id="fbf4c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationValueMultiText.</span><span class="sxs-lookup"><span data-stu-id="fbf4c-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueMultiText.</span></span>

|<span data-ttu-id="fbf4c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbf4c-130">Property</span></span>|<span data-ttu-id="fbf4c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbf4c-131">Type</span></span>|<span data-ttu-id="fbf4c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbf4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbf4c-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbf4c-133">lastModifiedDateTime</span></span>|<span data-ttu-id="fbf4c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbf4c-134">DateTimeOffset</span></span>|<span data-ttu-id="fbf4c-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fbf4c-135">The date and time the object was last modified.</span></span> <span data-ttu-id="fbf4c-136">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fbf4c-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="fbf4c-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbf4c-137">createdDateTime</span></span>|<span data-ttu-id="fbf4c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbf4c-138">DateTimeOffset</span></span>|<span data-ttu-id="fbf4c-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="fbf4c-139">The date and time the object was created.</span></span> <span data-ttu-id="fbf4c-140">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fbf4c-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="fbf4c-141">id</span><span class="sxs-lookup"><span data-stu-id="fbf4c-141">id</span></span>|<span data-ttu-id="fbf4c-142">String</span><span class="sxs-lookup"><span data-stu-id="fbf4c-142">String</span></span>|<span data-ttu-id="fbf4c-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fbf4c-143">Key of the entity.</span></span> <span data-ttu-id="fbf4c-144">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fbf4c-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="fbf4c-145">values</span><span class="sxs-lookup"><span data-stu-id="fbf4c-145">values</span></span>|<span data-ttu-id="fbf4c-146">String collection</span><span class="sxs-lookup"><span data-stu-id="fbf4c-146">String collection</span></span>|<span data-ttu-id="fbf4c-147">Uma coleção de cadeias de caracteres não vazias para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="fbf4c-147">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="fbf4c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbf4c-148">Response</span></span>
<span data-ttu-id="fbf4c-149">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbf4c-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbf4c-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbf4c-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbf4c-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbf4c-151">Request</span></span>
<span data-ttu-id="fbf4c-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbf4c-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "values": [
    "Values value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="fbf4c-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbf4c-153">Response</span></span>
<span data-ttu-id="fbf4c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbf4c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 292

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "5156903b-903b-5156-3b90-56513b905651",
  "values": [
    "Values value"
  ]
}
```





