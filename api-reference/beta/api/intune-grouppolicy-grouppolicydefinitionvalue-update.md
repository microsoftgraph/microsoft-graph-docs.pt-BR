---
title: Atualizar groupPolicyDefinitionValue
description: Atualize as propriedades de um objeto groupPolicyDefinitionValue.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb9185810155eace790304a2324ab7bba515cf12
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157489"
---
# <a name="update-grouppolicydefinitionvalue"></a><span data-ttu-id="52df5-103">Atualizar groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="52df5-103">Update groupPolicyDefinitionValue</span></span>

<span data-ttu-id="52df5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52df5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52df5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52df5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52df5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52df5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52df5-107">Atualize as propriedades de [um objeto groupPolicyDefinitionValue.](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="52df5-107">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52df5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52df5-108">Prerequisites</span></span>
<span data-ttu-id="52df5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52df5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52df5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52df5-111">Permission type</span></span>|<span data-ttu-id="52df5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52df5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52df5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52df5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52df5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52df5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="52df5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52df5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52df5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52df5-116">Not supported.</span></span>|
|<span data-ttu-id="52df5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52df5-117">Application</span></span>|<span data-ttu-id="52df5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52df5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52df5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52df5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="52df5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52df5-120">Request headers</span></span>
|<span data-ttu-id="52df5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52df5-121">Header</span></span>|<span data-ttu-id="52df5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="52df5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52df5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="52df5-123">Authorization</span></span>|<span data-ttu-id="52df5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52df5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52df5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52df5-125">Accept</span></span>|<span data-ttu-id="52df5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52df5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52df5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52df5-127">Request body</span></span>
<span data-ttu-id="52df5-128">No corpo da solicitação, fornece uma representação JSON para o [objeto groupPolicyDefinitionValue.](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="52df5-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

<span data-ttu-id="52df5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span><span class="sxs-lookup"><span data-stu-id="52df5-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

|<span data-ttu-id="52df5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52df5-130">Property</span></span>|<span data-ttu-id="52df5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="52df5-131">Type</span></span>|<span data-ttu-id="52df5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="52df5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52df5-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52df5-133">createdDateTime</span></span>|<span data-ttu-id="52df5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52df5-134">DateTimeOffset</span></span>|<span data-ttu-id="52df5-135">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="52df5-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="52df5-136">enabled</span><span class="sxs-lookup"><span data-stu-id="52df5-136">enabled</span></span>|<span data-ttu-id="52df5-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="52df5-137">Boolean</span></span>|<span data-ttu-id="52df5-138">Habilita ou desabilita a definição de política de grupo associada.</span><span class="sxs-lookup"><span data-stu-id="52df5-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="52df5-139">configurationType</span><span class="sxs-lookup"><span data-stu-id="52df5-139">configurationType</span></span>|[<span data-ttu-id="52df5-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="52df5-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="52df5-141">Especifica como o valor deve ser configurado.</span><span class="sxs-lookup"><span data-stu-id="52df5-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="52df5-142">Isso pode ser como uma Política ou como Uma Preferência.</span><span class="sxs-lookup"><span data-stu-id="52df5-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="52df5-143">Os valores possíveis são: `policy` e `preference`.</span><span class="sxs-lookup"><span data-stu-id="52df5-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="52df5-144">id</span><span class="sxs-lookup"><span data-stu-id="52df5-144">id</span></span>|<span data-ttu-id="52df5-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52df5-145">String</span></span>|<span data-ttu-id="52df5-146">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="52df5-146">Key of the entity.</span></span>|
|<span data-ttu-id="52df5-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52df5-147">lastModifiedDateTime</span></span>|<span data-ttu-id="52df5-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52df5-148">DateTimeOffset</span></span>|<span data-ttu-id="52df5-149">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="52df5-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="52df5-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="52df5-150">Response</span></span>
<span data-ttu-id="52df5-151">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52df5-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52df5-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52df5-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="52df5-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52df5-153">Request</span></span>
<span data-ttu-id="52df5-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52df5-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="52df5-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="52df5-155">Response</span></span>
<span data-ttu-id="52df5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52df5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




