---
title: Criar groupPolicyPresentationValueDecimal
description: Criar um novo objeto groupPolicyPresentationValueDecimal.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c7c441d9949cd7f5ec17635bc90f0c8873778950
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35989256"
---
# <a name="create-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="645d2-103">Criar groupPolicyPresentationValueDecimal</span><span class="sxs-lookup"><span data-stu-id="645d2-103">Create groupPolicyPresentationValueDecimal</span></span>

> <span data-ttu-id="645d2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="645d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="645d2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="645d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="645d2-106">Criar um novo objeto [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="645d2-106">Create a new [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="645d2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="645d2-107">Prerequisites</span></span>
<span data-ttu-id="645d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="645d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="645d2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="645d2-110">Permission type</span></span>|<span data-ttu-id="645d2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="645d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="645d2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="645d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="645d2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="645d2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="645d2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="645d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="645d2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="645d2-115">Not supported.</span></span>|
|<span data-ttu-id="645d2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="645d2-116">Application</span></span>|<span data-ttu-id="645d2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="645d2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="645d2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="645d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="645d2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="645d2-119">Request headers</span></span>
|<span data-ttu-id="645d2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="645d2-120">Header</span></span>|<span data-ttu-id="645d2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="645d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="645d2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="645d2-122">Authorization</span></span>|<span data-ttu-id="645d2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="645d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="645d2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="645d2-124">Accept</span></span>|<span data-ttu-id="645d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="645d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="645d2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="645d2-126">Request body</span></span>
<span data-ttu-id="645d2-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationValueDecimal.</span><span class="sxs-lookup"><span data-stu-id="645d2-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueDecimal object.</span></span>

<span data-ttu-id="645d2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationValueDecimal.</span><span class="sxs-lookup"><span data-stu-id="645d2-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueDecimal.</span></span>

|<span data-ttu-id="645d2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="645d2-129">Property</span></span>|<span data-ttu-id="645d2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="645d2-130">Type</span></span>|<span data-ttu-id="645d2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="645d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="645d2-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="645d2-132">lastModifiedDateTime</span></span>|<span data-ttu-id="645d2-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="645d2-133">DateTimeOffset</span></span>|<span data-ttu-id="645d2-134">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="645d2-134">The date and time the object was last modified.</span></span> <span data-ttu-id="645d2-135">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="645d2-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="645d2-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="645d2-136">createdDateTime</span></span>|<span data-ttu-id="645d2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="645d2-137">DateTimeOffset</span></span>|<span data-ttu-id="645d2-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="645d2-138">The date and time the object was created.</span></span> <span data-ttu-id="645d2-139">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="645d2-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="645d2-140">id</span><span class="sxs-lookup"><span data-stu-id="645d2-140">id</span></span>|<span data-ttu-id="645d2-141">String</span><span class="sxs-lookup"><span data-stu-id="645d2-141">String</span></span>|<span data-ttu-id="645d2-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="645d2-142">Key of the entity.</span></span> <span data-ttu-id="645d2-143">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="645d2-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="645d2-144">valor</span><span class="sxs-lookup"><span data-stu-id="645d2-144">value</span></span>|<span data-ttu-id="645d2-145">Int64</span><span class="sxs-lookup"><span data-stu-id="645d2-145">Int64</span></span>|<span data-ttu-id="645d2-146">Um valor inteiro não assinado para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="645d2-146">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="645d2-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="645d2-147">Response</span></span>
<span data-ttu-id="645d2-148">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="645d2-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="645d2-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="645d2-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="645d2-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="645d2-150">Request</span></span>
<span data-ttu-id="645d2-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="645d2-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="645d2-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="645d2-152">Response</span></span>
<span data-ttu-id="645d2-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="645d2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





