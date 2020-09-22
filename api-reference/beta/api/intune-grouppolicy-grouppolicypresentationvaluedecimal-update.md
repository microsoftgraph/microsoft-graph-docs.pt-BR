---
title: Atualizar groupPolicyPresentationValueDecimal
description: Atualiza as propriedades de um objeto groupPolicyPresentationValueDecimal.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 94565121784e123b7f59a868a03d7cec69b655a4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047319"
---
# <a name="update-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="13525-103">Atualizar groupPolicyPresentationValueDecimal</span><span class="sxs-lookup"><span data-stu-id="13525-103">Update groupPolicyPresentationValueDecimal</span></span>

<span data-ttu-id="13525-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13525-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13525-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="13525-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13525-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13525-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13525-107">Atualiza as propriedades de um objeto [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="13525-107">Update the properties of a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13525-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13525-108">Prerequisites</span></span>
<span data-ttu-id="13525-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13525-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13525-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13525-111">Permission type</span></span>|<span data-ttu-id="13525-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13525-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13525-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13525-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13525-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13525-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13525-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13525-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13525-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13525-116">Not supported.</span></span>|
|<span data-ttu-id="13525-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13525-117">Application</span></span>|<span data-ttu-id="13525-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13525-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13525-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13525-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="13525-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13525-120">Request headers</span></span>
|<span data-ttu-id="13525-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13525-121">Header</span></span>|<span data-ttu-id="13525-122">Valor</span><span class="sxs-lookup"><span data-stu-id="13525-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13525-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="13525-123">Authorization</span></span>|<span data-ttu-id="13525-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13525-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13525-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13525-125">Accept</span></span>|<span data-ttu-id="13525-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13525-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13525-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13525-127">Request body</span></span>
<span data-ttu-id="13525-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="13525-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

<span data-ttu-id="13525-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md).</span><span class="sxs-lookup"><span data-stu-id="13525-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md).</span></span>

|<span data-ttu-id="13525-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13525-130">Property</span></span>|<span data-ttu-id="13525-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="13525-131">Type</span></span>|<span data-ttu-id="13525-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="13525-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13525-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13525-133">lastModifiedDateTime</span></span>|<span data-ttu-id="13525-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13525-134">DateTimeOffset</span></span>|<span data-ttu-id="13525-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="13525-135">The date and time the object was last modified.</span></span> <span data-ttu-id="13525-136">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="13525-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="13525-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13525-137">createdDateTime</span></span>|<span data-ttu-id="13525-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13525-138">DateTimeOffset</span></span>|<span data-ttu-id="13525-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="13525-139">The date and time the object was created.</span></span> <span data-ttu-id="13525-140">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="13525-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="13525-141">id</span><span class="sxs-lookup"><span data-stu-id="13525-141">id</span></span>|<span data-ttu-id="13525-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13525-142">String</span></span>|<span data-ttu-id="13525-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="13525-143">Key of the entity.</span></span> <span data-ttu-id="13525-144">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="13525-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="13525-145">valor</span><span class="sxs-lookup"><span data-stu-id="13525-145">value</span></span>|<span data-ttu-id="13525-146">Int64</span><span class="sxs-lookup"><span data-stu-id="13525-146">Int64</span></span>|<span data-ttu-id="13525-147">Um valor inteiro não assinado para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="13525-147">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="13525-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="13525-148">Response</span></span>
<span data-ttu-id="13525-149">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13525-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13525-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13525-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="13525-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13525-151">Request</span></span>
<span data-ttu-id="13525-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13525-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="13525-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="13525-153">Response</span></span>
<span data-ttu-id="13525-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13525-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






