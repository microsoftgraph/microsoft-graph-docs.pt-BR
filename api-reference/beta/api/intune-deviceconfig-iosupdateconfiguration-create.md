---
title: Criar iosUpdateConfiguration
description: Cria um novo objeto iosUpdateConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d64989550b95a5c255924616dce599bf7913b68
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171292"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="0192e-103">Criar iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="0192e-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="0192e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0192e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0192e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0192e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0192e-106">Cria um novo objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0192e-106">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0192e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0192e-107">Prerequisites</span></span>
<span data-ttu-id="0192e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0192e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0192e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0192e-110">Permission type</span></span>|<span data-ttu-id="0192e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0192e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0192e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0192e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0192e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0192e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0192e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0192e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0192e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0192e-115">Not supported.</span></span>|
|<span data-ttu-id="0192e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0192e-116">Application</span></span>|<span data-ttu-id="0192e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0192e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0192e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0192e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0192e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0192e-119">Request headers</span></span>
|<span data-ttu-id="0192e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0192e-120">Header</span></span>|<span data-ttu-id="0192e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0192e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0192e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0192e-122">Authorization</span></span>|<span data-ttu-id="0192e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0192e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0192e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0192e-124">Accept</span></span>|<span data-ttu-id="0192e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0192e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0192e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0192e-126">Request body</span></span>
<span data-ttu-id="0192e-127">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0192e-127">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="0192e-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0192e-128">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="0192e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0192e-129">Property</span></span>|<span data-ttu-id="0192e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0192e-130">Type</span></span>|<span data-ttu-id="0192e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0192e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0192e-132">id</span><span class="sxs-lookup"><span data-stu-id="0192e-132">id</span></span>|<span data-ttu-id="0192e-133">String</span><span class="sxs-lookup"><span data-stu-id="0192e-133">String</span></span>|<span data-ttu-id="0192e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0192e-134">Key of the entity.</span></span> <span data-ttu-id="0192e-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0192e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0192e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0192e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0192e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0192e-137">DateTimeOffset</span></span>|<span data-ttu-id="0192e-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0192e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0192e-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0192e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0192e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0192e-140">roleScopeTagIds</span></span>|<span data-ttu-id="0192e-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0192e-141">String collection</span></span>|<span data-ttu-id="0192e-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0192e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0192e-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0192e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0192e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0192e-144">supportsScopeTags</span></span>|<span data-ttu-id="0192e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0192e-145">Boolean</span></span>|<span data-ttu-id="0192e-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0192e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0192e-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0192e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0192e-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0192e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0192e-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0192e-149">This property is read-only.</span></span> <span data-ttu-id="0192e-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0192e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0192e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0192e-151">createdDateTime</span></span>|<span data-ttu-id="0192e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0192e-152">DateTimeOffset</span></span>|<span data-ttu-id="0192e-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0192e-153">DateTime the object was created.</span></span> <span data-ttu-id="0192e-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0192e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0192e-155">description</span><span class="sxs-lookup"><span data-stu-id="0192e-155">description</span></span>|<span data-ttu-id="0192e-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0192e-156">String</span></span>|<span data-ttu-id="0192e-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0192e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0192e-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0192e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0192e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0192e-159">displayName</span></span>|<span data-ttu-id="0192e-160">String</span><span class="sxs-lookup"><span data-stu-id="0192e-160">String</span></span>|<span data-ttu-id="0192e-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0192e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0192e-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0192e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0192e-163">version</span><span class="sxs-lookup"><span data-stu-id="0192e-163">version</span></span>|<span data-ttu-id="0192e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0192e-164">Int32</span></span>|<span data-ttu-id="0192e-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0192e-165">Version of the device configuration.</span></span> <span data-ttu-id="0192e-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0192e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0192e-167">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0192e-167">isEnabled</span></span>|<span data-ttu-id="0192e-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="0192e-168">Boolean</span></span>|<span data-ttu-id="0192e-169">A configuração está habilitada na IU</span><span class="sxs-lookup"><span data-stu-id="0192e-169">Is setting enabled in UI</span></span>|
|<span data-ttu-id="0192e-170">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="0192e-170">activeHoursStart</span></span>|<span data-ttu-id="0192e-171">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0192e-171">TimeOfDay</span></span>|<span data-ttu-id="0192e-172">Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="0192e-172">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="0192e-173">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="0192e-173">activeHoursEnd</span></span>|<span data-ttu-id="0192e-174">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0192e-174">TimeOfDay</span></span>|<span data-ttu-id="0192e-175">Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="0192e-175">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="0192e-176">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="0192e-176">scheduledInstallDays</span></span>|<span data-ttu-id="0192e-177">coleção [DayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="0192e-177">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="0192e-178">Dias na semana para os quais o horário ativo está configurado.</span><span class="sxs-lookup"><span data-stu-id="0192e-178">Days in week for which active hours are configured.</span></span> <span data-ttu-id="0192e-179">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="0192e-179">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="0192e-180">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="0192e-180">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="0192e-181">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="0192e-181">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="0192e-182">Int32</span><span class="sxs-lookup"><span data-stu-id="0192e-182">Int32</span></span>|<span data-ttu-id="0192e-183">Deslocamento do horário UTC indicado em minutos</span><span class="sxs-lookup"><span data-stu-id="0192e-183">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="0192e-184">Propriedadeenforcedsoftwareupdatedelayindays</span><span class="sxs-lookup"><span data-stu-id="0192e-184">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="0192e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="0192e-185">Int32</span></span>|<span data-ttu-id="0192e-186">Dias antes que as atualizações de software fiquem visíveis para dispositivos iOS variando de 0 a 90, inclusive</span><span class="sxs-lookup"><span data-stu-id="0192e-186">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="0192e-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="0192e-187">Response</span></span>
<span data-ttu-id="0192e-188">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0192e-188">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0192e-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0192e-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="0192e-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0192e-190">Request</span></span>
<span data-ttu-id="0192e-191">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0192e-191">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0192e-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="0192e-192">Response</span></span>
<span data-ttu-id="0192e-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0192e-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




