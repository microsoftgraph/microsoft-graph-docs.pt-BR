---
title: Atualizar windowsPhone81GeneralConfiguration
description: Atualizar as propriedades de um objeto windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c4393c3a8cf1f55dd199a69cc58cab5094c1b710
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827535"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="0bada-103">Atualizar windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="0bada-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="0bada-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0bada-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bada-105">Atualizar as propriedades de um objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bada-105">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0bada-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0bada-106">Prerequisites</span></span>
<span data-ttu-id="0bada-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bada-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bada-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bada-109">Permission type</span></span>|<span data-ttu-id="0bada-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0bada-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bada-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bada-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0bada-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bada-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0bada-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bada-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bada-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bada-114">Not supported.</span></span>|
|<span data-ttu-id="0bada-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bada-115">Application</span></span>|<span data-ttu-id="0bada-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bada-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bada-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bada-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0bada-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bada-118">Request headers</span></span>
|<span data-ttu-id="0bada-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0bada-119">Header</span></span>|<span data-ttu-id="0bada-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0bada-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bada-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bada-121">Authorization</span></span>|<span data-ttu-id="0bada-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bada-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bada-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0bada-123">Accept</span></span>|<span data-ttu-id="0bada-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0bada-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bada-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bada-125">Request body</span></span>
<span data-ttu-id="0bada-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bada-126">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="0bada-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bada-127">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="0bada-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bada-128">Property</span></span>|<span data-ttu-id="0bada-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bada-129">Type</span></span>|<span data-ttu-id="0bada-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bada-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bada-131">id</span><span class="sxs-lookup"><span data-stu-id="0bada-131">id</span></span>|<span data-ttu-id="0bada-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bada-132">String</span></span>|<span data-ttu-id="0bada-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0bada-133">Key of the entity.</span></span> <span data-ttu-id="0bada-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bada-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bada-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0bada-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0bada-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bada-136">DateTimeOffset</span></span>|<span data-ttu-id="0bada-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0bada-137">DateTime the object was last modified.</span></span> <span data-ttu-id="0bada-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bada-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bada-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0bada-139">createdDateTime</span></span>|<span data-ttu-id="0bada-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bada-140">DateTimeOffset</span></span>|<span data-ttu-id="0bada-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0bada-141">DateTime the object was created.</span></span> <span data-ttu-id="0bada-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bada-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bada-143">description</span><span class="sxs-lookup"><span data-stu-id="0bada-143">description</span></span>|<span data-ttu-id="0bada-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bada-144">String</span></span>|<span data-ttu-id="0bada-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0bada-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0bada-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bada-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bada-147">displayName</span><span class="sxs-lookup"><span data-stu-id="0bada-147">displayName</span></span>|<span data-ttu-id="0bada-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bada-148">String</span></span>|<span data-ttu-id="0bada-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0bada-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0bada-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bada-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bada-151">version</span><span class="sxs-lookup"><span data-stu-id="0bada-151">version</span></span>|<span data-ttu-id="0bada-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0bada-152">Int32</span></span>|<span data-ttu-id="0bada-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0bada-153">Version of the device configuration.</span></span> <span data-ttu-id="0bada-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bada-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bada-155">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="0bada-155">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="0bada-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-156">Boolean</span></span>|<span data-ttu-id="0bada-157">Valor que indica se esta política se aplica somente ao Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="0bada-157">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="0bada-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0bada-158">This property is read-only.</span></span>|
|<span data-ttu-id="0bada-159">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="0bada-159">appsBlockCopyPaste</span></span>|<span data-ttu-id="0bada-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-160">Boolean</span></span>|<span data-ttu-id="0bada-161">Indica se a função copiar/colar deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="0bada-161">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="0bada-162">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="0bada-162">bluetoothBlocked</span></span>|<span data-ttu-id="0bada-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-163">Boolean</span></span>|<span data-ttu-id="0bada-164">Indica se o bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="0bada-164">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="0bada-165">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="0bada-165">cameraBlocked</span></span>|<span data-ttu-id="0bada-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-166">Boolean</span></span>|<span data-ttu-id="0bada-167">Indica se a câmera deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="0bada-167">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="0bada-168">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="0bada-168">cellularBlockWifiTethering</span></span>|<span data-ttu-id="0bada-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-169">Boolean</span></span>|<span data-ttu-id="0bada-170">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="0bada-170">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="0bada-171">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="0bada-171">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="0bada-172">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="0bada-172">compliantAppsList</span></span>|<span data-ttu-id="0bada-173">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="0bada-173">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="0bada-174">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="0bada-174">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="0bada-175">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="0bada-175">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="0bada-176">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="0bada-176">compliantAppListType</span></span>|[<span data-ttu-id="0bada-177">appListType</span><span class="sxs-lookup"><span data-stu-id="0bada-177">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="0bada-178">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="0bada-178">List that is in the AppComplianceList.</span></span> <span data-ttu-id="0bada-179">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="0bada-179">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="0bada-180">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="0bada-180">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="0bada-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-181">Boolean</span></span>|<span data-ttu-id="0bada-182">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="0bada-182">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="0bada-183">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="0bada-183">emailBlockAddingAccounts</span></span>|<span data-ttu-id="0bada-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-184">Boolean</span></span>|<span data-ttu-id="0bada-185">Indica se as contas de email personalizadas devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="0bada-185">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="0bada-186">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="0bada-186">locationServicesBlocked</span></span>|<span data-ttu-id="0bada-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-187">Boolean</span></span>|<span data-ttu-id="0bada-188">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="0bada-188">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="0bada-189">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="0bada-189">microsoftAccountBlocked</span></span>|<span data-ttu-id="0bada-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-190">Boolean</span></span>|<span data-ttu-id="0bada-191">Indica se o uso de uma conta da Microsoft deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="0bada-191">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="0bada-192">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="0bada-192">nfcBlocked</span></span>|<span data-ttu-id="0bada-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-193">Boolean</span></span>|<span data-ttu-id="0bada-194">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="0bada-194">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="0bada-195">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0bada-195">passwordBlockSimple</span></span>|<span data-ttu-id="0bada-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-196">Boolean</span></span>|<span data-ttu-id="0bada-197">Indica se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="0bada-197">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="0bada-198">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0bada-198">passwordExpirationDays</span></span>|<span data-ttu-id="0bada-199">Int32</span><span class="sxs-lookup"><span data-stu-id="0bada-199">Int32</span></span>|<span data-ttu-id="0bada-200">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="0bada-200">Number of days before the password expires.</span></span>|
|<span data-ttu-id="0bada-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0bada-201">passwordMinimumLength</span></span>|<span data-ttu-id="0bada-202">Int32</span><span class="sxs-lookup"><span data-stu-id="0bada-202">Int32</span></span>|<span data-ttu-id="0bada-203">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="0bada-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="0bada-204">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="0bada-204">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="0bada-205">Int32</span><span class="sxs-lookup"><span data-stu-id="0bada-205">Int32</span></span>|<span data-ttu-id="0bada-206">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="0bada-206">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="0bada-207">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0bada-207">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0bada-208">Int32</span><span class="sxs-lookup"><span data-stu-id="0bada-208">Int32</span></span>|<span data-ttu-id="0bada-209">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="0bada-209">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="0bada-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0bada-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0bada-211">Int32</span><span class="sxs-lookup"><span data-stu-id="0bada-211">Int32</span></span>|<span data-ttu-id="0bada-212">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="0bada-212">Number of previous passwords to block.</span></span> <span data-ttu-id="0bada-213">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="0bada-213">Valid values 0 to 24</span></span>|
|<span data-ttu-id="0bada-214">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="0bada-214">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="0bada-215">Int32</span><span class="sxs-lookup"><span data-stu-id="0bada-215">Int32</span></span>|<span data-ttu-id="0bada-216">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="0bada-216">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="0bada-217">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0bada-217">passwordRequiredType</span></span>|[<span data-ttu-id="0bada-218">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0bada-218">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0bada-219">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="0bada-219">Password type that is required.</span></span> <span data-ttu-id="0bada-220">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="0bada-220">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0bada-221">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0bada-221">passwordRequired</span></span>|<span data-ttu-id="0bada-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-222">Boolean</span></span>|<span data-ttu-id="0bada-223">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="0bada-223">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="0bada-224">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="0bada-224">screenCaptureBlocked</span></span>|<span data-ttu-id="0bada-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-225">Boolean</span></span>|<span data-ttu-id="0bada-226">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="0bada-226">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="0bada-227">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="0bada-227">storageBlockRemovableStorage</span></span>|<span data-ttu-id="0bada-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-228">Boolean</span></span>|<span data-ttu-id="0bada-229">Indica se o armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="0bada-229">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="0bada-230">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0bada-230">storageRequireEncryption</span></span>|<span data-ttu-id="0bada-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-231">Boolean</span></span>|<span data-ttu-id="0bada-232">Indica se a criptografia é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="0bada-232">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="0bada-233">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="0bada-233">webBrowserBlocked</span></span>|<span data-ttu-id="0bada-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-234">Boolean</span></span>|<span data-ttu-id="0bada-235">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="0bada-235">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="0bada-236">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="0bada-236">wifiBlocked</span></span>|<span data-ttu-id="0bada-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-237">Boolean</span></span>|<span data-ttu-id="0bada-238">Indica se o Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="0bada-238">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="0bada-239">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="0bada-239">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="0bada-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-240">Boolean</span></span>|<span data-ttu-id="0bada-241">Indica se a conexão automática a hotspots Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="0bada-241">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="0bada-242">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="0bada-242">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="0bada-243">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="0bada-243">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="0bada-244">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-244">Boolean</span></span>|<span data-ttu-id="0bada-245">Indica se os relatórios de hotspot Wi-Fi devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="0bada-245">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="0bada-246">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="0bada-246">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="0bada-247">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="0bada-247">windowsStoreBlocked</span></span>|<span data-ttu-id="0bada-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bada-248">Boolean</span></span>|<span data-ttu-id="0bada-249">Indica se a Windows Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="0bada-249">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="0bada-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bada-250">Response</span></span>
<span data-ttu-id="0bada-251">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bada-251">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bada-252">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0bada-252">Example</span></span>
### <a name="request"></a><span data-ttu-id="0bada-253">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bada-253">Request</span></span>
<span data-ttu-id="0bada-254">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bada-254">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="0bada-255">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bada-255">Response</span></span>
<span data-ttu-id="0bada-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0bada-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



