---
title: Criar groupPolicyPresentationValueList
description: Criar um novo objeto groupPolicyPresentationValueList.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a98f68e5a12fae5dc58da301bd730b1616b9fc61
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734333"
---
# <a name="create-grouppolicypresentationvaluelist"></a><span data-ttu-id="29c5c-103">Criar groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="29c5c-103">Create groupPolicyPresentationValueList</span></span>

<span data-ttu-id="29c5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29c5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29c5c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29c5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29c5c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29c5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29c5c-107">Criar um novo objeto [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="29c5c-107">Create a new [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29c5c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29c5c-108">Prerequisites</span></span>
<span data-ttu-id="29c5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29c5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29c5c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29c5c-111">Permission type</span></span>|<span data-ttu-id="29c5c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29c5c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29c5c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29c5c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29c5c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29c5c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="29c5c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29c5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29c5c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29c5c-116">Not supported.</span></span>|
|<span data-ttu-id="29c5c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29c5c-117">Application</span></span>|<span data-ttu-id="29c5c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29c5c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29c5c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29c5c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="29c5c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29c5c-120">Request headers</span></span>
|<span data-ttu-id="29c5c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29c5c-121">Header</span></span>|<span data-ttu-id="29c5c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="29c5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29c5c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="29c5c-123">Authorization</span></span>|<span data-ttu-id="29c5c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29c5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29c5c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29c5c-125">Accept</span></span>|<span data-ttu-id="29c5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29c5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29c5c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29c5c-127">Request body</span></span>
<span data-ttu-id="29c5c-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationValueList.</span><span class="sxs-lookup"><span data-stu-id="29c5c-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueList object.</span></span>

<span data-ttu-id="29c5c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationValueList.</span><span class="sxs-lookup"><span data-stu-id="29c5c-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueList.</span></span>

|<span data-ttu-id="29c5c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29c5c-130">Property</span></span>|<span data-ttu-id="29c5c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="29c5c-131">Type</span></span>|<span data-ttu-id="29c5c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="29c5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29c5c-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29c5c-133">lastModifiedDateTime</span></span>|<span data-ttu-id="29c5c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29c5c-134">DateTimeOffset</span></span>|<span data-ttu-id="29c5c-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="29c5c-135">The date and time the object was last modified.</span></span> <span data-ttu-id="29c5c-136">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="29c5c-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="29c5c-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29c5c-137">createdDateTime</span></span>|<span data-ttu-id="29c5c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29c5c-138">DateTimeOffset</span></span>|<span data-ttu-id="29c5c-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="29c5c-139">The date and time the object was created.</span></span> <span data-ttu-id="29c5c-140">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="29c5c-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="29c5c-141">id</span><span class="sxs-lookup"><span data-stu-id="29c5c-141">id</span></span>|<span data-ttu-id="29c5c-142">String</span><span class="sxs-lookup"><span data-stu-id="29c5c-142">String</span></span>|<span data-ttu-id="29c5c-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="29c5c-143">Key of the entity.</span></span> <span data-ttu-id="29c5c-144">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="29c5c-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="29c5c-145">values</span><span class="sxs-lookup"><span data-stu-id="29c5c-145">values</span></span>|<span data-ttu-id="29c5c-146">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="29c5c-146">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="29c5c-147">Uma lista de pares para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="29c5c-147">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="29c5c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="29c5c-148">Response</span></span>
<span data-ttu-id="29c5c-149">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29c5c-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29c5c-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29c5c-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="29c5c-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29c5c-151">Request</span></span>
<span data-ttu-id="29c5c-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29c5c-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
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

### <a name="response"></a><span data-ttu-id="29c5c-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="29c5c-153">Response</span></span>
<span data-ttu-id="29c5c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29c5c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





