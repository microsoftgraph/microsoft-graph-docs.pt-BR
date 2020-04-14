---
title: Criar groupPolicyPresentationValueLongDecimal
description: Criar um novo objeto groupPolicyPresentationValueLongDecimal.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 711bac80a5a04eb99ce84613855c12e2aaed58bb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460248"
---
# <a name="create-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="3051a-103">Criar groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="3051a-103">Create groupPolicyPresentationValueLongDecimal</span></span>

<span data-ttu-id="3051a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3051a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3051a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3051a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3051a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3051a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3051a-107">Criar um novo objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="3051a-107">Create a new [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3051a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3051a-108">Prerequisites</span></span>
<span data-ttu-id="3051a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3051a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3051a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3051a-111">Permission type</span></span>|<span data-ttu-id="3051a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3051a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3051a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3051a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3051a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3051a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3051a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3051a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3051a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3051a-116">Not supported.</span></span>|
|<span data-ttu-id="3051a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3051a-117">Application</span></span>|<span data-ttu-id="3051a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3051a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3051a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3051a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="3051a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3051a-120">Request headers</span></span>
|<span data-ttu-id="3051a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3051a-121">Header</span></span>|<span data-ttu-id="3051a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3051a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3051a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3051a-123">Authorization</span></span>|<span data-ttu-id="3051a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3051a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3051a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3051a-125">Accept</span></span>|<span data-ttu-id="3051a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3051a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3051a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3051a-127">Request body</span></span>
<span data-ttu-id="3051a-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationValueLongDecimal.</span><span class="sxs-lookup"><span data-stu-id="3051a-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueLongDecimal object.</span></span>

<span data-ttu-id="3051a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationValueLongDecimal.</span><span class="sxs-lookup"><span data-stu-id="3051a-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueLongDecimal.</span></span>

|<span data-ttu-id="3051a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3051a-130">Property</span></span>|<span data-ttu-id="3051a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3051a-131">Type</span></span>|<span data-ttu-id="3051a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3051a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3051a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3051a-133">lastModifiedDateTime</span></span>|<span data-ttu-id="3051a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3051a-134">DateTimeOffset</span></span>|<span data-ttu-id="3051a-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3051a-135">The date and time the object was last modified.</span></span> <span data-ttu-id="3051a-136">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3051a-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3051a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3051a-137">createdDateTime</span></span>|<span data-ttu-id="3051a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3051a-138">DateTimeOffset</span></span>|<span data-ttu-id="3051a-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3051a-139">The date and time the object was created.</span></span> <span data-ttu-id="3051a-140">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3051a-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3051a-141">id</span><span class="sxs-lookup"><span data-stu-id="3051a-141">id</span></span>|<span data-ttu-id="3051a-142">String</span><span class="sxs-lookup"><span data-stu-id="3051a-142">String</span></span>|<span data-ttu-id="3051a-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3051a-143">Key of the entity.</span></span> <span data-ttu-id="3051a-144">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3051a-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3051a-145">valor</span><span class="sxs-lookup"><span data-stu-id="3051a-145">value</span></span>|<span data-ttu-id="3051a-146">Int64</span><span class="sxs-lookup"><span data-stu-id="3051a-146">Int64</span></span>|<span data-ttu-id="3051a-147">Um valor Long não assinado para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="3051a-147">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="3051a-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="3051a-148">Response</span></span>
<span data-ttu-id="3051a-149">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3051a-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3051a-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3051a-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="3051a-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3051a-151">Request</span></span>
<span data-ttu-id="3051a-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3051a-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="3051a-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="3051a-153">Response</span></span>
<span data-ttu-id="3051a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3051a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



