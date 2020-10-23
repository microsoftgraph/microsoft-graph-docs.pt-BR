---
title: Atualizar groupPolicyPresentationValueLongDecimal
description: Atualiza as propriedades de um objeto groupPolicyPresentationValueLongDecimal.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2c82f9555c753546f6926acb503a10f523e3cfe3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698621"
---
# <a name="update-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="2f278-103">Atualizar groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="2f278-103">Update groupPolicyPresentationValueLongDecimal</span></span>

<span data-ttu-id="2f278-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f278-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f278-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f278-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f278-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f278-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f278-107">Atualiza as propriedades de um objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="2f278-107">Update the properties of a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f278-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f278-108">Prerequisites</span></span>
<span data-ttu-id="2f278-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f278-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f278-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f278-111">Permission type</span></span>|<span data-ttu-id="2f278-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f278-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f278-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f278-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f278-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f278-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f278-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f278-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f278-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f278-116">Not supported.</span></span>|
|<span data-ttu-id="2f278-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f278-117">Application</span></span>|<span data-ttu-id="2f278-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f278-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f278-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f278-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="2f278-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f278-120">Request headers</span></span>
|<span data-ttu-id="2f278-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f278-121">Header</span></span>|<span data-ttu-id="2f278-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2f278-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f278-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f278-123">Authorization</span></span>|<span data-ttu-id="2f278-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f278-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f278-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f278-125">Accept</span></span>|<span data-ttu-id="2f278-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f278-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f278-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f278-127">Request body</span></span>
<span data-ttu-id="2f278-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="2f278-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

<span data-ttu-id="2f278-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span><span class="sxs-lookup"><span data-stu-id="2f278-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span></span>

|<span data-ttu-id="2f278-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f278-130">Property</span></span>|<span data-ttu-id="2f278-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f278-131">Type</span></span>|<span data-ttu-id="2f278-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f278-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f278-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f278-133">lastModifiedDateTime</span></span>|<span data-ttu-id="2f278-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f278-134">DateTimeOffset</span></span>|<span data-ttu-id="2f278-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2f278-135">The date and time the object was last modified.</span></span> <span data-ttu-id="2f278-136">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2f278-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2f278-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f278-137">createdDateTime</span></span>|<span data-ttu-id="2f278-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f278-138">DateTimeOffset</span></span>|<span data-ttu-id="2f278-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2f278-139">The date and time the object was created.</span></span> <span data-ttu-id="2f278-140">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2f278-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2f278-141">id</span><span class="sxs-lookup"><span data-stu-id="2f278-141">id</span></span>|<span data-ttu-id="2f278-142">String</span><span class="sxs-lookup"><span data-stu-id="2f278-142">String</span></span>|<span data-ttu-id="2f278-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f278-143">Key of the entity.</span></span> <span data-ttu-id="2f278-144">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2f278-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2f278-145">valor</span><span class="sxs-lookup"><span data-stu-id="2f278-145">value</span></span>|<span data-ttu-id="2f278-146">Int64</span><span class="sxs-lookup"><span data-stu-id="2f278-146">Int64</span></span>|<span data-ttu-id="2f278-147">Um valor Long não assinado para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="2f278-147">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="2f278-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f278-148">Response</span></span>
<span data-ttu-id="2f278-149">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f278-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f278-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f278-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f278-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f278-151">Request</span></span>
<span data-ttu-id="2f278-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f278-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="2f278-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f278-153">Response</span></span>
<span data-ttu-id="2f278-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f278-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





