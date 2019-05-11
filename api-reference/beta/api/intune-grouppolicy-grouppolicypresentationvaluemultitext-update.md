---
title: Atualizar groupPolicyPresentationValueMultiText
description: Atualiza as propriedades de um objeto groupPolicyPresentationValueMultiText.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7828644fb9960f81e2f2f9ba23d21aa53cc09ff6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33904136"
---
# <a name="update-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="5e3e4-103">Atualizar groupPolicyPresentationValueMultiText</span><span class="sxs-lookup"><span data-stu-id="5e3e4-103">Update groupPolicyPresentationValueMultiText</span></span>

> <span data-ttu-id="5e3e4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5e3e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e3e4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e3e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e3e4-106">Atualiza as propriedades de um objeto [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .</span><span class="sxs-lookup"><span data-stu-id="5e3e4-106">Update the properties of a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e3e4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e3e4-107">Prerequisites</span></span>
<span data-ttu-id="5e3e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e3e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e3e4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e3e4-110">Permission type</span></span>|<span data-ttu-id="5e3e4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5e3e4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e3e4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e3e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e3e4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e3e4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5e3e4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e3e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e3e4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e3e4-115">Not supported.</span></span>|
|<span data-ttu-id="5e3e4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e3e4-116">Application</span></span>|<span data-ttu-id="5e3e4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e3e4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e3e4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e3e4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="5e3e4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e3e4-119">Request headers</span></span>
|<span data-ttu-id="5e3e4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e3e4-120">Header</span></span>|<span data-ttu-id="5e3e4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5e3e4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e3e4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e3e4-122">Authorization</span></span>|<span data-ttu-id="5e3e4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e3e4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e3e4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5e3e4-124">Accept</span></span>|<span data-ttu-id="5e3e4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5e3e4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e3e4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e3e4-126">Request body</span></span>
<span data-ttu-id="5e3e4-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .</span><span class="sxs-lookup"><span data-stu-id="5e3e4-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

<span data-ttu-id="5e3e4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span><span class="sxs-lookup"><span data-stu-id="5e3e4-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span></span>

|<span data-ttu-id="5e3e4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e3e4-129">Property</span></span>|<span data-ttu-id="5e3e4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e3e4-130">Type</span></span>|<span data-ttu-id="5e3e4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e3e4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e3e4-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e3e4-132">lastModifiedDateTime</span></span>|<span data-ttu-id="5e3e4-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e3e4-133">DateTimeOffset</span></span>|<span data-ttu-id="5e3e4-134">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5e3e4-134">The date and time the object was last modified.</span></span> <span data-ttu-id="5e3e4-135">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5e3e4-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="5e3e4-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e3e4-136">createdDateTime</span></span>|<span data-ttu-id="5e3e4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e3e4-137">DateTimeOffset</span></span>|<span data-ttu-id="5e3e4-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5e3e4-138">The date and time the object was created.</span></span> <span data-ttu-id="5e3e4-139">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5e3e4-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="5e3e4-140">id</span><span class="sxs-lookup"><span data-stu-id="5e3e4-140">id</span></span>|<span data-ttu-id="5e3e4-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e3e4-141">String</span></span>|<span data-ttu-id="5e3e4-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5e3e4-142">Key of the entity.</span></span> <span data-ttu-id="5e3e4-143">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5e3e4-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="5e3e4-144">values</span><span class="sxs-lookup"><span data-stu-id="5e3e4-144">values</span></span>|<span data-ttu-id="5e3e4-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e3e4-145">String collection</span></span>|<span data-ttu-id="5e3e4-146">Uma coleção de cadeias de caracteres não vazias para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="5e3e4-146">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="5e3e4-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e3e4-147">Response</span></span>
<span data-ttu-id="5e3e4-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e3e4-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e3e4-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e3e4-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e3e4-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e3e4-150">Request</span></span>
<span data-ttu-id="5e3e4-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e3e4-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5e3e4-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e3e4-152">Response</span></span>
<span data-ttu-id="5e3e4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e3e4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




