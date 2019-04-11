---
title: Criar windowsPhone81GeneralConfiguration
description: Criar um novo objeto windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e43396a0001d6c2dd7dfd836eccf89432f3ff30
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783798"
---
# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="1d195-103">Criar windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="1d195-103">Create windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="1d195-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d195-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d195-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d195-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d195-106">Criar um novo objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d195-106">Create a new [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d195-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1d195-107">Prerequisites</span></span>
<span data-ttu-id="1d195-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d195-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d195-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d195-110">Permission type</span></span>|<span data-ttu-id="1d195-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1d195-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d195-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d195-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d195-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d195-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1d195-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d195-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d195-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d195-115">Not supported.</span></span>|
|<span data-ttu-id="1d195-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d195-116">Application</span></span>|<span data-ttu-id="1d195-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d195-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d195-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d195-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1d195-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d195-119">Request headers</span></span>
|<span data-ttu-id="1d195-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d195-120">Header</span></span>|<span data-ttu-id="1d195-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1d195-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d195-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d195-122">Authorization</span></span>|<span data-ttu-id="1d195-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d195-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d195-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1d195-124">Accept</span></span>|<span data-ttu-id="1d195-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1d195-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d195-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d195-126">Request body</span></span>
<span data-ttu-id="1d195-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1d195-127">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="1d195-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1d195-128">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="1d195-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d195-129">Property</span></span>|<span data-ttu-id="1d195-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d195-130">Type</span></span>|<span data-ttu-id="1d195-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d195-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d195-132">id</span><span class="sxs-lookup"><span data-stu-id="1d195-132">id</span></span>|<span data-ttu-id="1d195-133">String</span><span class="sxs-lookup"><span data-stu-id="1d195-133">String</span></span>|<span data-ttu-id="1d195-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1d195-134">Key of the entity.</span></span> <span data-ttu-id="1d195-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d195-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d195-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d195-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1d195-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d195-137">DateTimeOffset</span></span>|<span data-ttu-id="1d195-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1d195-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1d195-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d195-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d195-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1d195-140">roleScopeTagIds</span></span>|<span data-ttu-id="1d195-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="1d195-141">String collection</span></span>|<span data-ttu-id="1d195-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="1d195-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1d195-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d195-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d195-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1d195-144">supportsScopeTags</span></span>|<span data-ttu-id="1d195-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-145">Boolean</span></span>|<span data-ttu-id="1d195-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="1d195-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1d195-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="1d195-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1d195-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="1d195-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1d195-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1d195-149">This property is read-only.</span></span> <span data-ttu-id="1d195-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d195-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d195-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d195-151">createdDateTime</span></span>|<span data-ttu-id="1d195-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d195-152">DateTimeOffset</span></span>|<span data-ttu-id="1d195-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1d195-153">DateTime the object was created.</span></span> <span data-ttu-id="1d195-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d195-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d195-155">description</span><span class="sxs-lookup"><span data-stu-id="1d195-155">description</span></span>|<span data-ttu-id="1d195-156">String</span><span class="sxs-lookup"><span data-stu-id="1d195-156">String</span></span>|<span data-ttu-id="1d195-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1d195-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1d195-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d195-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d195-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1d195-159">displayName</span></span>|<span data-ttu-id="1d195-160">String</span><span class="sxs-lookup"><span data-stu-id="1d195-160">String</span></span>|<span data-ttu-id="1d195-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1d195-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1d195-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d195-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d195-163">versão</span><span class="sxs-lookup"><span data-stu-id="1d195-163">version</span></span>|<span data-ttu-id="1d195-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1d195-164">Int32</span></span>|<span data-ttu-id="1d195-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1d195-165">Version of the device configuration.</span></span> <span data-ttu-id="1d195-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d195-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d195-167">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="1d195-167">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="1d195-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-168">Boolean</span></span>|<span data-ttu-id="1d195-169">Valor que indica se esta política se aplica somente ao Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="1d195-169">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="1d195-170">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1d195-170">This property is read-only.</span></span>|
|<span data-ttu-id="1d195-171">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="1d195-171">appsBlockCopyPaste</span></span>|<span data-ttu-id="1d195-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-172">Boolean</span></span>|<span data-ttu-id="1d195-173">Indica se a função copiar/colar deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1d195-173">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="1d195-174">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="1d195-174">bluetoothBlocked</span></span>|<span data-ttu-id="1d195-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-175">Boolean</span></span>|<span data-ttu-id="1d195-176">Indica se o bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1d195-176">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="1d195-177">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="1d195-177">cameraBlocked</span></span>|<span data-ttu-id="1d195-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-178">Boolean</span></span>|<span data-ttu-id="1d195-179">Indica se a câmera deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1d195-179">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="1d195-180">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="1d195-180">cellularBlockWifiTethering</span></span>|<span data-ttu-id="1d195-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-181">Boolean</span></span>|<span data-ttu-id="1d195-182">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1d195-182">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="1d195-183">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1d195-183">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="1d195-184">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="1d195-184">compliantAppsList</span></span>|<span data-ttu-id="1d195-185">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="1d195-185">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1d195-186">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="1d195-186">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="1d195-187">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="1d195-187">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="1d195-188">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="1d195-188">compliantAppListType</span></span>|[<span data-ttu-id="1d195-189">appListType</span><span class="sxs-lookup"><span data-stu-id="1d195-189">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="1d195-190">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="1d195-190">List that is in the AppComplianceList.</span></span> <span data-ttu-id="1d195-191">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="1d195-191">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="1d195-192">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="1d195-192">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="1d195-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-193">Boolean</span></span>|<span data-ttu-id="1d195-194">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1d195-194">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="1d195-195">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="1d195-195">emailBlockAddingAccounts</span></span>|<span data-ttu-id="1d195-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d195-196">Boolean</span></span>|<span data-ttu-id="1d195-197">Indica se as contas de email personalizadas devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="1d195-197">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="1d195-198">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="1d195-198">locationServicesBlocked</span></span>|<span data-ttu-id="1d195-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-199">Boolean</span></span>|<span data-ttu-id="1d195-200">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="1d195-200">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="1d195-201">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="1d195-201">microsoftAccountBlocked</span></span>|<span data-ttu-id="1d195-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-202">Boolean</span></span>|<span data-ttu-id="1d195-203">Indica se o uso de uma conta da Microsoft deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1d195-203">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="1d195-204">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="1d195-204">nfcBlocked</span></span>|<span data-ttu-id="1d195-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-205">Boolean</span></span>|<span data-ttu-id="1d195-206">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1d195-206">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="1d195-207">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="1d195-207">passwordBlockSimple</span></span>|<span data-ttu-id="1d195-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d195-208">Boolean</span></span>|<span data-ttu-id="1d195-209">Indica se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1d195-209">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="1d195-210">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1d195-210">passwordExpirationDays</span></span>|<span data-ttu-id="1d195-211">Int32</span><span class="sxs-lookup"><span data-stu-id="1d195-211">Int32</span></span>|<span data-ttu-id="1d195-212">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="1d195-212">Number of days before the password expires.</span></span>|
|<span data-ttu-id="1d195-213">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1d195-213">passwordMinimumLength</span></span>|<span data-ttu-id="1d195-214">Int32</span><span class="sxs-lookup"><span data-stu-id="1d195-214">Int32</span></span>|<span data-ttu-id="1d195-215">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="1d195-215">Minimum length of passwords.</span></span>|
|<span data-ttu-id="1d195-216">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1d195-216">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1d195-217">Int32</span><span class="sxs-lookup"><span data-stu-id="1d195-217">Int32</span></span>|<span data-ttu-id="1d195-218">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="1d195-218">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="1d195-219">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="1d195-219">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="1d195-220">Int32</span><span class="sxs-lookup"><span data-stu-id="1d195-220">Int32</span></span>|<span data-ttu-id="1d195-221">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="1d195-221">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="1d195-222">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1d195-222">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1d195-223">Int32</span><span class="sxs-lookup"><span data-stu-id="1d195-223">Int32</span></span>|<span data-ttu-id="1d195-224">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="1d195-224">Number of previous passwords to block.</span></span> <span data-ttu-id="1d195-225">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="1d195-225">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1d195-226">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1d195-226">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1d195-227">Int32</span><span class="sxs-lookup"><span data-stu-id="1d195-227">Int32</span></span>|<span data-ttu-id="1d195-228">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="1d195-228">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="1d195-229">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1d195-229">passwordRequiredType</span></span>|[<span data-ttu-id="1d195-230">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1d195-230">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="1d195-231">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="1d195-231">Password type that is required.</span></span> <span data-ttu-id="1d195-232">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="1d195-232">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="1d195-233">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="1d195-233">passwordRequired</span></span>|<span data-ttu-id="1d195-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-234">Boolean</span></span>|<span data-ttu-id="1d195-235">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="1d195-235">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="1d195-236">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="1d195-236">screenCaptureBlocked</span></span>|<span data-ttu-id="1d195-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-237">Boolean</span></span>|<span data-ttu-id="1d195-238">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="1d195-238">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="1d195-239">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="1d195-239">storageBlockRemovableStorage</span></span>|<span data-ttu-id="1d195-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-240">Boolean</span></span>|<span data-ttu-id="1d195-241">Indica se o armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1d195-241">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="1d195-242">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="1d195-242">storageRequireEncryption</span></span>|<span data-ttu-id="1d195-243">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-243">Boolean</span></span>|<span data-ttu-id="1d195-244">Indica se a criptografia é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="1d195-244">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="1d195-245">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="1d195-245">webBrowserBlocked</span></span>|<span data-ttu-id="1d195-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-246">Boolean</span></span>|<span data-ttu-id="1d195-247">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1d195-247">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="1d195-248">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="1d195-248">wifiBlocked</span></span>|<span data-ttu-id="1d195-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-249">Boolean</span></span>|<span data-ttu-id="1d195-250">Indica se o Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1d195-250">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="1d195-251">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="1d195-251">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="1d195-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d195-252">Boolean</span></span>|<span data-ttu-id="1d195-253">Indica se a conexão automática a hotspots Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1d195-253">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="1d195-254">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1d195-254">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="1d195-255">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="1d195-255">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="1d195-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d195-256">Boolean</span></span>|<span data-ttu-id="1d195-257">Indica se os relatórios de hotspot Wi-Fi devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="1d195-257">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="1d195-258">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1d195-258">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="1d195-259">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="1d195-259">windowsStoreBlocked</span></span>|<span data-ttu-id="1d195-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d195-260">Boolean</span></span>|<span data-ttu-id="1d195-261">Indica se a Windows Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1d195-261">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="1d195-262">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d195-262">Response</span></span>
<span data-ttu-id="1d195-263">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d195-263">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d195-264">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d195-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d195-265">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d195-265">Request</span></span>
<span data-ttu-id="1d195-266">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d195-266">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1553

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="1d195-267">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d195-267">Response</span></span>
<span data-ttu-id="1d195-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d195-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





