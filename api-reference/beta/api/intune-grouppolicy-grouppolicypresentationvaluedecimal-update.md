---
title: Atualizar groupPolicyPresentationValueDecimal
description: Atualiza as propriedades de um objeto groupPolicyPresentationValueDecimal.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 67c6e52bda7334d47602a045f8a61f8d3fd02876
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37193778"
---
# <a name="update-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="ab125-103">Atualizar groupPolicyPresentationValueDecimal</span><span class="sxs-lookup"><span data-stu-id="ab125-103">Update groupPolicyPresentationValueDecimal</span></span>

> <span data-ttu-id="ab125-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ab125-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab125-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ab125-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab125-106">Atualiza as propriedades de um objeto [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="ab125-106">Update the properties of a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab125-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ab125-107">Prerequisites</span></span>
<span data-ttu-id="ab125-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab125-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab125-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab125-110">Permission type</span></span>|<span data-ttu-id="ab125-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ab125-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab125-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab125-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ab125-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab125-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ab125-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab125-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab125-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab125-115">Not supported.</span></span>|
|<span data-ttu-id="ab125-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab125-116">Application</span></span>|<span data-ttu-id="ab125-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab125-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab125-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab125-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="ab125-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab125-119">Request headers</span></span>
|<span data-ttu-id="ab125-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab125-120">Header</span></span>|<span data-ttu-id="ab125-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ab125-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab125-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab125-122">Authorization</span></span>|<span data-ttu-id="ab125-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab125-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab125-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ab125-124">Accept</span></span>|<span data-ttu-id="ab125-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ab125-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab125-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab125-126">Request body</span></span>
<span data-ttu-id="ab125-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="ab125-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

<span data-ttu-id="ab125-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md).</span><span class="sxs-lookup"><span data-stu-id="ab125-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md).</span></span>

|<span data-ttu-id="ab125-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab125-129">Property</span></span>|<span data-ttu-id="ab125-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab125-130">Type</span></span>|<span data-ttu-id="ab125-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab125-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab125-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab125-132">lastModifiedDateTime</span></span>|<span data-ttu-id="ab125-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab125-133">DateTimeOffset</span></span>|<span data-ttu-id="ab125-134">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ab125-134">The date and time the object was last modified.</span></span> <span data-ttu-id="ab125-135">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ab125-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="ab125-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab125-136">createdDateTime</span></span>|<span data-ttu-id="ab125-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab125-137">DateTimeOffset</span></span>|<span data-ttu-id="ab125-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ab125-138">The date and time the object was created.</span></span> <span data-ttu-id="ab125-139">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ab125-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="ab125-140">id</span><span class="sxs-lookup"><span data-stu-id="ab125-140">id</span></span>|<span data-ttu-id="ab125-141">String</span><span class="sxs-lookup"><span data-stu-id="ab125-141">String</span></span>|<span data-ttu-id="ab125-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ab125-142">Key of the entity.</span></span> <span data-ttu-id="ab125-143">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ab125-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="ab125-144">valor</span><span class="sxs-lookup"><span data-stu-id="ab125-144">value</span></span>|<span data-ttu-id="ab125-145">Int64</span><span class="sxs-lookup"><span data-stu-id="ab125-145">Int64</span></span>|<span data-ttu-id="ab125-146">Um valor inteiro não assinado para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="ab125-146">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="ab125-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab125-147">Response</span></span>
<span data-ttu-id="ab125-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab125-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab125-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab125-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab125-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab125-150">Request</span></span>
<span data-ttu-id="ab125-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab125-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="ab125-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab125-152">Response</span></span>
<span data-ttu-id="ab125-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab125-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 264

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8821bede-bede-8821-debe-2188debe2188",
  "value": 5
}
```




