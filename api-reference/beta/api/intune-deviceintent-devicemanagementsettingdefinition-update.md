---
title: Atualizar deviceManagementSettingDefinition
description: Atualiza as propriedades de um objeto deviceManagementSettingDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d349fd80a65020e03b691305bb2e968ec5407db5
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522570"
---
# <a name="update-devicemanagementsettingdefinition"></a><span data-ttu-id="439d5-103">Atualizar deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="439d5-103">Update deviceManagementSettingDefinition</span></span>

> <span data-ttu-id="439d5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="439d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="439d5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="439d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="439d5-106">Atualiza as propriedades de um objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="439d5-106">Update the properties of a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="439d5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="439d5-107">Prerequisites</span></span>
<span data-ttu-id="439d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="439d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="439d5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="439d5-110">Permission type</span></span>|<span data-ttu-id="439d5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="439d5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="439d5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="439d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="439d5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="439d5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="439d5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="439d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="439d5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="439d5-115">Not supported.</span></span>|
|<span data-ttu-id="439d5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="439d5-116">Application</span></span>|<span data-ttu-id="439d5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="439d5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="439d5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="439d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="439d5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="439d5-119">Request headers</span></span>
|<span data-ttu-id="439d5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="439d5-120">Header</span></span>|<span data-ttu-id="439d5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="439d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="439d5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="439d5-122">Authorization</span></span>|<span data-ttu-id="439d5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="439d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="439d5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="439d5-124">Accept</span></span>|<span data-ttu-id="439d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="439d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="439d5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="439d5-126">Request body</span></span>
<span data-ttu-id="439d5-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="439d5-127">In the request body, supply a JSON representation for the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

<span data-ttu-id="439d5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="439d5-128">The following table shows the properties that are required when you create the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span>

|<span data-ttu-id="439d5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="439d5-129">Property</span></span>|<span data-ttu-id="439d5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="439d5-130">Type</span></span>|<span data-ttu-id="439d5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="439d5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="439d5-132">id</span><span class="sxs-lookup"><span data-stu-id="439d5-132">id</span></span>|<span data-ttu-id="439d5-133">String</span><span class="sxs-lookup"><span data-stu-id="439d5-133">String</span></span>|<span data-ttu-id="439d5-134">A ID da definição de configuração</span><span class="sxs-lookup"><span data-stu-id="439d5-134">The ID of the setting definition</span></span>|
|<span data-ttu-id="439d5-135">valueType</span><span class="sxs-lookup"><span data-stu-id="439d5-135">valueType</span></span>|[<span data-ttu-id="439d5-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="439d5-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="439d5-137">O tipo de dados do valor.</span><span class="sxs-lookup"><span data-stu-id="439d5-137">The data type of the value.</span></span> <span data-ttu-id="439d5-138">Os valores possíveis são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="439d5-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="439d5-139">displayName</span><span class="sxs-lookup"><span data-stu-id="439d5-139">displayName</span></span>|<span data-ttu-id="439d5-140">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="439d5-140">String</span></span>|<span data-ttu-id="439d5-141">O nome de exibição da configuração</span><span class="sxs-lookup"><span data-stu-id="439d5-141">The setting's display name</span></span>|
|<span data-ttu-id="439d5-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="439d5-142">isTopLevel</span></span>|<span data-ttu-id="439d5-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="439d5-143">Boolean</span></span>|<span data-ttu-id="439d5-144">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa</span><span class="sxs-lookup"><span data-stu-id="439d5-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="439d5-145">description</span><span class="sxs-lookup"><span data-stu-id="439d5-145">description</span></span>|<span data-ttu-id="439d5-146">String</span><span class="sxs-lookup"><span data-stu-id="439d5-146">String</span></span>|<span data-ttu-id="439d5-147">A descrição da configuração</span><span class="sxs-lookup"><span data-stu-id="439d5-147">The setting's description</span></span>|
|<span data-ttu-id="439d5-148">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="439d5-148">documentationUrl</span></span>|<span data-ttu-id="439d5-149">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="439d5-149">String</span></span>|<span data-ttu-id="439d5-150">URL para configurar a documentação</span><span class="sxs-lookup"><span data-stu-id="439d5-150">Url to setting documentation</span></span>|
|<span data-ttu-id="439d5-151">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="439d5-151">keywords</span></span>|<span data-ttu-id="439d5-152">Coleção String</span><span class="sxs-lookup"><span data-stu-id="439d5-152">String collection</span></span>|<span data-ttu-id="439d5-153">Palavras-chave associadas à configuração</span><span class="sxs-lookup"><span data-stu-id="439d5-153">Keywords associated with the setting</span></span>|
|<span data-ttu-id="439d5-154">as</span><span class="sxs-lookup"><span data-stu-id="439d5-154">constraints</span></span>|<span data-ttu-id="439d5-155">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="439d5-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="439d5-156">Conjunto de restrições para o valor de configuração</span><span class="sxs-lookup"><span data-stu-id="439d5-156">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="439d5-157">relação</span><span class="sxs-lookup"><span data-stu-id="439d5-157">dependencies</span></span>|<span data-ttu-id="439d5-158">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="439d5-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="439d5-159">Coleção de dependências em outras configurações</span><span class="sxs-lookup"><span data-stu-id="439d5-159">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="439d5-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="439d5-160">Response</span></span>
<span data-ttu-id="439d5-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="439d5-161">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="439d5-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="439d5-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="439d5-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="439d5-163">Request</span></span>
<span data-ttu-id="439d5-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="439d5-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 728

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="439d5-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="439d5-165">Response</span></span>
<span data-ttu-id="439d5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="439d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 777

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ]
}
```







