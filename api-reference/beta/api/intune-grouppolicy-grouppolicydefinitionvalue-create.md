---
title: Criar groupPolicyDefinitionValue
description: Criar um novo objeto groupPolicyDefinitionValue.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 38878e072b1ef5d339e6f5ebaed58ac5c9d5220b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943120"
---
# <a name="create-grouppolicydefinitionvalue"></a><span data-ttu-id="f3da7-103">Criar groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="f3da7-103">Create groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="f3da7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3da7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3da7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3da7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3da7-106">Criar um novo objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="f3da7-106">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3da7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f3da7-107">Prerequisites</span></span>
<span data-ttu-id="f3da7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3da7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3da7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3da7-110">Permission type</span></span>|<span data-ttu-id="f3da7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f3da7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3da7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3da7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3da7-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3da7-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f3da7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3da7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3da7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3da7-115">Not supported.</span></span>|
|<span data-ttu-id="f3da7-116">Application</span><span class="sxs-lookup"><span data-stu-id="f3da7-116">Application</span></span>|<span data-ttu-id="f3da7-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3da7-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3da7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3da7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## <a name="request-headers"></a><span data-ttu-id="f3da7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3da7-119">Request headers</span></span>
|<span data-ttu-id="f3da7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3da7-120">Header</span></span>|<span data-ttu-id="f3da7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f3da7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3da7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3da7-122">Authorization</span></span>|<span data-ttu-id="f3da7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3da7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3da7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f3da7-124">Accept</span></span>|<span data-ttu-id="f3da7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3da7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3da7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3da7-126">Request body</span></span>
<span data-ttu-id="f3da7-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyDefinitionValue.</span><span class="sxs-lookup"><span data-stu-id="f3da7-127">In the request body, supply a JSON representation for the groupPolicyDefinitionValue object.</span></span>

<span data-ttu-id="f3da7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyDefinitionValue.</span><span class="sxs-lookup"><span data-stu-id="f3da7-128">The following table shows the properties that are required when you create the groupPolicyDefinitionValue.</span></span>

|<span data-ttu-id="f3da7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3da7-129">Property</span></span>|<span data-ttu-id="f3da7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3da7-130">Type</span></span>|<span data-ttu-id="f3da7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3da7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3da7-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3da7-132">createdDateTime</span></span>|<span data-ttu-id="f3da7-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3da7-133">DateTimeOffset</span></span>|<span data-ttu-id="f3da7-134">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f3da7-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="f3da7-135">enabled</span><span class="sxs-lookup"><span data-stu-id="f3da7-135">enabled</span></span>|<span data-ttu-id="f3da7-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3da7-136">Boolean</span></span>|<span data-ttu-id="f3da7-137">Habilita ou desabilita a definição de política de grupo associada.</span><span class="sxs-lookup"><span data-stu-id="f3da7-137">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="f3da7-138">ConfigurationType</span><span class="sxs-lookup"><span data-stu-id="f3da7-138">configurationType</span></span>|[<span data-ttu-id="f3da7-139">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="f3da7-139">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="f3da7-140">Especifica como o valor deve ser configurado.</span><span class="sxs-lookup"><span data-stu-id="f3da7-140">Specifies how the value should be configured.</span></span> <span data-ttu-id="f3da7-141">Isso pode ser uma política ou uma preferência.</span><span class="sxs-lookup"><span data-stu-id="f3da7-141">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="f3da7-142">Os valores possíveis são: `policy` e `preference`.</span><span class="sxs-lookup"><span data-stu-id="f3da7-142">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="f3da7-143">id</span><span class="sxs-lookup"><span data-stu-id="f3da7-143">id</span></span>|<span data-ttu-id="f3da7-144">String</span><span class="sxs-lookup"><span data-stu-id="f3da7-144">String</span></span>|<span data-ttu-id="f3da7-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f3da7-145">Key of the entity.</span></span>|
|<span data-ttu-id="f3da7-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3da7-146">lastModifiedDateTime</span></span>|<span data-ttu-id="f3da7-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3da7-147">DateTimeOffset</span></span>|<span data-ttu-id="f3da7-148">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f3da7-148">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="f3da7-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3da7-149">Response</span></span>
<span data-ttu-id="f3da7-150">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3da7-150">If successful, this method returns a `201 Created` response code and a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3da7-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3da7-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3da7-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3da7-152">Request</span></span>
<span data-ttu-id="f3da7-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3da7-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f3da7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3da7-154">Response</span></span>
<span data-ttu-id="f3da7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3da7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





