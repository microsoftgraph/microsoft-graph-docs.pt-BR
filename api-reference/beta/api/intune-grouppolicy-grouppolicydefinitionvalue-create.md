---
title: Criar groupPolicyDefinitionValue
description: Criar um novo objeto groupPolicyDefinitionValue.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6a09cb39fdd0a479af494ba105abc9505426e60c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49285861"
---
# <a name="create-grouppolicydefinitionvalue"></a><span data-ttu-id="fcb04-103">Criar groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="fcb04-103">Create groupPolicyDefinitionValue</span></span>

<span data-ttu-id="fcb04-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcb04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcb04-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fcb04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcb04-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fcb04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcb04-107">Criar um novo objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="fcb04-107">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcb04-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fcb04-108">Prerequisites</span></span>
<span data-ttu-id="fcb04-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcb04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcb04-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcb04-111">Permission type</span></span>|<span data-ttu-id="fcb04-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fcb04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcb04-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcb04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fcb04-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcb04-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fcb04-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcb04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcb04-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcb04-116">Not supported.</span></span>|
|<span data-ttu-id="fcb04-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcb04-117">Application</span></span>|<span data-ttu-id="fcb04-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcb04-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcb04-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcb04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## <a name="request-headers"></a><span data-ttu-id="fcb04-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcb04-120">Request headers</span></span>
|<span data-ttu-id="fcb04-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fcb04-121">Header</span></span>|<span data-ttu-id="fcb04-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fcb04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcb04-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcb04-123">Authorization</span></span>|<span data-ttu-id="fcb04-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcb04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcb04-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fcb04-125">Accept</span></span>|<span data-ttu-id="fcb04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fcb04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcb04-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcb04-127">Request body</span></span>
<span data-ttu-id="fcb04-128">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyDefinitionValue.</span><span class="sxs-lookup"><span data-stu-id="fcb04-128">In the request body, supply a JSON representation for the groupPolicyDefinitionValue object.</span></span>

<span data-ttu-id="fcb04-129">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyDefinitionValue.</span><span class="sxs-lookup"><span data-stu-id="fcb04-129">The following table shows the properties that are required when you create the groupPolicyDefinitionValue.</span></span>

|<span data-ttu-id="fcb04-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fcb04-130">Property</span></span>|<span data-ttu-id="fcb04-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcb04-131">Type</span></span>|<span data-ttu-id="fcb04-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcb04-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcb04-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fcb04-133">createdDateTime</span></span>|<span data-ttu-id="fcb04-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcb04-134">DateTimeOffset</span></span>|<span data-ttu-id="fcb04-135">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="fcb04-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="fcb04-136">enabled</span><span class="sxs-lookup"><span data-stu-id="fcb04-136">enabled</span></span>|<span data-ttu-id="fcb04-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="fcb04-137">Boolean</span></span>|<span data-ttu-id="fcb04-138">Habilita ou desabilita a definição de política de grupo associada.</span><span class="sxs-lookup"><span data-stu-id="fcb04-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="fcb04-139">ConfigurationType</span><span class="sxs-lookup"><span data-stu-id="fcb04-139">configurationType</span></span>|[<span data-ttu-id="fcb04-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="fcb04-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="fcb04-141">Especifica como o valor deve ser configurado.</span><span class="sxs-lookup"><span data-stu-id="fcb04-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="fcb04-142">Isso pode ser uma política ou uma preferência.</span><span class="sxs-lookup"><span data-stu-id="fcb04-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="fcb04-143">Os valores possíveis são: `policy` e `preference`.</span><span class="sxs-lookup"><span data-stu-id="fcb04-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="fcb04-144">id</span><span class="sxs-lookup"><span data-stu-id="fcb04-144">id</span></span>|<span data-ttu-id="fcb04-145">String</span><span class="sxs-lookup"><span data-stu-id="fcb04-145">String</span></span>|<span data-ttu-id="fcb04-146">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fcb04-146">Key of the entity.</span></span>|
|<span data-ttu-id="fcb04-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fcb04-147">lastModifiedDateTime</span></span>|<span data-ttu-id="fcb04-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcb04-148">DateTimeOffset</span></span>|<span data-ttu-id="fcb04-149">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fcb04-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="fcb04-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcb04-150">Response</span></span>
<span data-ttu-id="fcb04-151">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fcb04-151">If successful, this method returns a `201 Created` response code and a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcb04-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fcb04-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcb04-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcb04-153">Request</span></span>
<span data-ttu-id="fcb04-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcb04-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fcb04-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcb04-155">Response</span></span>
<span data-ttu-id="fcb04-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fcb04-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




