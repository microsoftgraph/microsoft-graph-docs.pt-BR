---
title: Criar iosUpdateConfiguration
description: Cria um novo objeto iosUpdateConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 359f6833cc7705445941d7b85f56f00295df2c30
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408618"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="04b33-103">Criar iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="04b33-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="04b33-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="04b33-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="04b33-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="04b33-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04b33-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="04b33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04b33-107">Cria um novo objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="04b33-107">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04b33-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04b33-108">Prerequisites</span></span>
<span data-ttu-id="04b33-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="04b33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="04b33-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04b33-111">Permission type</span></span>|<span data-ttu-id="04b33-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04b33-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04b33-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04b33-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04b33-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b33-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="04b33-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04b33-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04b33-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04b33-116">Not supported.</span></span>|
|<span data-ttu-id="04b33-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04b33-117">Application</span></span>|<span data-ttu-id="04b33-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04b33-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04b33-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04b33-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="04b33-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04b33-120">Request headers</span></span>
|<span data-ttu-id="04b33-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04b33-121">Header</span></span>|<span data-ttu-id="04b33-122">Valor</span><span class="sxs-lookup"><span data-stu-id="04b33-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04b33-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="04b33-123">Authorization</span></span>|<span data-ttu-id="04b33-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04b33-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04b33-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04b33-125">Accept</span></span>|<span data-ttu-id="04b33-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04b33-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04b33-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04b33-127">Request body</span></span>
<span data-ttu-id="04b33-128">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="04b33-128">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="04b33-129">A tabela a seguir mostra as propriedades obrigatórias ao criar iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="04b33-129">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="04b33-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04b33-130">Property</span></span>|<span data-ttu-id="04b33-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="04b33-131">Type</span></span>|<span data-ttu-id="04b33-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="04b33-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04b33-133">id</span><span class="sxs-lookup"><span data-stu-id="04b33-133">id</span></span>|<span data-ttu-id="04b33-134">String</span><span class="sxs-lookup"><span data-stu-id="04b33-134">String</span></span>|<span data-ttu-id="04b33-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="04b33-135">Key of the entity.</span></span> <span data-ttu-id="04b33-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04b33-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04b33-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04b33-137">lastModifiedDateTime</span></span>|<span data-ttu-id="04b33-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04b33-138">DateTimeOffset</span></span>|<span data-ttu-id="04b33-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="04b33-139">DateTime the object was last modified.</span></span> <span data-ttu-id="04b33-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04b33-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04b33-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="04b33-141">roleScopeTagIds</span></span>|<span data-ttu-id="04b33-142">String collection</span><span class="sxs-lookup"><span data-stu-id="04b33-142">String collection</span></span>|<span data-ttu-id="04b33-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="04b33-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="04b33-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04b33-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04b33-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="04b33-145">supportsScopeTags</span></span>|<span data-ttu-id="04b33-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="04b33-146">Boolean</span></span>|<span data-ttu-id="04b33-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="04b33-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="04b33-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="04b33-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="04b33-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="04b33-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="04b33-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="04b33-150">This property is read-only.</span></span> <span data-ttu-id="04b33-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04b33-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04b33-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04b33-152">createdDateTime</span></span>|<span data-ttu-id="04b33-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04b33-153">DateTimeOffset</span></span>|<span data-ttu-id="04b33-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="04b33-154">DateTime the object was created.</span></span> <span data-ttu-id="04b33-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04b33-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04b33-156">description</span><span class="sxs-lookup"><span data-stu-id="04b33-156">description</span></span>|<span data-ttu-id="04b33-157">String</span><span class="sxs-lookup"><span data-stu-id="04b33-157">String</span></span>|<span data-ttu-id="04b33-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04b33-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="04b33-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04b33-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04b33-160">displayName</span><span class="sxs-lookup"><span data-stu-id="04b33-160">displayName</span></span>|<span data-ttu-id="04b33-161">String</span><span class="sxs-lookup"><span data-stu-id="04b33-161">String</span></span>|<span data-ttu-id="04b33-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04b33-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="04b33-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04b33-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04b33-164">version</span><span class="sxs-lookup"><span data-stu-id="04b33-164">version</span></span>|<span data-ttu-id="04b33-165">Int32</span><span class="sxs-lookup"><span data-stu-id="04b33-165">Int32</span></span>|<span data-ttu-id="04b33-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04b33-166">Version of the device configuration.</span></span> <span data-ttu-id="04b33-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04b33-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04b33-168">isEnabled</span><span class="sxs-lookup"><span data-stu-id="04b33-168">isEnabled</span></span>|<span data-ttu-id="04b33-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="04b33-169">Boolean</span></span>|<span data-ttu-id="04b33-170">Configuração estiver habilitada na interface do usuário</span><span class="sxs-lookup"><span data-stu-id="04b33-170">Is setting enabled in UI</span></span>|
|<span data-ttu-id="04b33-171">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="04b33-171">activeHoursStart</span></span>|<span data-ttu-id="04b33-172">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="04b33-172">TimeOfDay</span></span>|<span data-ttu-id="04b33-173">Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="04b33-173">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="04b33-174">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="04b33-174">activeHoursEnd</span></span>|<span data-ttu-id="04b33-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="04b33-175">TimeOfDay</span></span>|<span data-ttu-id="04b33-176">Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="04b33-176">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="04b33-177">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="04b33-177">scheduledInstallDays</span></span>|<span data-ttu-id="04b33-178">coleção [dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="04b33-178">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="04b33-179">Dias na semana para os quais o horário ativo está configurado.</span><span class="sxs-lookup"><span data-stu-id="04b33-179">Days in week for which active hours are configured.</span></span> <span data-ttu-id="04b33-180">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="04b33-180">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="04b33-181">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="04b33-181">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="04b33-182">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="04b33-182">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="04b33-183">Int32</span><span class="sxs-lookup"><span data-stu-id="04b33-183">Int32</span></span>|<span data-ttu-id="04b33-184">Deslocamento do horário UTC indicado em minutos</span><span class="sxs-lookup"><span data-stu-id="04b33-184">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="04b33-185">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="04b33-185">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="04b33-186">Int32</span><span class="sxs-lookup"><span data-stu-id="04b33-186">Int32</span></span>|<span data-ttu-id="04b33-187">Dias antes de atualizações de software estão visíveis para os dispositivos iOS que varia de 0 a 90 inclusive</span><span class="sxs-lookup"><span data-stu-id="04b33-187">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="04b33-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="04b33-188">Response</span></span>
<span data-ttu-id="04b33-189">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04b33-189">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04b33-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04b33-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="04b33-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04b33-191">Request</span></span>
<span data-ttu-id="04b33-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04b33-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04b33-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="04b33-193">Response</span></span>
<span data-ttu-id="04b33-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04b33-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




