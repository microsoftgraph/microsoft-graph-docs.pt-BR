---
title: Atualizar groupPolicyDefinitionValue
description: Atualize as propriedades de um objeto groupPolicyDefinitionValue.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d346a40e5ee8c2cba6f1510cf52d747e85a0b788
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428964"
---
# <a name="update-grouppolicydefinitionvalue"></a><span data-ttu-id="fd209-103">Atualizar groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="fd209-103">Update groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="fd209-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="fd209-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fd209-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fd209-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd209-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="fd209-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd209-107">Atualize as propriedades de um objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="fd209-107">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd209-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd209-108">Prerequisites</span></span>
<span data-ttu-id="fd209-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd209-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fd209-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd209-111">Permission type</span></span>|<span data-ttu-id="fd209-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd209-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd209-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd209-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fd209-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd209-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fd209-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd209-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd209-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd209-116">Not supported.</span></span>|
|<span data-ttu-id="fd209-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd209-117">Application</span></span>|<span data-ttu-id="fd209-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd209-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd209-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd209-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="fd209-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd209-120">Request headers</span></span>
|<span data-ttu-id="fd209-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd209-121">Header</span></span>|<span data-ttu-id="fd209-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fd209-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd209-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd209-123">Authorization</span></span>|<span data-ttu-id="fd209-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd209-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd209-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd209-125">Accept</span></span>|<span data-ttu-id="fd209-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fd209-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd209-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd209-127">Request body</span></span>
<span data-ttu-id="fd209-128">No corpo da solicitação, fornece uma representação JSON para o objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="fd209-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

<span data-ttu-id="fd209-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span><span class="sxs-lookup"><span data-stu-id="fd209-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

|<span data-ttu-id="fd209-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd209-130">Property</span></span>|<span data-ttu-id="fd209-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd209-131">Type</span></span>|<span data-ttu-id="fd209-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd209-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd209-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd209-133">createdDateTime</span></span>|<span data-ttu-id="fd209-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd209-134">DateTimeOffset</span></span>|<span data-ttu-id="fd209-135">A data e hora que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="fd209-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="fd209-136">enabled</span><span class="sxs-lookup"><span data-stu-id="fd209-136">enabled</span></span>|<span data-ttu-id="fd209-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd209-137">Boolean</span></span>|<span data-ttu-id="fd209-138">Habilita ou desabilita a definição de política de grupo associado.</span><span class="sxs-lookup"><span data-stu-id="fd209-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="fd209-139">configurationType</span><span class="sxs-lookup"><span data-stu-id="fd209-139">configurationType</span></span>|[<span data-ttu-id="fd209-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="fd209-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="fd209-141">Especifica como o valor deve ser configurado.</span><span class="sxs-lookup"><span data-stu-id="fd209-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="fd209-142">Isso pode ser como uma política ou como uma preferência.</span><span class="sxs-lookup"><span data-stu-id="fd209-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="fd209-143">Os valores possíveis são: `policy` e `preference`.</span><span class="sxs-lookup"><span data-stu-id="fd209-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="fd209-144">id</span><span class="sxs-lookup"><span data-stu-id="fd209-144">id</span></span>|<span data-ttu-id="fd209-145">String</span><span class="sxs-lookup"><span data-stu-id="fd209-145">String</span></span>|<span data-ttu-id="fd209-146">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fd209-146">Key of the entity.</span></span>|
|<span data-ttu-id="fd209-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd209-147">lastModifiedDateTime</span></span>|<span data-ttu-id="fd209-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd209-148">DateTimeOffset</span></span>|<span data-ttu-id="fd209-149">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fd209-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="fd209-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd209-150">Response</span></span>
<span data-ttu-id="fd209-151">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd209-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd209-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd209-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd209-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd209-153">Request</span></span>
<span data-ttu-id="fd209-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd209-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fd209-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd209-155">Response</span></span>
<span data-ttu-id="fd209-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd209-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




