---
title: Criar groupPolicyPresentationValueText
description: Criar um novo objeto groupPolicyPresentationValueText.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 81f547401e1549b69ce92bfcd5e827350aa6e6bc
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33904080"
---
# <a name="create-grouppolicypresentationvaluetext"></a><span data-ttu-id="cdbbe-103">Criar groupPolicyPresentationValueText</span><span class="sxs-lookup"><span data-stu-id="cdbbe-103">Create groupPolicyPresentationValueText</span></span>

> <span data-ttu-id="cdbbe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cdbbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdbbe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cdbbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdbbe-106">Criar um novo objeto [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="cdbbe-106">Create a new [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdbbe-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cdbbe-107">Prerequisites</span></span>
<span data-ttu-id="cdbbe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdbbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdbbe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdbbe-110">Permission type</span></span>|<span data-ttu-id="cdbbe-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cdbbe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdbbe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdbbe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cdbbe-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdbbe-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cdbbe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdbbe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdbbe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdbbe-115">Not supported.</span></span>|
|<span data-ttu-id="cdbbe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdbbe-116">Application</span></span>|<span data-ttu-id="cdbbe-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdbbe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdbbe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdbbe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="cdbbe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdbbe-119">Request headers</span></span>
|<span data-ttu-id="cdbbe-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cdbbe-120">Header</span></span>|<span data-ttu-id="cdbbe-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cdbbe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdbbe-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdbbe-122">Authorization</span></span>|<span data-ttu-id="cdbbe-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdbbe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdbbe-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cdbbe-124">Accept</span></span>|<span data-ttu-id="cdbbe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cdbbe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdbbe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdbbe-126">Request body</span></span>
<span data-ttu-id="cdbbe-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyPresentationValueText.</span><span class="sxs-lookup"><span data-stu-id="cdbbe-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueText object.</span></span>

<span data-ttu-id="cdbbe-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyPresentationValueText.</span><span class="sxs-lookup"><span data-stu-id="cdbbe-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueText.</span></span>

|<span data-ttu-id="cdbbe-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cdbbe-129">Property</span></span>|<span data-ttu-id="cdbbe-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdbbe-130">Type</span></span>|<span data-ttu-id="cdbbe-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdbbe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdbbe-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cdbbe-132">lastModifiedDateTime</span></span>|<span data-ttu-id="cdbbe-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdbbe-133">DateTimeOffset</span></span>|<span data-ttu-id="cdbbe-134">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cdbbe-134">The date and time the object was last modified.</span></span> <span data-ttu-id="cdbbe-135">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="cdbbe-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="cdbbe-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cdbbe-136">createdDateTime</span></span>|<span data-ttu-id="cdbbe-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdbbe-137">DateTimeOffset</span></span>|<span data-ttu-id="cdbbe-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="cdbbe-138">The date and time the object was created.</span></span> <span data-ttu-id="cdbbe-139">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="cdbbe-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="cdbbe-140">id</span><span class="sxs-lookup"><span data-stu-id="cdbbe-140">id</span></span>|<span data-ttu-id="cdbbe-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cdbbe-141">String</span></span>|<span data-ttu-id="cdbbe-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cdbbe-142">Key of the entity.</span></span> <span data-ttu-id="cdbbe-143">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="cdbbe-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="cdbbe-144">value</span><span class="sxs-lookup"><span data-stu-id="cdbbe-144">value</span></span>|<span data-ttu-id="cdbbe-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cdbbe-145">String</span></span>|<span data-ttu-id="cdbbe-146">Um valor String para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="cdbbe-146">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="cdbbe-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdbbe-147">Response</span></span>
<span data-ttu-id="cdbbe-148">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdbbe-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdbbe-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdbbe-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdbbe-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdbbe-150">Request</span></span>
<span data-ttu-id="cdbbe-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdbbe-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="cdbbe-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdbbe-152">Response</span></span>
<span data-ttu-id="cdbbe-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cdbbe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 273

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "a3883444-3444-a388-4434-88a3443488a3",
  "value": "Value value"
}
```




