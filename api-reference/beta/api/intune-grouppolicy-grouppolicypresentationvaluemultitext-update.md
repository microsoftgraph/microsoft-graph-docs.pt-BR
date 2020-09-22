---
title: Atualizar groupPolicyPresentationValueMultiText
description: Atualiza as propriedades de um objeto groupPolicyPresentationValueMultiText.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df4adc4f56577f04ec9e4e16decd87e00a138e85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020185"
---
# <a name="update-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="4135f-103">Atualizar groupPolicyPresentationValueMultiText</span><span class="sxs-lookup"><span data-stu-id="4135f-103">Update groupPolicyPresentationValueMultiText</span></span>

<span data-ttu-id="4135f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4135f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4135f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4135f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4135f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4135f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4135f-107">Atualiza as propriedades de um objeto [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .</span><span class="sxs-lookup"><span data-stu-id="4135f-107">Update the properties of a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4135f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4135f-108">Prerequisites</span></span>
<span data-ttu-id="4135f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4135f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4135f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4135f-111">Permission type</span></span>|<span data-ttu-id="4135f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4135f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4135f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4135f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4135f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4135f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4135f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4135f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4135f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4135f-116">Not supported.</span></span>|
|<span data-ttu-id="4135f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4135f-117">Application</span></span>|<span data-ttu-id="4135f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4135f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4135f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4135f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="4135f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4135f-120">Request headers</span></span>
|<span data-ttu-id="4135f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4135f-121">Header</span></span>|<span data-ttu-id="4135f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4135f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4135f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4135f-123">Authorization</span></span>|<span data-ttu-id="4135f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4135f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4135f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4135f-125">Accept</span></span>|<span data-ttu-id="4135f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4135f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4135f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4135f-127">Request body</span></span>
<span data-ttu-id="4135f-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .</span><span class="sxs-lookup"><span data-stu-id="4135f-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

<span data-ttu-id="4135f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span><span class="sxs-lookup"><span data-stu-id="4135f-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span></span>

|<span data-ttu-id="4135f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4135f-130">Property</span></span>|<span data-ttu-id="4135f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4135f-131">Type</span></span>|<span data-ttu-id="4135f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4135f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4135f-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4135f-133">lastModifiedDateTime</span></span>|<span data-ttu-id="4135f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4135f-134">DateTimeOffset</span></span>|<span data-ttu-id="4135f-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4135f-135">The date and time the object was last modified.</span></span> <span data-ttu-id="4135f-136">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="4135f-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="4135f-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4135f-137">createdDateTime</span></span>|<span data-ttu-id="4135f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4135f-138">DateTimeOffset</span></span>|<span data-ttu-id="4135f-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4135f-139">The date and time the object was created.</span></span> <span data-ttu-id="4135f-140">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="4135f-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="4135f-141">id</span><span class="sxs-lookup"><span data-stu-id="4135f-141">id</span></span>|<span data-ttu-id="4135f-142">String</span><span class="sxs-lookup"><span data-stu-id="4135f-142">String</span></span>|<span data-ttu-id="4135f-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4135f-143">Key of the entity.</span></span> <span data-ttu-id="4135f-144">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="4135f-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="4135f-145">values</span><span class="sxs-lookup"><span data-stu-id="4135f-145">values</span></span>|<span data-ttu-id="4135f-146">Coleção String</span><span class="sxs-lookup"><span data-stu-id="4135f-146">String collection</span></span>|<span data-ttu-id="4135f-147">Uma coleção de cadeias de caracteres não vazias para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="4135f-147">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="4135f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="4135f-148">Response</span></span>
<span data-ttu-id="4135f-149">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4135f-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4135f-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4135f-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="4135f-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4135f-151">Request</span></span>
<span data-ttu-id="4135f-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4135f-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "values": [
    "Values value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="4135f-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="4135f-153">Response</span></span>
<span data-ttu-id="4135f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4135f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






