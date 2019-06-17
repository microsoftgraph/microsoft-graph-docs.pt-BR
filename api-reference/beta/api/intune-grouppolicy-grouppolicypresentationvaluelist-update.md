---
title: Atualizar groupPolicyPresentationValueList
description: Atualiza as propriedades de um objeto groupPolicyPresentationValueList.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b739c2ac02218e948de3eb95d5a451b24c08395b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985490"
---
# <a name="update-grouppolicypresentationvaluelist"></a><span data-ttu-id="07b5b-103">Atualizar groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="07b5b-103">Update groupPolicyPresentationValueList</span></span>

> <span data-ttu-id="07b5b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07b5b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07b5b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07b5b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07b5b-106">Atualiza as propriedades de um objeto [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="07b5b-106">Update the properties of a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07b5b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07b5b-107">Prerequisites</span></span>
<span data-ttu-id="07b5b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07b5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07b5b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07b5b-110">Permission type</span></span>|<span data-ttu-id="07b5b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07b5b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07b5b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07b5b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07b5b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07b5b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="07b5b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07b5b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07b5b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07b5b-115">Not supported.</span></span>|
|<span data-ttu-id="07b5b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07b5b-116">Application</span></span>|<span data-ttu-id="07b5b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07b5b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07b5b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07b5b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="07b5b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07b5b-119">Request headers</span></span>
|<span data-ttu-id="07b5b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07b5b-120">Header</span></span>|<span data-ttu-id="07b5b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="07b5b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07b5b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="07b5b-122">Authorization</span></span>|<span data-ttu-id="07b5b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07b5b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07b5b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07b5b-124">Accept</span></span>|<span data-ttu-id="07b5b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07b5b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07b5b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07b5b-126">Request body</span></span>
<span data-ttu-id="07b5b-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="07b5b-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

<span data-ttu-id="07b5b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span><span class="sxs-lookup"><span data-stu-id="07b5b-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>

|<span data-ttu-id="07b5b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07b5b-129">Property</span></span>|<span data-ttu-id="07b5b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="07b5b-130">Type</span></span>|<span data-ttu-id="07b5b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="07b5b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07b5b-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07b5b-132">lastModifiedDateTime</span></span>|<span data-ttu-id="07b5b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07b5b-133">DateTimeOffset</span></span>|<span data-ttu-id="07b5b-134">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="07b5b-134">The date and time the object was last modified.</span></span> <span data-ttu-id="07b5b-135">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="07b5b-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="07b5b-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07b5b-136">createdDateTime</span></span>|<span data-ttu-id="07b5b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07b5b-137">DateTimeOffset</span></span>|<span data-ttu-id="07b5b-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="07b5b-138">The date and time the object was created.</span></span> <span data-ttu-id="07b5b-139">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="07b5b-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="07b5b-140">id</span><span class="sxs-lookup"><span data-stu-id="07b5b-140">id</span></span>|<span data-ttu-id="07b5b-141">String</span><span class="sxs-lookup"><span data-stu-id="07b5b-141">String</span></span>|<span data-ttu-id="07b5b-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="07b5b-142">Key of the entity.</span></span> <span data-ttu-id="07b5b-143">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="07b5b-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="07b5b-144">values</span><span class="sxs-lookup"><span data-stu-id="07b5b-144">values</span></span>|<span data-ttu-id="07b5b-145">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="07b5b-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="07b5b-146">Uma lista de pares para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="07b5b-146">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="07b5b-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="07b5b-147">Response</span></span>
<span data-ttu-id="07b5b-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07b5b-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07b5b-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07b5b-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="07b5b-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07b5b-150">Request</span></span>
<span data-ttu-id="07b5b-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07b5b-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="07b5b-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="07b5b-152">Response</span></span>
<span data-ttu-id="07b5b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07b5b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "1dbb7865-7865-1dbb-6578-bb1d6578bb1d",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```





