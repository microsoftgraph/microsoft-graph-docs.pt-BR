---
title: Criar groupPolicyPresentationValueBoolean
description: Criar um novo objeto groupPolicyPresentationValueBoolean.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e191fb84e3c3b2e9bb9d0b15a0e12a455d3f3b9d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34965869"
---
# <a name="create-grouppolicypresentationvalueboolean"></a><span data-ttu-id="b19cb-103">Criar groupPolicyPresentationValueBoolean</span><span class="sxs-lookup"><span data-stu-id="b19cb-103">Create groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="b19cb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b19cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b19cb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b19cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b19cb-106">Criar um novo objeto [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) .</span><span class="sxs-lookup"><span data-stu-id="b19cb-106">Create a new [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b19cb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b19cb-107">Prerequisites</span></span>
<span data-ttu-id="b19cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b19cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b19cb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b19cb-110">Permission type</span></span>|<span data-ttu-id="b19cb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b19cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b19cb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b19cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b19cb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b19cb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b19cb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b19cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b19cb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b19cb-115">Not supported.</span></span>|
|<span data-ttu-id="b19cb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b19cb-116">Application</span></span>|<span data-ttu-id="b19cb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b19cb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b19cb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b19cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="b19cb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b19cb-119">Request headers</span></span>
|<span data-ttu-id="b19cb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b19cb-120">Header</span></span>|<span data-ttu-id="b19cb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b19cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b19cb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b19cb-122">Authorization</span></span>|<span data-ttu-id="b19cb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b19cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b19cb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b19cb-124">Accept</span></span>|<span data-ttu-id="b19cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b19cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b19cb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b19cb-126">Request body</span></span>
<span data-ttu-id="b19cb-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationValueBoolean.</span><span class="sxs-lookup"><span data-stu-id="b19cb-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueBoolean object.</span></span>

<span data-ttu-id="b19cb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationValueBoolean.</span><span class="sxs-lookup"><span data-stu-id="b19cb-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueBoolean.</span></span>

|<span data-ttu-id="b19cb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b19cb-129">Property</span></span>|<span data-ttu-id="b19cb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b19cb-130">Type</span></span>|<span data-ttu-id="b19cb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b19cb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b19cb-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b19cb-132">lastModifiedDateTime</span></span>|<span data-ttu-id="b19cb-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b19cb-133">DateTimeOffset</span></span>|<span data-ttu-id="b19cb-134">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b19cb-134">The date and time the object was last modified.</span></span> <span data-ttu-id="b19cb-135">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b19cb-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b19cb-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b19cb-136">createdDateTime</span></span>|<span data-ttu-id="b19cb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b19cb-137">DateTimeOffset</span></span>|<span data-ttu-id="b19cb-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b19cb-138">The date and time the object was created.</span></span> <span data-ttu-id="b19cb-139">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b19cb-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b19cb-140">id</span><span class="sxs-lookup"><span data-stu-id="b19cb-140">id</span></span>|<span data-ttu-id="b19cb-141">String</span><span class="sxs-lookup"><span data-stu-id="b19cb-141">String</span></span>|<span data-ttu-id="b19cb-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b19cb-142">Key of the entity.</span></span> <span data-ttu-id="b19cb-143">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b19cb-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b19cb-144">value</span><span class="sxs-lookup"><span data-stu-id="b19cb-144">value</span></span>|<span data-ttu-id="b19cb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b19cb-145">Boolean</span></span>|<span data-ttu-id="b19cb-146">Um valor booliano para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="b19cb-146">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="b19cb-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="b19cb-147">Response</span></span>
<span data-ttu-id="b19cb-148">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b19cb-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b19cb-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b19cb-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="b19cb-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b19cb-150">Request</span></span>
<span data-ttu-id="b19cb-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b19cb-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="b19cb-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="b19cb-152">Response</span></span>
<span data-ttu-id="b19cb-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b19cb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





