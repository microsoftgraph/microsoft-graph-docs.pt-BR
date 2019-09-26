---
title: Criar groupPolicyPresentationValueText
description: Criar um novo objeto groupPolicyPresentationValueText.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 80faa33c50c97b6d6e7d34adace6dc9fd6a33a02
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37193505"
---
# <a name="create-grouppolicypresentationvaluetext"></a><span data-ttu-id="89c36-103">Criar groupPolicyPresentationValueText</span><span class="sxs-lookup"><span data-stu-id="89c36-103">Create groupPolicyPresentationValueText</span></span>

> <span data-ttu-id="89c36-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89c36-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89c36-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89c36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89c36-106">Criar um novo objeto [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="89c36-106">Create a new [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89c36-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89c36-107">Prerequisites</span></span>
<span data-ttu-id="89c36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89c36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89c36-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89c36-110">Permission type</span></span>|<span data-ttu-id="89c36-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89c36-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89c36-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89c36-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89c36-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89c36-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="89c36-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89c36-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89c36-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89c36-115">Not supported.</span></span>|
|<span data-ttu-id="89c36-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89c36-116">Application</span></span>|<span data-ttu-id="89c36-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89c36-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89c36-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89c36-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="89c36-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89c36-119">Request headers</span></span>
|<span data-ttu-id="89c36-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89c36-120">Header</span></span>|<span data-ttu-id="89c36-121">Valor</span><span class="sxs-lookup"><span data-stu-id="89c36-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89c36-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="89c36-122">Authorization</span></span>|<span data-ttu-id="89c36-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89c36-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89c36-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="89c36-124">Accept</span></span>|<span data-ttu-id="89c36-125">application/json</span><span class="sxs-lookup"><span data-stu-id="89c36-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89c36-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89c36-126">Request body</span></span>
<span data-ttu-id="89c36-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationValueText.</span><span class="sxs-lookup"><span data-stu-id="89c36-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueText object.</span></span>

<span data-ttu-id="89c36-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationValueText.</span><span class="sxs-lookup"><span data-stu-id="89c36-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueText.</span></span>

|<span data-ttu-id="89c36-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89c36-129">Property</span></span>|<span data-ttu-id="89c36-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="89c36-130">Type</span></span>|<span data-ttu-id="89c36-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="89c36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89c36-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89c36-132">lastModifiedDateTime</span></span>|<span data-ttu-id="89c36-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89c36-133">DateTimeOffset</span></span>|<span data-ttu-id="89c36-134">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="89c36-134">The date and time the object was last modified.</span></span> <span data-ttu-id="89c36-135">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="89c36-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="89c36-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89c36-136">createdDateTime</span></span>|<span data-ttu-id="89c36-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89c36-137">DateTimeOffset</span></span>|<span data-ttu-id="89c36-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="89c36-138">The date and time the object was created.</span></span> <span data-ttu-id="89c36-139">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="89c36-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="89c36-140">id</span><span class="sxs-lookup"><span data-stu-id="89c36-140">id</span></span>|<span data-ttu-id="89c36-141">String</span><span class="sxs-lookup"><span data-stu-id="89c36-141">String</span></span>|<span data-ttu-id="89c36-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="89c36-142">Key of the entity.</span></span> <span data-ttu-id="89c36-143">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="89c36-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="89c36-144">value</span><span class="sxs-lookup"><span data-stu-id="89c36-144">value</span></span>|<span data-ttu-id="89c36-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89c36-145">String</span></span>|<span data-ttu-id="89c36-146">Um valor String para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="89c36-146">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="89c36-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="89c36-147">Response</span></span>
<span data-ttu-id="89c36-148">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89c36-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89c36-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89c36-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="89c36-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89c36-150">Request</span></span>
<span data-ttu-id="89c36-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89c36-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="89c36-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="89c36-152">Response</span></span>
<span data-ttu-id="89c36-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89c36-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 273

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "a3883444-3444-a388-4434-88a3443488a3",
  "value": "Value value"
}
```




