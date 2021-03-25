---
title: Criar groupPolicyPresentationValueText
description: Crie um novo objeto groupPolicyPresentationValueText.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8cddae999d99b9a0f8bc9929cf253f181d56c507
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157133"
---
# <a name="create-grouppolicypresentationvaluetext"></a><span data-ttu-id="d20fb-103">Criar groupPolicyPresentationValueText</span><span class="sxs-lookup"><span data-stu-id="d20fb-103">Create groupPolicyPresentationValueText</span></span>

<span data-ttu-id="d20fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d20fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d20fb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d20fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d20fb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d20fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d20fb-107">Crie um novo [objeto groupPolicyPresentationValueText.](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)</span><span class="sxs-lookup"><span data-stu-id="d20fb-107">Create a new [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d20fb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d20fb-108">Prerequisites</span></span>
<span data-ttu-id="d20fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d20fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d20fb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d20fb-111">Permission type</span></span>|<span data-ttu-id="d20fb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d20fb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d20fb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d20fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d20fb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d20fb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d20fb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d20fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d20fb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d20fb-116">Not supported.</span></span>|
|<span data-ttu-id="d20fb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d20fb-117">Application</span></span>|<span data-ttu-id="d20fb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d20fb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d20fb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d20fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="d20fb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d20fb-120">Request headers</span></span>
|<span data-ttu-id="d20fb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d20fb-121">Header</span></span>|<span data-ttu-id="d20fb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d20fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d20fb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d20fb-123">Authorization</span></span>|<span data-ttu-id="d20fb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d20fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d20fb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d20fb-125">Accept</span></span>|<span data-ttu-id="d20fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d20fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d20fb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d20fb-127">Request body</span></span>
<span data-ttu-id="d20fb-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationValueText.</span><span class="sxs-lookup"><span data-stu-id="d20fb-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueText object.</span></span>

<span data-ttu-id="d20fb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyPresentationValueText.</span><span class="sxs-lookup"><span data-stu-id="d20fb-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueText.</span></span>

|<span data-ttu-id="d20fb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d20fb-130">Property</span></span>|<span data-ttu-id="d20fb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d20fb-131">Type</span></span>|<span data-ttu-id="d20fb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d20fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d20fb-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d20fb-133">lastModifiedDateTime</span></span>|<span data-ttu-id="d20fb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d20fb-134">DateTimeOffset</span></span>|<span data-ttu-id="d20fb-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d20fb-135">The date and time the object was last modified.</span></span> <span data-ttu-id="d20fb-136">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d20fb-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="d20fb-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d20fb-137">createdDateTime</span></span>|<span data-ttu-id="d20fb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d20fb-138">DateTimeOffset</span></span>|<span data-ttu-id="d20fb-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d20fb-139">The date and time the object was created.</span></span> <span data-ttu-id="d20fb-140">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d20fb-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="d20fb-141">id</span><span class="sxs-lookup"><span data-stu-id="d20fb-141">id</span></span>|<span data-ttu-id="d20fb-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d20fb-142">String</span></span>|<span data-ttu-id="d20fb-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d20fb-143">Key of the entity.</span></span> <span data-ttu-id="d20fb-144">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d20fb-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="d20fb-145">value</span><span class="sxs-lookup"><span data-stu-id="d20fb-145">value</span></span>|<span data-ttu-id="d20fb-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d20fb-146">String</span></span>|<span data-ttu-id="d20fb-147">Um valor de cadeia de caracteres para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="d20fb-147">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="d20fb-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="d20fb-148">Response</span></span>
<span data-ttu-id="d20fb-149">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d20fb-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d20fb-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d20fb-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="d20fb-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d20fb-151">Request</span></span>
<span data-ttu-id="d20fb-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d20fb-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="d20fb-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d20fb-153">Response</span></span>
<span data-ttu-id="d20fb-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d20fb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




