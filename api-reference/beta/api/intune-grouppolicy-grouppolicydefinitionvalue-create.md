---
title: Criar groupPolicyDefinitionValue
description: Criar um novo objeto groupPolicyDefinitionValue.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0ca08cc47517d16103b3133dfe8aa5e16838fec4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465041"
---
# <a name="create-grouppolicydefinitionvalue"></a><span data-ttu-id="304c0-103">Criar groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="304c0-103">Create groupPolicyDefinitionValue</span></span>

<span data-ttu-id="304c0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="304c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="304c0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="304c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="304c0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="304c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="304c0-107">Criar um novo objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="304c0-107">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="304c0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="304c0-108">Prerequisites</span></span>
<span data-ttu-id="304c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="304c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="304c0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="304c0-111">Permission type</span></span>|<span data-ttu-id="304c0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="304c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="304c0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="304c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="304c0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="304c0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="304c0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="304c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="304c0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="304c0-116">Not supported.</span></span>|
|<span data-ttu-id="304c0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="304c0-117">Application</span></span>|<span data-ttu-id="304c0-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="304c0-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="304c0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="304c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## <a name="request-headers"></a><span data-ttu-id="304c0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="304c0-120">Request headers</span></span>
|<span data-ttu-id="304c0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="304c0-121">Header</span></span>|<span data-ttu-id="304c0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="304c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="304c0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="304c0-123">Authorization</span></span>|<span data-ttu-id="304c0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="304c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="304c0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="304c0-125">Accept</span></span>|<span data-ttu-id="304c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="304c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="304c0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="304c0-127">Request body</span></span>
<span data-ttu-id="304c0-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyDefinitionValue.</span><span class="sxs-lookup"><span data-stu-id="304c0-128">In the request body, supply a JSON representation for the groupPolicyDefinitionValue object.</span></span>

<span data-ttu-id="304c0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyDefinitionValue.</span><span class="sxs-lookup"><span data-stu-id="304c0-129">The following table shows the properties that are required when you create the groupPolicyDefinitionValue.</span></span>

|<span data-ttu-id="304c0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="304c0-130">Property</span></span>|<span data-ttu-id="304c0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="304c0-131">Type</span></span>|<span data-ttu-id="304c0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="304c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="304c0-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="304c0-133">createdDateTime</span></span>|<span data-ttu-id="304c0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="304c0-134">DateTimeOffset</span></span>|<span data-ttu-id="304c0-135">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="304c0-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="304c0-136">enabled</span><span class="sxs-lookup"><span data-stu-id="304c0-136">enabled</span></span>|<span data-ttu-id="304c0-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="304c0-137">Boolean</span></span>|<span data-ttu-id="304c0-138">Habilita ou desabilita a definição de política de grupo associada.</span><span class="sxs-lookup"><span data-stu-id="304c0-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="304c0-139">ConfigurationType</span><span class="sxs-lookup"><span data-stu-id="304c0-139">configurationType</span></span>|[<span data-ttu-id="304c0-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="304c0-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="304c0-141">Especifica como o valor deve ser configurado.</span><span class="sxs-lookup"><span data-stu-id="304c0-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="304c0-142">Isso pode ser uma política ou uma preferência.</span><span class="sxs-lookup"><span data-stu-id="304c0-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="304c0-143">Os valores possíveis são: `policy` e `preference`.</span><span class="sxs-lookup"><span data-stu-id="304c0-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="304c0-144">id</span><span class="sxs-lookup"><span data-stu-id="304c0-144">id</span></span>|<span data-ttu-id="304c0-145">String</span><span class="sxs-lookup"><span data-stu-id="304c0-145">String</span></span>|<span data-ttu-id="304c0-146">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="304c0-146">Key of the entity.</span></span>|
|<span data-ttu-id="304c0-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="304c0-147">lastModifiedDateTime</span></span>|<span data-ttu-id="304c0-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="304c0-148">DateTimeOffset</span></span>|<span data-ttu-id="304c0-149">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="304c0-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="304c0-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="304c0-150">Response</span></span>
<span data-ttu-id="304c0-151">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="304c0-151">If successful, this method returns a `201 Created` response code and a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="304c0-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="304c0-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="304c0-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="304c0-153">Request</span></span>
<span data-ttu-id="304c0-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="304c0-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="304c0-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="304c0-155">Response</span></span>
<span data-ttu-id="304c0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="304c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





