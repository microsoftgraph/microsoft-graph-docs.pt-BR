---
title: Atualizar windowsPhone81GeneralConfiguration
description: Atualizar as propriedades de um objeto windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f0776dd36301bdb35d73e7e0564d445217e93be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984532"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="3fe15-103">Atualizar windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="3fe15-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="3fe15-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3fe15-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fe15-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3fe15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fe15-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3fe15-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fe15-107">Atualizar as propriedades de um objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3fe15-107">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3fe15-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3fe15-108">Prerequisites</span></span>
<span data-ttu-id="3fe15-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fe15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fe15-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fe15-111">Permission type</span></span>|<span data-ttu-id="3fe15-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3fe15-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fe15-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fe15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3fe15-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fe15-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3fe15-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fe15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fe15-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fe15-116">Not supported.</span></span>|
|<span data-ttu-id="3fe15-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fe15-117">Application</span></span>|<span data-ttu-id="3fe15-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fe15-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fe15-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fe15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3fe15-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fe15-120">Request headers</span></span>
|<span data-ttu-id="3fe15-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3fe15-121">Header</span></span>|<span data-ttu-id="3fe15-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3fe15-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fe15-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fe15-123">Authorization</span></span>|<span data-ttu-id="3fe15-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fe15-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fe15-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3fe15-125">Accept</span></span>|<span data-ttu-id="3fe15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fe15-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fe15-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fe15-127">Request body</span></span>
<span data-ttu-id="3fe15-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3fe15-128">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="3fe15-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3fe15-129">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="3fe15-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fe15-130">Property</span></span>|<span data-ttu-id="3fe15-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fe15-131">Type</span></span>|<span data-ttu-id="3fe15-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fe15-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fe15-133">id</span><span class="sxs-lookup"><span data-stu-id="3fe15-133">id</span></span>|<span data-ttu-id="3fe15-134">String</span><span class="sxs-lookup"><span data-stu-id="3fe15-134">String</span></span>|<span data-ttu-id="3fe15-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3fe15-135">Key of the entity.</span></span> <span data-ttu-id="3fe15-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fe15-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fe15-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3fe15-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3fe15-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fe15-138">DateTimeOffset</span></span>|<span data-ttu-id="3fe15-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3fe15-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3fe15-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fe15-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fe15-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3fe15-141">roleScopeTagIds</span></span>|<span data-ttu-id="3fe15-142">String collection</span><span class="sxs-lookup"><span data-stu-id="3fe15-142">String collection</span></span>|<span data-ttu-id="3fe15-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="3fe15-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3fe15-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fe15-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fe15-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3fe15-145">supportsScopeTags</span></span>|<span data-ttu-id="3fe15-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-146">Boolean</span></span>|<span data-ttu-id="3fe15-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3fe15-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3fe15-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3fe15-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3fe15-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="3fe15-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3fe15-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3fe15-150">This property is read-only.</span></span> <span data-ttu-id="3fe15-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fe15-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fe15-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3fe15-152">createdDateTime</span></span>|<span data-ttu-id="3fe15-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fe15-153">DateTimeOffset</span></span>|<span data-ttu-id="3fe15-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3fe15-154">DateTime the object was created.</span></span> <span data-ttu-id="3fe15-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fe15-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fe15-156">description</span><span class="sxs-lookup"><span data-stu-id="3fe15-156">description</span></span>|<span data-ttu-id="3fe15-157">String</span><span class="sxs-lookup"><span data-stu-id="3fe15-157">String</span></span>|<span data-ttu-id="3fe15-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3fe15-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3fe15-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fe15-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fe15-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3fe15-160">displayName</span></span>|<span data-ttu-id="3fe15-161">String</span><span class="sxs-lookup"><span data-stu-id="3fe15-161">String</span></span>|<span data-ttu-id="3fe15-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3fe15-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3fe15-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fe15-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fe15-164">version</span><span class="sxs-lookup"><span data-stu-id="3fe15-164">version</span></span>|<span data-ttu-id="3fe15-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3fe15-165">Int32</span></span>|<span data-ttu-id="3fe15-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3fe15-166">Version of the device configuration.</span></span> <span data-ttu-id="3fe15-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fe15-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fe15-168">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="3fe15-168">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="3fe15-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-169">Boolean</span></span>|<span data-ttu-id="3fe15-170">Valor que indica se esta política se aplica somente ao Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="3fe15-170">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="3fe15-171">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3fe15-171">This property is read-only.</span></span>|
|<span data-ttu-id="3fe15-172">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="3fe15-172">appsBlockCopyPaste</span></span>|<span data-ttu-id="3fe15-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-173">Boolean</span></span>|<span data-ttu-id="3fe15-174">Indica se a função copiar/colar deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="3fe15-174">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="3fe15-175">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="3fe15-175">bluetoothBlocked</span></span>|<span data-ttu-id="3fe15-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-176">Boolean</span></span>|<span data-ttu-id="3fe15-177">Indica se o bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3fe15-177">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="3fe15-178">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="3fe15-178">cameraBlocked</span></span>|<span data-ttu-id="3fe15-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-179">Boolean</span></span>|<span data-ttu-id="3fe15-180">Indica se a câmera deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="3fe15-180">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="3fe15-181">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="3fe15-181">cellularBlockWifiTethering</span></span>|<span data-ttu-id="3fe15-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-182">Boolean</span></span>|<span data-ttu-id="3fe15-183">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3fe15-183">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="3fe15-184">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3fe15-184">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="3fe15-185">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="3fe15-185">compliantAppsList</span></span>|<span data-ttu-id="3fe15-186">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="3fe15-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3fe15-187">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="3fe15-187">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="3fe15-188">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="3fe15-188">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="3fe15-189">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="3fe15-189">compliantAppListType</span></span>|[<span data-ttu-id="3fe15-190">appListType</span><span class="sxs-lookup"><span data-stu-id="3fe15-190">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="3fe15-191">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="3fe15-191">List that is in the AppComplianceList.</span></span> <span data-ttu-id="3fe15-192">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="3fe15-192">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="3fe15-193">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="3fe15-193">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="3fe15-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-194">Boolean</span></span>|<span data-ttu-id="3fe15-195">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3fe15-195">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="3fe15-196">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="3fe15-196">emailBlockAddingAccounts</span></span>|<span data-ttu-id="3fe15-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-197">Boolean</span></span>|<span data-ttu-id="3fe15-198">Indica se as contas de email personalizadas devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="3fe15-198">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="3fe15-199">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="3fe15-199">locationServicesBlocked</span></span>|<span data-ttu-id="3fe15-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-200">Boolean</span></span>|<span data-ttu-id="3fe15-201">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="3fe15-201">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="3fe15-202">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="3fe15-202">microsoftAccountBlocked</span></span>|<span data-ttu-id="3fe15-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-203">Boolean</span></span>|<span data-ttu-id="3fe15-204">Indica se o uso de uma conta da Microsoft deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3fe15-204">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="3fe15-205">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="3fe15-205">nfcBlocked</span></span>|<span data-ttu-id="3fe15-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-206">Boolean</span></span>|<span data-ttu-id="3fe15-207">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="3fe15-207">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="3fe15-208">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="3fe15-208">passwordBlockSimple</span></span>|<span data-ttu-id="3fe15-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-209">Boolean</span></span>|<span data-ttu-id="3fe15-210">Indica se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="3fe15-210">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="3fe15-211">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3fe15-211">passwordExpirationDays</span></span>|<span data-ttu-id="3fe15-212">Int32</span><span class="sxs-lookup"><span data-stu-id="3fe15-212">Int32</span></span>|<span data-ttu-id="3fe15-213">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="3fe15-213">Number of days before the password expires.</span></span>|
|<span data-ttu-id="3fe15-214">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3fe15-214">passwordMinimumLength</span></span>|<span data-ttu-id="3fe15-215">Int32</span><span class="sxs-lookup"><span data-stu-id="3fe15-215">Int32</span></span>|<span data-ttu-id="3fe15-216">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="3fe15-216">Minimum length of passwords.</span></span>|
|<span data-ttu-id="3fe15-217">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="3fe15-217">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="3fe15-218">Int32</span><span class="sxs-lookup"><span data-stu-id="3fe15-218">Int32</span></span>|<span data-ttu-id="3fe15-219">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="3fe15-219">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="3fe15-220">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3fe15-220">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="3fe15-221">Int32</span><span class="sxs-lookup"><span data-stu-id="3fe15-221">Int32</span></span>|<span data-ttu-id="3fe15-222">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="3fe15-222">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="3fe15-223">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3fe15-223">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3fe15-224">Int32</span><span class="sxs-lookup"><span data-stu-id="3fe15-224">Int32</span></span>|<span data-ttu-id="3fe15-225">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="3fe15-225">Number of previous passwords to block.</span></span> <span data-ttu-id="3fe15-226">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="3fe15-226">Valid values 0 to 24</span></span>|
|<span data-ttu-id="3fe15-227">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="3fe15-227">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="3fe15-228">Int32</span><span class="sxs-lookup"><span data-stu-id="3fe15-228">Int32</span></span>|<span data-ttu-id="3fe15-229">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="3fe15-229">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="3fe15-230">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3fe15-230">passwordRequiredType</span></span>|[<span data-ttu-id="3fe15-231">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3fe15-231">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="3fe15-232">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="3fe15-232">Password type that is required.</span></span> <span data-ttu-id="3fe15-233">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="3fe15-233">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3fe15-234">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3fe15-234">passwordRequired</span></span>|<span data-ttu-id="3fe15-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-235">Boolean</span></span>|<span data-ttu-id="3fe15-236">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="3fe15-236">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="3fe15-237">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="3fe15-237">screenCaptureBlocked</span></span>|<span data-ttu-id="3fe15-238">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-238">Boolean</span></span>|<span data-ttu-id="3fe15-239">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="3fe15-239">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="3fe15-240">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="3fe15-240">storageBlockRemovableStorage</span></span>|<span data-ttu-id="3fe15-241">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-241">Boolean</span></span>|<span data-ttu-id="3fe15-242">Indica se o armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3fe15-242">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="3fe15-243">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="3fe15-243">storageRequireEncryption</span></span>|<span data-ttu-id="3fe15-244">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-244">Boolean</span></span>|<span data-ttu-id="3fe15-245">Indica se a criptografia é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="3fe15-245">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="3fe15-246">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="3fe15-246">webBrowserBlocked</span></span>|<span data-ttu-id="3fe15-247">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-247">Boolean</span></span>|<span data-ttu-id="3fe15-248">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3fe15-248">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="3fe15-249">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="3fe15-249">wifiBlocked</span></span>|<span data-ttu-id="3fe15-250">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-250">Boolean</span></span>|<span data-ttu-id="3fe15-251">Indica se o Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3fe15-251">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="3fe15-252">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="3fe15-252">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="3fe15-253">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-253">Boolean</span></span>|<span data-ttu-id="3fe15-254">Indica se a conexão automática a hotspots Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="3fe15-254">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="3fe15-255">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3fe15-255">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="3fe15-256">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="3fe15-256">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="3fe15-257">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-257">Boolean</span></span>|<span data-ttu-id="3fe15-258">Indica se os relatórios de hotspot Wi-Fi devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="3fe15-258">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="3fe15-259">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3fe15-259">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="3fe15-260">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="3fe15-260">windowsStoreBlocked</span></span>|<span data-ttu-id="3fe15-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fe15-261">Boolean</span></span>|<span data-ttu-id="3fe15-262">Indica se a Windows Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="3fe15-262">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="3fe15-263">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fe15-263">Response</span></span>
<span data-ttu-id="3fe15-264">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fe15-264">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fe15-265">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fe15-265">Example</span></span>
### <a name="request"></a><span data-ttu-id="3fe15-266">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fe15-266">Request</span></span>
<span data-ttu-id="3fe15-267">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fe15-267">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1544

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="3fe15-268">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fe15-268">Response</span></span>
<span data-ttu-id="3fe15-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3fe15-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1725

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```





