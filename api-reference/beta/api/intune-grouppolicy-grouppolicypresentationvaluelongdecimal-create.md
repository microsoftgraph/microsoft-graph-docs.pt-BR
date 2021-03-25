---
title: Criar groupPolicyPresentationValueLongDecimal
description: Crie um novo objeto groupPolicyPresentationValueLongDecimal.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9164f48349106c411977cf0e229cdeb51fcffdff
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157161"
---
# <a name="create-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="d9401-103">Criar groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="d9401-103">Create groupPolicyPresentationValueLongDecimal</span></span>

<span data-ttu-id="d9401-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9401-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9401-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9401-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9401-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9401-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9401-107">Crie um novo [objeto groupPolicyPresentationValueLongDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)</span><span class="sxs-lookup"><span data-stu-id="d9401-107">Create a new [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9401-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9401-108">Prerequisites</span></span>
<span data-ttu-id="d9401-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9401-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9401-111">Permission type</span></span>|<span data-ttu-id="d9401-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9401-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9401-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9401-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9401-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9401-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9401-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9401-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9401-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9401-116">Not supported.</span></span>|
|<span data-ttu-id="d9401-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9401-117">Application</span></span>|<span data-ttu-id="d9401-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9401-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9401-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9401-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="d9401-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9401-120">Request headers</span></span>
|<span data-ttu-id="d9401-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9401-121">Header</span></span>|<span data-ttu-id="d9401-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d9401-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9401-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9401-123">Authorization</span></span>|<span data-ttu-id="d9401-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9401-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9401-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9401-125">Accept</span></span>|<span data-ttu-id="d9401-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9401-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9401-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9401-127">Request body</span></span>
<span data-ttu-id="d9401-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyPresentationValueLongDecimal.</span><span class="sxs-lookup"><span data-stu-id="d9401-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueLongDecimal object.</span></span>

<span data-ttu-id="d9401-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyPresentationValueLongDecimal.</span><span class="sxs-lookup"><span data-stu-id="d9401-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueLongDecimal.</span></span>

|<span data-ttu-id="d9401-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9401-130">Property</span></span>|<span data-ttu-id="d9401-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9401-131">Type</span></span>|<span data-ttu-id="d9401-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9401-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9401-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9401-133">lastModifiedDateTime</span></span>|<span data-ttu-id="d9401-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9401-134">DateTimeOffset</span></span>|<span data-ttu-id="d9401-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d9401-135">The date and time the object was last modified.</span></span> <span data-ttu-id="d9401-136">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d9401-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="d9401-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9401-137">createdDateTime</span></span>|<span data-ttu-id="d9401-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9401-138">DateTimeOffset</span></span>|<span data-ttu-id="d9401-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d9401-139">The date and time the object was created.</span></span> <span data-ttu-id="d9401-140">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d9401-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="d9401-141">id</span><span class="sxs-lookup"><span data-stu-id="d9401-141">id</span></span>|<span data-ttu-id="d9401-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9401-142">String</span></span>|<span data-ttu-id="d9401-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d9401-143">Key of the entity.</span></span> <span data-ttu-id="d9401-144">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d9401-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="d9401-145">valor</span><span class="sxs-lookup"><span data-stu-id="d9401-145">value</span></span>|<span data-ttu-id="d9401-146">Int64</span><span class="sxs-lookup"><span data-stu-id="d9401-146">Int64</span></span>|<span data-ttu-id="d9401-147">Um valor longo não assinado para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="d9401-147">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="d9401-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9401-148">Response</span></span>
<span data-ttu-id="d9401-149">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9401-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9401-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9401-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9401-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9401-151">Request</span></span>
<span data-ttu-id="d9401-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9401-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="d9401-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9401-153">Response</span></span>
<span data-ttu-id="d9401-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9401-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




