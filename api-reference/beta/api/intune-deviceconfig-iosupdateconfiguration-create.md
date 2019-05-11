---
title: Criar iosUpdateConfiguration
description: Cria um novo objeto iosUpdateConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b650c64e1c5c90462f4a513e77d43cdc0424a7ce
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923306"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="7d468-103">Criar iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="7d468-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="7d468-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7d468-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d468-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d468-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d468-106">Cria um novo objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d468-106">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d468-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d468-107">Prerequisites</span></span>
<span data-ttu-id="7d468-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d468-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d468-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d468-110">Permission type</span></span>|<span data-ttu-id="7d468-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d468-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d468-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d468-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d468-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d468-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d468-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d468-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d468-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d468-115">Not supported.</span></span>|
|<span data-ttu-id="7d468-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d468-116">Application</span></span>|<span data-ttu-id="7d468-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d468-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d468-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d468-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7d468-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d468-119">Request headers</span></span>
|<span data-ttu-id="7d468-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d468-120">Header</span></span>|<span data-ttu-id="7d468-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7d468-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d468-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d468-122">Authorization</span></span>|<span data-ttu-id="7d468-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d468-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d468-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d468-124">Accept</span></span>|<span data-ttu-id="7d468-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7d468-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d468-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d468-126">Request body</span></span>
<span data-ttu-id="7d468-127">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7d468-127">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="7d468-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7d468-128">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="7d468-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d468-129">Property</span></span>|<span data-ttu-id="7d468-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d468-130">Type</span></span>|<span data-ttu-id="7d468-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d468-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d468-132">id</span><span class="sxs-lookup"><span data-stu-id="7d468-132">id</span></span>|<span data-ttu-id="7d468-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d468-133">String</span></span>|<span data-ttu-id="7d468-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7d468-134">Key of the entity.</span></span> <span data-ttu-id="7d468-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d468-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d468-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d468-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7d468-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d468-137">DateTimeOffset</span></span>|<span data-ttu-id="7d468-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7d468-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7d468-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d468-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d468-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7d468-140">roleScopeTagIds</span></span>|<span data-ttu-id="7d468-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d468-141">String collection</span></span>|<span data-ttu-id="7d468-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="7d468-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7d468-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d468-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d468-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7d468-144">supportsScopeTags</span></span>|<span data-ttu-id="7d468-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d468-145">Boolean</span></span>|<span data-ttu-id="7d468-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="7d468-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7d468-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="7d468-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7d468-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="7d468-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7d468-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d468-149">This property is read-only.</span></span> <span data-ttu-id="7d468-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d468-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d468-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d468-151">createdDateTime</span></span>|<span data-ttu-id="7d468-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d468-152">DateTimeOffset</span></span>|<span data-ttu-id="7d468-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7d468-153">DateTime the object was created.</span></span> <span data-ttu-id="7d468-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d468-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d468-155">description</span><span class="sxs-lookup"><span data-stu-id="7d468-155">description</span></span>|<span data-ttu-id="7d468-156">String</span><span class="sxs-lookup"><span data-stu-id="7d468-156">String</span></span>|<span data-ttu-id="7d468-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d468-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7d468-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d468-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d468-159">displayName</span><span class="sxs-lookup"><span data-stu-id="7d468-159">displayName</span></span>|<span data-ttu-id="7d468-160">String</span><span class="sxs-lookup"><span data-stu-id="7d468-160">String</span></span>|<span data-ttu-id="7d468-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d468-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7d468-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d468-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d468-163">versão</span><span class="sxs-lookup"><span data-stu-id="7d468-163">version</span></span>|<span data-ttu-id="7d468-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7d468-164">Int32</span></span>|<span data-ttu-id="7d468-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d468-165">Version of the device configuration.</span></span> <span data-ttu-id="7d468-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d468-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d468-167">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7d468-167">isEnabled</span></span>|<span data-ttu-id="7d468-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d468-168">Boolean</span></span>|<span data-ttu-id="7d468-169">A configuração está habilitada na IU</span><span class="sxs-lookup"><span data-stu-id="7d468-169">Is setting enabled in UI</span></span>|
|<span data-ttu-id="7d468-170">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="7d468-170">activeHoursStart</span></span>|<span data-ttu-id="7d468-171">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7d468-171">TimeOfDay</span></span>|<span data-ttu-id="7d468-172">Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="7d468-172">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="7d468-173">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="7d468-173">activeHoursEnd</span></span>|<span data-ttu-id="7d468-174">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7d468-174">TimeOfDay</span></span>|<span data-ttu-id="7d468-175">Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="7d468-175">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="7d468-176">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="7d468-176">scheduledInstallDays</span></span>|<span data-ttu-id="7d468-177">coleção [DayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="7d468-177">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="7d468-178">Dias na semana para os quais o horário ativo está configurado.</span><span class="sxs-lookup"><span data-stu-id="7d468-178">Days in week for which active hours are configured.</span></span> <span data-ttu-id="7d468-179">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="7d468-179">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="7d468-180">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="7d468-180">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="7d468-181">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="7d468-181">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="7d468-182">Int32</span><span class="sxs-lookup"><span data-stu-id="7d468-182">Int32</span></span>|<span data-ttu-id="7d468-183">Deslocamento do horário UTC indicado em minutos</span><span class="sxs-lookup"><span data-stu-id="7d468-183">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="7d468-184">Propriedadeenforcedsoftwareupdatedelayindays</span><span class="sxs-lookup"><span data-stu-id="7d468-184">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="7d468-185">Int32</span><span class="sxs-lookup"><span data-stu-id="7d468-185">Int32</span></span>|<span data-ttu-id="7d468-186">Dias antes que as atualizações de software fiquem visíveis para dispositivos iOS variando de 0 a 90, inclusive</span><span class="sxs-lookup"><span data-stu-id="7d468-186">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="7d468-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d468-187">Response</span></span>
<span data-ttu-id="7d468-188">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d468-188">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d468-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d468-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d468-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d468-190">Request</span></span>
<span data-ttu-id="7d468-191">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d468-191">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 482

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```

### <a name="response"></a><span data-ttu-id="7d468-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d468-192">Response</span></span>
<span data-ttu-id="7d468-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d468-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 654

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```




