---
title: Atualizar androidOmaCpConfiguration
description: Atualiza as propriedades de um objeto androidOmaCpConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f8b7bba614056e97081b8a7997a9fbae4e83e74
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32475932"
---
# <a name="update-androidomacpconfiguration"></a><span data-ttu-id="bb419-103">Atualizar androidOmaCpConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb419-103">Update androidOmaCpConfiguration</span></span>

> <span data-ttu-id="bb419-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb419-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb419-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb419-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb419-106">Atualiza as propriedades de um objeto [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bb419-106">Update the properties of a [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb419-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb419-107">Prerequisites</span></span>
<span data-ttu-id="bb419-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb419-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb419-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb419-110">Permission type</span></span>|<span data-ttu-id="bb419-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb419-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb419-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb419-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb419-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb419-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb419-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb419-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb419-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb419-115">Not supported.</span></span>|
|<span data-ttu-id="bb419-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb419-116">Application</span></span>|<span data-ttu-id="bb419-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb419-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb419-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb419-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bb419-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb419-119">Request headers</span></span>
|<span data-ttu-id="bb419-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb419-120">Header</span></span>|<span data-ttu-id="bb419-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bb419-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb419-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb419-122">Authorization</span></span>|<span data-ttu-id="bb419-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb419-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb419-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb419-124">Accept</span></span>|<span data-ttu-id="bb419-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb419-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb419-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb419-126">Request body</span></span>
<span data-ttu-id="bb419-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bb419-127">In the request body, supply a JSON representation for the [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

<span data-ttu-id="bb419-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb419-128">The following table shows the properties that are required when you create the [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md).</span></span>

|<span data-ttu-id="bb419-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb419-129">Property</span></span>|<span data-ttu-id="bb419-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb419-130">Type</span></span>|<span data-ttu-id="bb419-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb419-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb419-132">id</span><span class="sxs-lookup"><span data-stu-id="bb419-132">id</span></span>|<span data-ttu-id="bb419-133">String</span><span class="sxs-lookup"><span data-stu-id="bb419-133">String</span></span>|<span data-ttu-id="bb419-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bb419-134">Key of the entity.</span></span> <span data-ttu-id="bb419-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb419-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb419-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb419-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bb419-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb419-137">DateTimeOffset</span></span>|<span data-ttu-id="bb419-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="bb419-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bb419-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb419-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb419-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bb419-140">roleScopeTagIds</span></span>|<span data-ttu-id="bb419-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb419-141">String collection</span></span>|<span data-ttu-id="bb419-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="bb419-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bb419-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb419-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb419-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bb419-144">supportsScopeTags</span></span>|<span data-ttu-id="bb419-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb419-145">Boolean</span></span>|<span data-ttu-id="bb419-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="bb419-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bb419-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="bb419-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bb419-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="bb419-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bb419-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb419-149">This property is read-only.</span></span> <span data-ttu-id="bb419-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb419-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb419-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb419-151">createdDateTime</span></span>|<span data-ttu-id="bb419-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb419-152">DateTimeOffset</span></span>|<span data-ttu-id="bb419-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bb419-153">DateTime the object was created.</span></span> <span data-ttu-id="bb419-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb419-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb419-155">description</span><span class="sxs-lookup"><span data-stu-id="bb419-155">description</span></span>|<span data-ttu-id="bb419-156">String</span><span class="sxs-lookup"><span data-stu-id="bb419-156">String</span></span>|<span data-ttu-id="bb419-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb419-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bb419-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb419-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb419-159">displayName</span><span class="sxs-lookup"><span data-stu-id="bb419-159">displayName</span></span>|<span data-ttu-id="bb419-160">String</span><span class="sxs-lookup"><span data-stu-id="bb419-160">String</span></span>|<span data-ttu-id="bb419-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb419-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bb419-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb419-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb419-163">versão</span><span class="sxs-lookup"><span data-stu-id="bb419-163">version</span></span>|<span data-ttu-id="bb419-164">Int32</span><span class="sxs-lookup"><span data-stu-id="bb419-164">Int32</span></span>|<span data-ttu-id="bb419-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb419-165">Version of the device configuration.</span></span> <span data-ttu-id="bb419-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb419-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb419-167">configurationXml</span><span class="sxs-lookup"><span data-stu-id="bb419-167">configurationXml</span></span>|<span data-ttu-id="bb419-168">Binary</span><span class="sxs-lookup"><span data-stu-id="bb419-168">Binary</span></span>|<span data-ttu-id="bb419-169">XML de configuração que será aplicada ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb419-169">Configuration XML that will be applied to the device.</span></span> <span data-ttu-id="bb419-170">Quando ele é lido, ele só fornece uma cadeia de caracteres de espaço reservado, pois os dados originais são criptografados e armazenados.</span><span class="sxs-lookup"><span data-stu-id="bb419-170">When it is read, it only provides a placeholder string since the original data is encrypted and stored.</span></span>|



## <a name="response"></a><span data-ttu-id="bb419-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb419-171">Response</span></span>
<span data-ttu-id="bb419-172">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb419-172">If successful, this method returns a `200 OK` response code and an updated [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb419-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb419-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb419-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb419-174">Request</span></span>
<span data-ttu-id="bb419-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb419-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="bb419-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb419-176">Response</span></span>
<span data-ttu-id="bb419-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb419-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "id": "5f682e4a-2e4a-5f68-4a2e-685f4a2e685f",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```





