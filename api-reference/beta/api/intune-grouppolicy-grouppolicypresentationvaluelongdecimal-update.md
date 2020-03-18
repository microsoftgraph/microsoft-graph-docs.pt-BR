---
title: Atualizar groupPolicyPresentationValueLongDecimal
description: Atualiza as propriedades de um objeto groupPolicyPresentationValueLongDecimal.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5141f907f3cee59d50535fcb6c9ff71549a65841
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803873"
---
# <a name="update-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="99aa0-103">Atualizar groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="99aa0-103">Update groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="99aa0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99aa0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99aa0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99aa0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99aa0-106">Atualiza as propriedades de um objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="99aa0-106">Update the properties of a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99aa0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99aa0-107">Prerequisites</span></span>
<span data-ttu-id="99aa0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99aa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99aa0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99aa0-110">Permission type</span></span>|<span data-ttu-id="99aa0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99aa0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99aa0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99aa0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99aa0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99aa0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="99aa0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99aa0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99aa0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99aa0-115">Not supported.</span></span>|
|<span data-ttu-id="99aa0-116">Application</span><span class="sxs-lookup"><span data-stu-id="99aa0-116">Application</span></span>|<span data-ttu-id="99aa0-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99aa0-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99aa0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99aa0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="99aa0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99aa0-119">Request headers</span></span>
|<span data-ttu-id="99aa0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99aa0-120">Header</span></span>|<span data-ttu-id="99aa0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="99aa0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99aa0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="99aa0-122">Authorization</span></span>|<span data-ttu-id="99aa0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99aa0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99aa0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99aa0-124">Accept</span></span>|<span data-ttu-id="99aa0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="99aa0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99aa0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99aa0-126">Request body</span></span>
<span data-ttu-id="99aa0-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="99aa0-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

<span data-ttu-id="99aa0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span><span class="sxs-lookup"><span data-stu-id="99aa0-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span></span>

|<span data-ttu-id="99aa0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99aa0-129">Property</span></span>|<span data-ttu-id="99aa0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="99aa0-130">Type</span></span>|<span data-ttu-id="99aa0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="99aa0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99aa0-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99aa0-132">lastModifiedDateTime</span></span>|<span data-ttu-id="99aa0-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99aa0-133">DateTimeOffset</span></span>|<span data-ttu-id="99aa0-134">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="99aa0-134">The date and time the object was last modified.</span></span> <span data-ttu-id="99aa0-135">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="99aa0-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="99aa0-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99aa0-136">createdDateTime</span></span>|<span data-ttu-id="99aa0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99aa0-137">DateTimeOffset</span></span>|<span data-ttu-id="99aa0-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="99aa0-138">The date and time the object was created.</span></span> <span data-ttu-id="99aa0-139">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="99aa0-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="99aa0-140">id</span><span class="sxs-lookup"><span data-stu-id="99aa0-140">id</span></span>|<span data-ttu-id="99aa0-141">String</span><span class="sxs-lookup"><span data-stu-id="99aa0-141">String</span></span>|<span data-ttu-id="99aa0-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="99aa0-142">Key of the entity.</span></span> <span data-ttu-id="99aa0-143">Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="99aa0-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="99aa0-144">valor</span><span class="sxs-lookup"><span data-stu-id="99aa0-144">value</span></span>|<span data-ttu-id="99aa0-145">Int64</span><span class="sxs-lookup"><span data-stu-id="99aa0-145">Int64</span></span>|<span data-ttu-id="99aa0-146">Um valor Long não assinado para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="99aa0-146">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="99aa0-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="99aa0-147">Response</span></span>
<span data-ttu-id="99aa0-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99aa0-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99aa0-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99aa0-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="99aa0-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99aa0-150">Request</span></span>
<span data-ttu-id="99aa0-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99aa0-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="99aa0-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="99aa0-152">Response</span></span>
<span data-ttu-id="99aa0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99aa0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




