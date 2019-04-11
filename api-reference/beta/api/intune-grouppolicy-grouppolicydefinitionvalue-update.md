---
title: Atualizar groupPolicyDefinitionValue
description: Atualiza as propriedades de um objeto groupPolicyDefinitionValue.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5780357ef7e6720d01d043ae7b7aecc89195f0bb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807144"
---
# <a name="update-grouppolicydefinitionvalue"></a><span data-ttu-id="0cc82-103">Atualizar groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="0cc82-103">Update groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="0cc82-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0cc82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cc82-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0cc82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cc82-106">Atualiza as propriedades de um objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="0cc82-106">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cc82-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0cc82-107">Prerequisites</span></span>
<span data-ttu-id="0cc82-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cc82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cc82-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cc82-110">Permission type</span></span>|<span data-ttu-id="0cc82-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0cc82-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cc82-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cc82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0cc82-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cc82-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0cc82-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cc82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cc82-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cc82-115">Not supported.</span></span>|
|<span data-ttu-id="0cc82-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cc82-116">Application</span></span>|<span data-ttu-id="0cc82-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cc82-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cc82-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cc82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="0cc82-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cc82-119">Request headers</span></span>
|<span data-ttu-id="0cc82-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0cc82-120">Header</span></span>|<span data-ttu-id="0cc82-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0cc82-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cc82-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cc82-122">Authorization</span></span>|<span data-ttu-id="0cc82-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cc82-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cc82-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0cc82-124">Accept</span></span>|<span data-ttu-id="0cc82-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0cc82-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cc82-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cc82-126">Request body</span></span>
<span data-ttu-id="0cc82-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="0cc82-127">In the request body, supply a JSON representation for the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

<span data-ttu-id="0cc82-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span><span class="sxs-lookup"><span data-stu-id="0cc82-128">The following table shows the properties that are required when you create the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

|<span data-ttu-id="0cc82-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cc82-129">Property</span></span>|<span data-ttu-id="0cc82-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cc82-130">Type</span></span>|<span data-ttu-id="0cc82-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cc82-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cc82-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0cc82-132">createdDateTime</span></span>|<span data-ttu-id="0cc82-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cc82-133">DateTimeOffset</span></span>|<span data-ttu-id="0cc82-134">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0cc82-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="0cc82-135">enabled</span><span class="sxs-lookup"><span data-stu-id="0cc82-135">enabled</span></span>|<span data-ttu-id="0cc82-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cc82-136">Boolean</span></span>|<span data-ttu-id="0cc82-137">Habilita ou desabilita a definição de política de grupo associada.</span><span class="sxs-lookup"><span data-stu-id="0cc82-137">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="0cc82-138">ConfigurationType</span><span class="sxs-lookup"><span data-stu-id="0cc82-138">configurationType</span></span>|[<span data-ttu-id="0cc82-139">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="0cc82-139">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="0cc82-140">Especifica como o valor deve ser configurado.</span><span class="sxs-lookup"><span data-stu-id="0cc82-140">Specifies how the value should be configured.</span></span> <span data-ttu-id="0cc82-141">Isso pode ser uma política ou uma preferência.</span><span class="sxs-lookup"><span data-stu-id="0cc82-141">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="0cc82-142">Os valores possíveis são: `policy` e `preference`.</span><span class="sxs-lookup"><span data-stu-id="0cc82-142">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="0cc82-143">id</span><span class="sxs-lookup"><span data-stu-id="0cc82-143">id</span></span>|<span data-ttu-id="0cc82-144">String</span><span class="sxs-lookup"><span data-stu-id="0cc82-144">String</span></span>|<span data-ttu-id="0cc82-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0cc82-145">Key of the entity.</span></span>|
|<span data-ttu-id="0cc82-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0cc82-146">lastModifiedDateTime</span></span>|<span data-ttu-id="0cc82-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cc82-147">DateTimeOffset</span></span>|<span data-ttu-id="0cc82-148">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0cc82-148">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="0cc82-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cc82-149">Response</span></span>
<span data-ttu-id="0cc82-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cc82-150">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cc82-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cc82-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cc82-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cc82-152">Request</span></span>
<span data-ttu-id="0cc82-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cc82-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="0cc82-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cc82-154">Response</span></span>
<span data-ttu-id="0cc82-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0cc82-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "enabled": true,
  "configurationType": "preference",
  "id": "50428918-8918-5042-1889-425018894250",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





