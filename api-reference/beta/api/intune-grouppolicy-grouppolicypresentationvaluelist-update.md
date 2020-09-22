---
title: Atualizar groupPolicyPresentationValueList
description: Atualiza as propriedades de um objeto groupPolicyPresentationValueList.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f43f17b95f565fec62d904da566cd33396c6b5d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994607"
---
# <a name="update-grouppolicypresentationvaluelist"></a><span data-ttu-id="b5770-103">Atualizar groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="b5770-103">Update groupPolicyPresentationValueList</span></span>

<span data-ttu-id="b5770-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5770-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5770-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b5770-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5770-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b5770-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5770-107">Atualiza as propriedades de um objeto [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="b5770-107">Update the properties of a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5770-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b5770-108">Prerequisites</span></span>
<span data-ttu-id="b5770-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5770-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5770-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5770-111">Permission type</span></span>|<span data-ttu-id="b5770-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b5770-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5770-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5770-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5770-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5770-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5770-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5770-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5770-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5770-116">Not supported.</span></span>|
|<span data-ttu-id="b5770-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5770-117">Application</span></span>|<span data-ttu-id="b5770-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5770-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5770-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5770-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="b5770-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5770-120">Request headers</span></span>
|<span data-ttu-id="b5770-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b5770-121">Header</span></span>|<span data-ttu-id="b5770-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b5770-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5770-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5770-123">Authorization</span></span>|<span data-ttu-id="b5770-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5770-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5770-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b5770-125">Accept</span></span>|<span data-ttu-id="b5770-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5770-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5770-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5770-127">Request body</span></span>
<span data-ttu-id="b5770-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="b5770-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

<span data-ttu-id="b5770-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span><span class="sxs-lookup"><span data-stu-id="b5770-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>

|<span data-ttu-id="b5770-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5770-130">Property</span></span>|<span data-ttu-id="b5770-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5770-131">Type</span></span>|<span data-ttu-id="b5770-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5770-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5770-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5770-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b5770-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5770-134">DateTimeOffset</span></span>|<span data-ttu-id="b5770-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b5770-135">The date and time the object was last modified.</span></span> <span data-ttu-id="b5770-136">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b5770-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b5770-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5770-137">createdDateTime</span></span>|<span data-ttu-id="b5770-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5770-138">DateTimeOffset</span></span>|<span data-ttu-id="b5770-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b5770-139">The date and time the object was created.</span></span> <span data-ttu-id="b5770-140">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b5770-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b5770-141">id</span><span class="sxs-lookup"><span data-stu-id="b5770-141">id</span></span>|<span data-ttu-id="b5770-142">String</span><span class="sxs-lookup"><span data-stu-id="b5770-142">String</span></span>|<span data-ttu-id="b5770-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b5770-143">Key of the entity.</span></span> <span data-ttu-id="b5770-144">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b5770-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b5770-145">values</span><span class="sxs-lookup"><span data-stu-id="b5770-145">values</span></span>|<span data-ttu-id="b5770-146">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b5770-146">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b5770-147">Uma lista de pares para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="b5770-147">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="b5770-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5770-148">Response</span></span>
<span data-ttu-id="b5770-149">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5770-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5770-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5770-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5770-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5770-151">Request</span></span>
<span data-ttu-id="b5770-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5770-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b5770-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5770-153">Response</span></span>
<span data-ttu-id="b5770-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5770-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






