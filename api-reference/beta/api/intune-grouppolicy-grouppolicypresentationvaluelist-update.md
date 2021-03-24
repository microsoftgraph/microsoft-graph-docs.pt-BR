---
title: Atualizar groupPolicyPresentationValueList
description: Atualize as propriedades de um objeto groupPolicyPresentationValueList.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 46f7658a559098ece77d880d2c43e894b27dc95c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125993"
---
# <a name="update-grouppolicypresentationvaluelist"></a><span data-ttu-id="3ceee-103">Atualizar groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="3ceee-103">Update groupPolicyPresentationValueList</span></span>

<span data-ttu-id="3ceee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ceee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ceee-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3ceee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ceee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ceee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ceee-107">Atualize as propriedades de [um objeto groupPolicyPresentationValueList.](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)</span><span class="sxs-lookup"><span data-stu-id="3ceee-107">Update the properties of a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ceee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3ceee-108">Prerequisites</span></span>
<span data-ttu-id="3ceee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ceee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ceee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ceee-111">Permission type</span></span>|<span data-ttu-id="3ceee-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ceee-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ceee-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ceee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ceee-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ceee-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3ceee-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ceee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ceee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ceee-116">Not supported.</span></span>|
|<span data-ttu-id="3ceee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ceee-117">Application</span></span>|<span data-ttu-id="3ceee-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ceee-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ceee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ceee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="3ceee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ceee-120">Request headers</span></span>
|<span data-ttu-id="3ceee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3ceee-121">Header</span></span>|<span data-ttu-id="3ceee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3ceee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ceee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ceee-123">Authorization</span></span>|<span data-ttu-id="3ceee-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ceee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ceee-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3ceee-125">Accept</span></span>|<span data-ttu-id="3ceee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ceee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ceee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ceee-127">Request body</span></span>
<span data-ttu-id="3ceee-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicyPresentationValueList.](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)</span><span class="sxs-lookup"><span data-stu-id="3ceee-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

<span data-ttu-id="3ceee-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span><span class="sxs-lookup"><span data-stu-id="3ceee-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>

|<span data-ttu-id="3ceee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ceee-130">Property</span></span>|<span data-ttu-id="3ceee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ceee-131">Type</span></span>|<span data-ttu-id="3ceee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ceee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ceee-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ceee-133">lastModifiedDateTime</span></span>|<span data-ttu-id="3ceee-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ceee-134">DateTimeOffset</span></span>|<span data-ttu-id="3ceee-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3ceee-135">The date and time the object was last modified.</span></span> <span data-ttu-id="3ceee-136">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3ceee-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3ceee-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ceee-137">createdDateTime</span></span>|<span data-ttu-id="3ceee-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ceee-138">DateTimeOffset</span></span>|<span data-ttu-id="3ceee-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3ceee-139">The date and time the object was created.</span></span> <span data-ttu-id="3ceee-140">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3ceee-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3ceee-141">id</span><span class="sxs-lookup"><span data-stu-id="3ceee-141">id</span></span>|<span data-ttu-id="3ceee-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ceee-142">String</span></span>|<span data-ttu-id="3ceee-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3ceee-143">Key of the entity.</span></span> <span data-ttu-id="3ceee-144">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3ceee-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3ceee-145">values</span><span class="sxs-lookup"><span data-stu-id="3ceee-145">values</span></span>|<span data-ttu-id="3ceee-146">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="3ceee-146">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3ceee-147">Uma lista de pares para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="3ceee-147">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="3ceee-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ceee-148">Response</span></span>
<span data-ttu-id="3ceee-149">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ceee-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ceee-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ceee-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ceee-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ceee-151">Request</span></span>
<span data-ttu-id="3ceee-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ceee-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3ceee-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ceee-153">Response</span></span>
<span data-ttu-id="3ceee-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ceee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




