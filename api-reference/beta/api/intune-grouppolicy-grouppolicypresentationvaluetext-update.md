---
title: Atualizar groupPolicyPresentationValueText
description: Atualize as propriedades de um objeto groupPolicyPresentationValueText.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 49e65216583e4e928562b5e7b5c053ae97beef3d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157091"
---
# <a name="update-grouppolicypresentationvaluetext"></a><span data-ttu-id="b67b8-103">Atualizar groupPolicyPresentationValueText</span><span class="sxs-lookup"><span data-stu-id="b67b8-103">Update groupPolicyPresentationValueText</span></span>

<span data-ttu-id="b67b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b67b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b67b8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b67b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b67b8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b67b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b67b8-107">Atualize as propriedades de [um objeto groupPolicyPresentationValueText.](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)</span><span class="sxs-lookup"><span data-stu-id="b67b8-107">Update the properties of a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b67b8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b67b8-108">Prerequisites</span></span>
<span data-ttu-id="b67b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b67b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b67b8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b67b8-111">Permission type</span></span>|<span data-ttu-id="b67b8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b67b8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b67b8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b67b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b67b8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b67b8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b67b8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b67b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b67b8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b67b8-116">Not supported.</span></span>|
|<span data-ttu-id="b67b8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b67b8-117">Application</span></span>|<span data-ttu-id="b67b8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b67b8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b67b8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b67b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="b67b8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b67b8-120">Request headers</span></span>
|<span data-ttu-id="b67b8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b67b8-121">Header</span></span>|<span data-ttu-id="b67b8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b67b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b67b8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b67b8-123">Authorization</span></span>|<span data-ttu-id="b67b8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b67b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b67b8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b67b8-125">Accept</span></span>|<span data-ttu-id="b67b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b67b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b67b8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b67b8-127">Request body</span></span>
<span data-ttu-id="b67b8-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicyPresentationValueText.](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)</span><span class="sxs-lookup"><span data-stu-id="b67b8-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

<span data-ttu-id="b67b8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span><span class="sxs-lookup"><span data-stu-id="b67b8-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span></span>

|<span data-ttu-id="b67b8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b67b8-130">Property</span></span>|<span data-ttu-id="b67b8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b67b8-131">Type</span></span>|<span data-ttu-id="b67b8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b67b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b67b8-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b67b8-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b67b8-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b67b8-134">DateTimeOffset</span></span>|<span data-ttu-id="b67b8-135">A data e a hora em que o objeto foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b67b8-135">The date and time the object was last modified.</span></span> <span data-ttu-id="b67b8-136">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b67b8-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b67b8-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b67b8-137">createdDateTime</span></span>|<span data-ttu-id="b67b8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b67b8-138">DateTimeOffset</span></span>|<span data-ttu-id="b67b8-139">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b67b8-139">The date and time the object was created.</span></span> <span data-ttu-id="b67b8-140">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b67b8-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b67b8-141">id</span><span class="sxs-lookup"><span data-stu-id="b67b8-141">id</span></span>|<span data-ttu-id="b67b8-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b67b8-142">String</span></span>|<span data-ttu-id="b67b8-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b67b8-143">Key of the entity.</span></span> <span data-ttu-id="b67b8-144">Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b67b8-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b67b8-145">value</span><span class="sxs-lookup"><span data-stu-id="b67b8-145">value</span></span>|<span data-ttu-id="b67b8-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b67b8-146">String</span></span>|<span data-ttu-id="b67b8-147">Um valor de cadeia de caracteres para a apresentação associada.</span><span class="sxs-lookup"><span data-stu-id="b67b8-147">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="b67b8-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b67b8-148">Response</span></span>
<span data-ttu-id="b67b8-149">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b67b8-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b67b8-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b67b8-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="b67b8-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b67b8-151">Request</span></span>
<span data-ttu-id="b67b8-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b67b8-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="b67b8-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b67b8-153">Response</span></span>
<span data-ttu-id="b67b8-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b67b8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




