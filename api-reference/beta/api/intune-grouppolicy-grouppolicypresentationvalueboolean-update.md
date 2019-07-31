---
title: Atualizar groupPolicyPresentationValueBoolean
description: Atualiza as propriedades de um objeto groupPolicyPresentationValueBoolean.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e1395b1d44451ed3c053f199260dd997ab8cedbb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35989231"
---
# <a name="update-grouppolicypresentationvalueboolean"></a><span data-ttu-id="07377-103">Atualizar groupPolicyPresentationValueBoolean</span><span class="sxs-lookup"><span data-stu-id="07377-103">Update groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="07377-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07377-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07377-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07377-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07377-106">Atualiza as propriedades de um objeto [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) .</span><span class="sxs-lookup"><span data-stu-id="07377-106">Update the properties of a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07377-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07377-107">Prerequisites</span></span>
<span data-ttu-id="07377-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07377-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07377-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07377-110">Permission type</span></span>|<span data-ttu-id="07377-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07377-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07377-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07377-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07377-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07377-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="07377-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07377-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07377-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07377-115">Not supported.</span></span>|
|<span data-ttu-id="07377-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07377-116">Application</span></span>|<span data-ttu-id="07377-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07377-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07377-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07377-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="07377-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07377-119">Request headers</span></span>
|<span data-ttu-id="07377-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07377-120">Header</span></span>|<span data-ttu-id="07377-121">Valor</span><span class="sxs-lookup"><span data-stu-id="07377-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07377-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="07377-122">Authorization</span></span>|<span data-ttu-id="07377-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07377-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07377-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07377-124">Accept</span></span>|<span data-ttu-id="07377-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07377-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07377-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07377-126">Request body</span></span>
<span data-ttu-id="07377-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) .</span><span class="sxs-lookup"><span data-stu-id="07377-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

<span data-ttu-id="07377-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span><span class="sxs-lookup"><span data-stu-id="07377-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span></span>

|<span data-ttu-id="07377-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07377-129">Property</span></span>|<span data-ttu-id="07377-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="07377-130">Type</span></span>|<span data-ttu-id="07377-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="07377-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07377-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07377-132">lastModifiedDateTime</span></span>|<span data-ttu-id="07377-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07377-133">DateTimeOffset</span></span>|<span data-ttu-id="07377-134">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="07377-134">The date and time the object was last modified.</span></span> <span data-ttu-id="07377-135">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="07377-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="07377-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07377-136">createdDateTime</span></span>|<span data-ttu-id="07377-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07377-137">DateTimeOffset</span></span>|<span data-ttu-id="07377-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="07377-138">The date and time the object was created.</span></span> <span data-ttu-id="07377-139">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="07377-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="07377-140">id</span><span class="sxs-lookup"><span data-stu-id="07377-140">id</span></span>|<span data-ttu-id="07377-141">String</span><span class="sxs-lookup"><span data-stu-id="07377-141">String</span></span>|<span data-ttu-id="07377-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="07377-142">Key of the entity.</span></span> <span data-ttu-id="07377-143">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="07377-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="07377-144">value</span><span class="sxs-lookup"><span data-stu-id="07377-144">value</span></span>|<span data-ttu-id="07377-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="07377-145">Boolean</span></span>|<span data-ttu-id="07377-146">Um valor booliano para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="07377-146">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="07377-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="07377-147">Response</span></span>
<span data-ttu-id="07377-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07377-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07377-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07377-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="07377-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07377-150">Request</span></span>
<span data-ttu-id="07377-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07377-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="07377-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="07377-152">Response</span></span>
<span data-ttu-id="07377-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07377-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





