---
title: Criar groupPolicyPresentationValueLongDecimal
description: Criar um novo objeto groupPolicyPresentationValueLongDecimal.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d63e947209e4cd5323c8eb34570154164d2f4b56
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37193715"
---
# <a name="create-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="55060-103">Criar groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="55060-103">Create groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="55060-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55060-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55060-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55060-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55060-106">Criar um novo objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="55060-106">Create a new [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55060-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55060-107">Prerequisites</span></span>
<span data-ttu-id="55060-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55060-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55060-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55060-110">Permission type</span></span>|<span data-ttu-id="55060-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55060-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55060-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55060-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55060-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55060-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="55060-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55060-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55060-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55060-115">Not supported.</span></span>|
|<span data-ttu-id="55060-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55060-116">Application</span></span>|<span data-ttu-id="55060-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55060-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55060-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55060-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="55060-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55060-119">Request headers</span></span>
|<span data-ttu-id="55060-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55060-120">Header</span></span>|<span data-ttu-id="55060-121">Valor</span><span class="sxs-lookup"><span data-stu-id="55060-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55060-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="55060-122">Authorization</span></span>|<span data-ttu-id="55060-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55060-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55060-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="55060-124">Accept</span></span>|<span data-ttu-id="55060-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55060-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55060-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55060-126">Request body</span></span>
<span data-ttu-id="55060-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationValueLongDecimal.</span><span class="sxs-lookup"><span data-stu-id="55060-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueLongDecimal object.</span></span>

<span data-ttu-id="55060-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationValueLongDecimal.</span><span class="sxs-lookup"><span data-stu-id="55060-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueLongDecimal.</span></span>

|<span data-ttu-id="55060-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55060-129">Property</span></span>|<span data-ttu-id="55060-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="55060-130">Type</span></span>|<span data-ttu-id="55060-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="55060-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55060-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55060-132">lastModifiedDateTime</span></span>|<span data-ttu-id="55060-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55060-133">DateTimeOffset</span></span>|<span data-ttu-id="55060-134">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="55060-134">The date and time the object was last modified.</span></span> <span data-ttu-id="55060-135">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="55060-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="55060-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55060-136">createdDateTime</span></span>|<span data-ttu-id="55060-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55060-137">DateTimeOffset</span></span>|<span data-ttu-id="55060-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="55060-138">The date and time the object was created.</span></span> <span data-ttu-id="55060-139">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="55060-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="55060-140">id</span><span class="sxs-lookup"><span data-stu-id="55060-140">id</span></span>|<span data-ttu-id="55060-141">String</span><span class="sxs-lookup"><span data-stu-id="55060-141">String</span></span>|<span data-ttu-id="55060-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="55060-142">Key of the entity.</span></span> <span data-ttu-id="55060-143">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="55060-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="55060-144">valor</span><span class="sxs-lookup"><span data-stu-id="55060-144">value</span></span>|<span data-ttu-id="55060-145">Int64</span><span class="sxs-lookup"><span data-stu-id="55060-145">Int64</span></span>|<span data-ttu-id="55060-146">Um valor Long não assinado para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="55060-146">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="55060-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="55060-147">Response</span></span>
<span data-ttu-id="55060-148">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55060-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55060-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55060-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="55060-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55060-150">Request</span></span>
<span data-ttu-id="55060-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55060-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="55060-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="55060-152">Response</span></span>
<span data-ttu-id="55060-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55060-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 268

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "210f7078-7078-210f-7870-0f2178700f21",
  "value": 5
}
```




