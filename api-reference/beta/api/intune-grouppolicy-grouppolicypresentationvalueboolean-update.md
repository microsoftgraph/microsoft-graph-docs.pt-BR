---
title: Atualizar groupPolicyPresentationValueBoolean
description: Atualiza as propriedades de um objeto groupPolicyPresentationValueBoolean.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a05f9f8b2018d0f5d0c8f2986f0cb06620514e81
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49227340"
---
# <a name="update-grouppolicypresentationvalueboolean"></a><span data-ttu-id="c74b4-103">Atualizar groupPolicyPresentationValueBoolean</span><span class="sxs-lookup"><span data-stu-id="c74b4-103">Update groupPolicyPresentationValueBoolean</span></span>

<span data-ttu-id="c74b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c74b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c74b4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c74b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c74b4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c74b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c74b4-107">Atualiza as propriedades de um objeto [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) .</span><span class="sxs-lookup"><span data-stu-id="c74b4-107">Update the properties of a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c74b4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c74b4-108">Prerequisites</span></span>
<span data-ttu-id="c74b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c74b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c74b4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c74b4-111">Permission type</span></span>|<span data-ttu-id="c74b4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c74b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c74b4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c74b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c74b4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c74b4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c74b4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c74b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c74b4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c74b4-116">Not supported.</span></span>|
|<span data-ttu-id="c74b4-117">Application</span><span class="sxs-lookup"><span data-stu-id="c74b4-117">Application</span></span>|<span data-ttu-id="c74b4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c74b4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c74b4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c74b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="c74b4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c74b4-120">Request headers</span></span>
|<span data-ttu-id="c74b4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c74b4-121">Header</span></span>|<span data-ttu-id="c74b4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c74b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c74b4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c74b4-123">Authorization</span></span>|<span data-ttu-id="c74b4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c74b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c74b4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c74b4-125">Accept</span></span>|<span data-ttu-id="c74b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c74b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c74b4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c74b4-127">Request body</span></span>
<span data-ttu-id="c74b4-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) .</span><span class="sxs-lookup"><span data-stu-id="c74b4-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

<span data-ttu-id="c74b4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span><span class="sxs-lookup"><span data-stu-id="c74b4-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span></span>

|<span data-ttu-id="c74b4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c74b4-130">Property</span></span>|<span data-ttu-id="c74b4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c74b4-131">Type</span></span>|<span data-ttu-id="c74b4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c74b4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c74b4-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c74b4-133">lastModifiedDateTime</span></span>|<span data-ttu-id="c74b4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c74b4-134">DateTimeOffset</span></span>|<span data-ttu-id="c74b4-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c74b4-135">The date and time the object was last modified.</span></span> <span data-ttu-id="c74b4-136">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c74b4-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="c74b4-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c74b4-137">createdDateTime</span></span>|<span data-ttu-id="c74b4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c74b4-138">DateTimeOffset</span></span>|<span data-ttu-id="c74b4-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c74b4-139">The date and time the object was created.</span></span> <span data-ttu-id="c74b4-140">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c74b4-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="c74b4-141">id</span><span class="sxs-lookup"><span data-stu-id="c74b4-141">id</span></span>|<span data-ttu-id="c74b4-142">String</span><span class="sxs-lookup"><span data-stu-id="c74b4-142">String</span></span>|<span data-ttu-id="c74b4-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c74b4-143">Key of the entity.</span></span> <span data-ttu-id="c74b4-144">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c74b4-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="c74b4-145">value</span><span class="sxs-lookup"><span data-stu-id="c74b4-145">value</span></span>|<span data-ttu-id="c74b4-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c74b4-146">Boolean</span></span>|<span data-ttu-id="c74b4-147">Um valor booliano para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="c74b4-147">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="c74b4-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c74b4-148">Response</span></span>
<span data-ttu-id="c74b4-149">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c74b4-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c74b4-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c74b4-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="c74b4-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c74b4-151">Request</span></span>
<span data-ttu-id="c74b4-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c74b4-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="c74b4-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c74b4-153">Response</span></span>
<span data-ttu-id="c74b4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c74b4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




