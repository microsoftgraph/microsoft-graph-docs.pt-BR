---
title: Atualizar groupPolicyPresentationValueLongDecimal
description: Atualize as propriedades de um objeto groupPolicyPresentationValueLongDecimal.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 29db585995728b84f6f4157c5e3c61c0ffa3fe7d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145730"
---
# <a name="update-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="a51df-103">Atualizar groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="a51df-103">Update groupPolicyPresentationValueLongDecimal</span></span>

<span data-ttu-id="a51df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a51df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a51df-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a51df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a51df-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a51df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a51df-107">Atualize as propriedades de [um objeto groupPolicyPresentationValueLongDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)</span><span class="sxs-lookup"><span data-stu-id="a51df-107">Update the properties of a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a51df-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a51df-108">Prerequisites</span></span>
<span data-ttu-id="a51df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a51df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a51df-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a51df-111">Permission type</span></span>|<span data-ttu-id="a51df-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a51df-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a51df-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a51df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a51df-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a51df-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a51df-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a51df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a51df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a51df-116">Not supported.</span></span>|
|<span data-ttu-id="a51df-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a51df-117">Application</span></span>|<span data-ttu-id="a51df-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a51df-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a51df-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a51df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="a51df-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a51df-120">Request headers</span></span>
|<span data-ttu-id="a51df-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a51df-121">Header</span></span>|<span data-ttu-id="a51df-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a51df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a51df-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a51df-123">Authorization</span></span>|<span data-ttu-id="a51df-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a51df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a51df-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a51df-125">Accept</span></span>|<span data-ttu-id="a51df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a51df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a51df-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a51df-127">Request body</span></span>
<span data-ttu-id="a51df-128">No corpo da solicitação, fornece uma representação JSON para [o objeto groupPolicyPresentationValueLongDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)</span><span class="sxs-lookup"><span data-stu-id="a51df-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

<span data-ttu-id="a51df-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span><span class="sxs-lookup"><span data-stu-id="a51df-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span></span>

|<span data-ttu-id="a51df-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a51df-130">Property</span></span>|<span data-ttu-id="a51df-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a51df-131">Type</span></span>|<span data-ttu-id="a51df-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a51df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a51df-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a51df-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a51df-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a51df-134">DateTimeOffset</span></span>|<span data-ttu-id="a51df-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a51df-135">The date and time the object was last modified.</span></span> <span data-ttu-id="a51df-136">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="a51df-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="a51df-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a51df-137">createdDateTime</span></span>|<span data-ttu-id="a51df-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a51df-138">DateTimeOffset</span></span>|<span data-ttu-id="a51df-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a51df-139">The date and time the object was created.</span></span> <span data-ttu-id="a51df-140">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="a51df-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="a51df-141">id</span><span class="sxs-lookup"><span data-stu-id="a51df-141">id</span></span>|<span data-ttu-id="a51df-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a51df-142">String</span></span>|<span data-ttu-id="a51df-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a51df-143">Key of the entity.</span></span> <span data-ttu-id="a51df-144">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="a51df-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="a51df-145">valor</span><span class="sxs-lookup"><span data-stu-id="a51df-145">value</span></span>|<span data-ttu-id="a51df-146">Int64</span><span class="sxs-lookup"><span data-stu-id="a51df-146">Int64</span></span>|<span data-ttu-id="a51df-147">Um valor longo não assinado para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="a51df-147">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="a51df-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a51df-148">Response</span></span>
<span data-ttu-id="a51df-149">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a51df-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a51df-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a51df-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="a51df-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a51df-151">Request</span></span>
<span data-ttu-id="a51df-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a51df-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="a51df-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a51df-153">Response</span></span>
<span data-ttu-id="a51df-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a51df-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




