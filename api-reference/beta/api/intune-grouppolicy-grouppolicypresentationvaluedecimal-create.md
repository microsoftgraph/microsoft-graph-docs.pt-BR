---
title: Criar groupPolicyPresentationValueDecimal
description: Criar um novo objeto groupPolicyPresentationValueDecimal.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e4ef33a1f72444fc951b4161bb46225d5d9750c1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464208"
---
# <a name="create-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="36bb5-103">Criar groupPolicyPresentationValueDecimal</span><span class="sxs-lookup"><span data-stu-id="36bb5-103">Create groupPolicyPresentationValueDecimal</span></span>

<span data-ttu-id="36bb5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="36bb5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36bb5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="36bb5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36bb5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="36bb5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36bb5-107">Criar um novo objeto [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="36bb5-107">Create a new [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36bb5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="36bb5-108">Prerequisites</span></span>
<span data-ttu-id="36bb5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36bb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36bb5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36bb5-111">Permission type</span></span>|<span data-ttu-id="36bb5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="36bb5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36bb5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36bb5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36bb5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36bb5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="36bb5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36bb5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36bb5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36bb5-116">Not supported.</span></span>|
|<span data-ttu-id="36bb5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36bb5-117">Application</span></span>|<span data-ttu-id="36bb5-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36bb5-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36bb5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36bb5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="36bb5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36bb5-120">Request headers</span></span>
|<span data-ttu-id="36bb5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36bb5-121">Header</span></span>|<span data-ttu-id="36bb5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="36bb5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36bb5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="36bb5-123">Authorization</span></span>|<span data-ttu-id="36bb5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36bb5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36bb5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="36bb5-125">Accept</span></span>|<span data-ttu-id="36bb5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36bb5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36bb5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36bb5-127">Request body</span></span>
<span data-ttu-id="36bb5-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationValueDecimal.</span><span class="sxs-lookup"><span data-stu-id="36bb5-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueDecimal object.</span></span>

<span data-ttu-id="36bb5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationValueDecimal.</span><span class="sxs-lookup"><span data-stu-id="36bb5-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueDecimal.</span></span>

|<span data-ttu-id="36bb5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36bb5-130">Property</span></span>|<span data-ttu-id="36bb5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="36bb5-131">Type</span></span>|<span data-ttu-id="36bb5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="36bb5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36bb5-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36bb5-133">lastModifiedDateTime</span></span>|<span data-ttu-id="36bb5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36bb5-134">DateTimeOffset</span></span>|<span data-ttu-id="36bb5-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="36bb5-135">The date and time the object was last modified.</span></span> <span data-ttu-id="36bb5-136">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="36bb5-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="36bb5-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36bb5-137">createdDateTime</span></span>|<span data-ttu-id="36bb5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36bb5-138">DateTimeOffset</span></span>|<span data-ttu-id="36bb5-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="36bb5-139">The date and time the object was created.</span></span> <span data-ttu-id="36bb5-140">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="36bb5-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="36bb5-141">id</span><span class="sxs-lookup"><span data-stu-id="36bb5-141">id</span></span>|<span data-ttu-id="36bb5-142">String</span><span class="sxs-lookup"><span data-stu-id="36bb5-142">String</span></span>|<span data-ttu-id="36bb5-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="36bb5-143">Key of the entity.</span></span> <span data-ttu-id="36bb5-144">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="36bb5-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="36bb5-145">valor</span><span class="sxs-lookup"><span data-stu-id="36bb5-145">value</span></span>|<span data-ttu-id="36bb5-146">Int64</span><span class="sxs-lookup"><span data-stu-id="36bb5-146">Int64</span></span>|<span data-ttu-id="36bb5-147">Um valor inteiro não assinado para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="36bb5-147">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="36bb5-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="36bb5-148">Response</span></span>
<span data-ttu-id="36bb5-149">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36bb5-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36bb5-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36bb5-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="36bb5-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36bb5-151">Request</span></span>
<span data-ttu-id="36bb5-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36bb5-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="36bb5-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="36bb5-153">Response</span></span>
<span data-ttu-id="36bb5-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36bb5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





