---
title: Atualizar groupPolicyPresentationValueList
description: Atualiza as propriedades de um objeto groupPolicyPresentationValueList.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b948849e505cd185ee42195d5e2b7e646bf30e63
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33904311"
---
# <a name="update-grouppolicypresentationvaluelist"></a><span data-ttu-id="18ebb-103">Atualizar groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="18ebb-103">Update groupPolicyPresentationValueList</span></span>

> <span data-ttu-id="18ebb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="18ebb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18ebb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18ebb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18ebb-106">Atualiza as propriedades de um objeto [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="18ebb-106">Update the properties of a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18ebb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="18ebb-107">Prerequisites</span></span>
<span data-ttu-id="18ebb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18ebb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18ebb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18ebb-110">Permission type</span></span>|<span data-ttu-id="18ebb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="18ebb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18ebb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18ebb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18ebb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18ebb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="18ebb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18ebb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18ebb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18ebb-115">Not supported.</span></span>|
|<span data-ttu-id="18ebb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18ebb-116">Application</span></span>|<span data-ttu-id="18ebb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18ebb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18ebb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18ebb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="18ebb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18ebb-119">Request headers</span></span>
|<span data-ttu-id="18ebb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18ebb-120">Header</span></span>|<span data-ttu-id="18ebb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="18ebb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18ebb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="18ebb-122">Authorization</span></span>|<span data-ttu-id="18ebb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18ebb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18ebb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="18ebb-124">Accept</span></span>|<span data-ttu-id="18ebb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18ebb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18ebb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18ebb-126">Request body</span></span>
<span data-ttu-id="18ebb-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="18ebb-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

<span data-ttu-id="18ebb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span><span class="sxs-lookup"><span data-stu-id="18ebb-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>

|<span data-ttu-id="18ebb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18ebb-129">Property</span></span>|<span data-ttu-id="18ebb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="18ebb-130">Type</span></span>|<span data-ttu-id="18ebb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="18ebb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18ebb-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18ebb-132">lastModifiedDateTime</span></span>|<span data-ttu-id="18ebb-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18ebb-133">DateTimeOffset</span></span>|<span data-ttu-id="18ebb-134">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="18ebb-134">The date and time the object was last modified.</span></span> <span data-ttu-id="18ebb-135">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="18ebb-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="18ebb-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18ebb-136">createdDateTime</span></span>|<span data-ttu-id="18ebb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18ebb-137">DateTimeOffset</span></span>|<span data-ttu-id="18ebb-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="18ebb-138">The date and time the object was created.</span></span> <span data-ttu-id="18ebb-139">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="18ebb-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="18ebb-140">id</span><span class="sxs-lookup"><span data-stu-id="18ebb-140">id</span></span>|<span data-ttu-id="18ebb-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18ebb-141">String</span></span>|<span data-ttu-id="18ebb-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="18ebb-142">Key of the entity.</span></span> <span data-ttu-id="18ebb-143">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="18ebb-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="18ebb-144">values</span><span class="sxs-lookup"><span data-stu-id="18ebb-144">values</span></span>|<span data-ttu-id="18ebb-145">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="18ebb-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="18ebb-146">Uma lista de pares para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="18ebb-146">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="18ebb-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="18ebb-147">Response</span></span>
<span data-ttu-id="18ebb-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18ebb-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18ebb-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18ebb-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="18ebb-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18ebb-150">Request</span></span>
<span data-ttu-id="18ebb-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18ebb-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18ebb-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="18ebb-152">Response</span></span>
<span data-ttu-id="18ebb-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18ebb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




