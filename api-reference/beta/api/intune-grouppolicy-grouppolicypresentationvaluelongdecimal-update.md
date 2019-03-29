---
title: Atualizar groupPolicyPresentationValueLongDecimal
description: Atualiza as propriedades de um objeto groupPolicyPresentationValueLongDecimal.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cddaed3f562df00e25854bba6beb1f00ee832d43
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968018"
---
# <a name="update-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="b28bb-103">Atualizar groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="b28bb-103">Update groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="b28bb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b28bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b28bb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b28bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b28bb-106">Atualiza as propriedades de um objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="b28bb-106">Update the properties of a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b28bb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b28bb-107">Prerequisites</span></span>
<span data-ttu-id="b28bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b28bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b28bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b28bb-110">Permission type</span></span>|<span data-ttu-id="b28bb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b28bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b28bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b28bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b28bb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b28bb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b28bb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b28bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b28bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b28bb-115">Not supported.</span></span>|
|<span data-ttu-id="b28bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b28bb-116">Application</span></span>|<span data-ttu-id="b28bb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b28bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b28bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b28bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="b28bb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b28bb-119">Request headers</span></span>
|<span data-ttu-id="b28bb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b28bb-120">Header</span></span>|<span data-ttu-id="b28bb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b28bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b28bb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b28bb-122">Authorization</span></span>|<span data-ttu-id="b28bb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b28bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b28bb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b28bb-124">Accept</span></span>|<span data-ttu-id="b28bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b28bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b28bb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b28bb-126">Request body</span></span>
<span data-ttu-id="b28bb-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="b28bb-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

<span data-ttu-id="b28bb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span><span class="sxs-lookup"><span data-stu-id="b28bb-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span></span>

|<span data-ttu-id="b28bb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b28bb-129">Property</span></span>|<span data-ttu-id="b28bb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b28bb-130">Type</span></span>|<span data-ttu-id="b28bb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b28bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b28bb-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b28bb-132">lastModifiedDateTime</span></span>|<span data-ttu-id="b28bb-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b28bb-133">DateTimeOffset</span></span>|<span data-ttu-id="b28bb-134">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b28bb-134">The date and time the object was last modified.</span></span> <span data-ttu-id="b28bb-135">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b28bb-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b28bb-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b28bb-136">createdDateTime</span></span>|<span data-ttu-id="b28bb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b28bb-137">DateTimeOffset</span></span>|<span data-ttu-id="b28bb-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b28bb-138">The date and time the object was created.</span></span> <span data-ttu-id="b28bb-139">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b28bb-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b28bb-140">id</span><span class="sxs-lookup"><span data-stu-id="b28bb-140">id</span></span>|<span data-ttu-id="b28bb-141">String</span><span class="sxs-lookup"><span data-stu-id="b28bb-141">String</span></span>|<span data-ttu-id="b28bb-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b28bb-142">Key of the entity.</span></span> <span data-ttu-id="b28bb-143">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b28bb-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b28bb-144">value</span><span class="sxs-lookup"><span data-stu-id="b28bb-144">value</span></span>|<span data-ttu-id="b28bb-145">Int64</span><span class="sxs-lookup"><span data-stu-id="b28bb-145">Int64</span></span>|<span data-ttu-id="b28bb-146">Um valor Long não assinado para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="b28bb-146">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="b28bb-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="b28bb-147">Response</span></span>
<span data-ttu-id="b28bb-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b28bb-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b28bb-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b28bb-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="b28bb-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b28bb-150">Request</span></span>
<span data-ttu-id="b28bb-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b28bb-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="b28bb-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="b28bb-152">Response</span></span>
<span data-ttu-id="b28bb-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b28bb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




