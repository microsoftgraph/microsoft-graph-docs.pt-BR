---
title: Criar groupPolicyPresentationValueText
description: Criar um novo objeto groupPolicyPresentationValueText.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 52768d32767829ee6a9a1d1c672738881f09654c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463163"
---
# <a name="create-grouppolicypresentationvaluetext"></a><span data-ttu-id="58531-103">Criar groupPolicyPresentationValueText</span><span class="sxs-lookup"><span data-stu-id="58531-103">Create groupPolicyPresentationValueText</span></span>

<span data-ttu-id="58531-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58531-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58531-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58531-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58531-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58531-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58531-107">Criar um novo objeto [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="58531-107">Create a new [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58531-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58531-108">Prerequisites</span></span>
<span data-ttu-id="58531-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58531-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58531-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58531-111">Permission type</span></span>|<span data-ttu-id="58531-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58531-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58531-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58531-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58531-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58531-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58531-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58531-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58531-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58531-116">Not supported.</span></span>|
|<span data-ttu-id="58531-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58531-117">Application</span></span>|<span data-ttu-id="58531-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58531-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58531-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58531-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="58531-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58531-120">Request headers</span></span>
|<span data-ttu-id="58531-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58531-121">Header</span></span>|<span data-ttu-id="58531-122">Valor</span><span class="sxs-lookup"><span data-stu-id="58531-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58531-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="58531-123">Authorization</span></span>|<span data-ttu-id="58531-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58531-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58531-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58531-125">Accept</span></span>|<span data-ttu-id="58531-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58531-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58531-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58531-127">Request body</span></span>
<span data-ttu-id="58531-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationValueText.</span><span class="sxs-lookup"><span data-stu-id="58531-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueText object.</span></span>

<span data-ttu-id="58531-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationValueText.</span><span class="sxs-lookup"><span data-stu-id="58531-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueText.</span></span>

|<span data-ttu-id="58531-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58531-130">Property</span></span>|<span data-ttu-id="58531-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="58531-131">Type</span></span>|<span data-ttu-id="58531-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="58531-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58531-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58531-133">lastModifiedDateTime</span></span>|<span data-ttu-id="58531-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58531-134">DateTimeOffset</span></span>|<span data-ttu-id="58531-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="58531-135">The date and time the object was last modified.</span></span> <span data-ttu-id="58531-136">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="58531-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="58531-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58531-137">createdDateTime</span></span>|<span data-ttu-id="58531-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58531-138">DateTimeOffset</span></span>|<span data-ttu-id="58531-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="58531-139">The date and time the object was created.</span></span> <span data-ttu-id="58531-140">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="58531-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="58531-141">id</span><span class="sxs-lookup"><span data-stu-id="58531-141">id</span></span>|<span data-ttu-id="58531-142">String</span><span class="sxs-lookup"><span data-stu-id="58531-142">String</span></span>|<span data-ttu-id="58531-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="58531-143">Key of the entity.</span></span> <span data-ttu-id="58531-144">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="58531-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="58531-145">value</span><span class="sxs-lookup"><span data-stu-id="58531-145">value</span></span>|<span data-ttu-id="58531-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58531-146">String</span></span>|<span data-ttu-id="58531-147">Um valor String para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="58531-147">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="58531-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="58531-148">Response</span></span>
<span data-ttu-id="58531-149">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58531-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58531-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58531-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="58531-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58531-151">Request</span></span>
<span data-ttu-id="58531-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58531-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="58531-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="58531-153">Response</span></span>
<span data-ttu-id="58531-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58531-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



