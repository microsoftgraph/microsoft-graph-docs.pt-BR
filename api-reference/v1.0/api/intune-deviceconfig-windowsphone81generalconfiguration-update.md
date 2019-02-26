---
title: Atualizar windowsPhone81GeneralConfiguration
description: Atualizar as propriedades de um objeto windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49a200ef46b9f7f068d7100888daae576d7e8c9c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263928"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="4c614-103">Atualizar windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c614-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="4c614-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c614-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c614-105">Atualizar as propriedades de um objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c614-105">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c614-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c614-106">Prerequisites</span></span>
<span data-ttu-id="4c614-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4c614-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4c614-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c614-109">Permission type</span></span>|<span data-ttu-id="4c614-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4c614-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c614-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c614-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c614-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c614-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c614-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c614-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c614-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c614-114">Not supported.</span></span>|
|<span data-ttu-id="4c614-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c614-115">Application</span></span>|<span data-ttu-id="4c614-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c614-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c614-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c614-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4c614-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c614-118">Request headers</span></span>
|<span data-ttu-id="4c614-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c614-119">Header</span></span>|<span data-ttu-id="4c614-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4c614-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c614-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c614-121">Authorization</span></span>|<span data-ttu-id="4c614-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c614-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c614-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4c614-123">Accept</span></span>|<span data-ttu-id="4c614-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4c614-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c614-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c614-125">Request body</span></span>
<span data-ttu-id="4c614-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c614-126">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="4c614-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c614-127">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="4c614-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c614-128">Property</span></span>|<span data-ttu-id="4c614-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c614-129">Type</span></span>|<span data-ttu-id="4c614-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c614-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c614-131">id</span><span class="sxs-lookup"><span data-stu-id="4c614-131">id</span></span>|<span data-ttu-id="4c614-132">String</span><span class="sxs-lookup"><span data-stu-id="4c614-132">String</span></span>|<span data-ttu-id="4c614-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4c614-133">Key of the entity.</span></span> <span data-ttu-id="4c614-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c614-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c614-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c614-135">lastModifiedDateTime</span></span>|<span data-ttu-id="4c614-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c614-136">DateTimeOffset</span></span>|<span data-ttu-id="4c614-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4c614-137">DateTime the object was last modified.</span></span> <span data-ttu-id="4c614-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c614-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c614-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c614-139">createdDateTime</span></span>|<span data-ttu-id="4c614-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c614-140">DateTimeOffset</span></span>|<span data-ttu-id="4c614-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4c614-141">DateTime the object was created.</span></span> <span data-ttu-id="4c614-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c614-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c614-143">description</span><span class="sxs-lookup"><span data-stu-id="4c614-143">description</span></span>|<span data-ttu-id="4c614-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c614-144">String</span></span>|<span data-ttu-id="4c614-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4c614-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4c614-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c614-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c614-147">displayName</span><span class="sxs-lookup"><span data-stu-id="4c614-147">displayName</span></span>|<span data-ttu-id="4c614-148">String</span><span class="sxs-lookup"><span data-stu-id="4c614-148">String</span></span>|<span data-ttu-id="4c614-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4c614-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4c614-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c614-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c614-151">version</span><span class="sxs-lookup"><span data-stu-id="4c614-151">version</span></span>|<span data-ttu-id="4c614-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4c614-152">Int32</span></span>|<span data-ttu-id="4c614-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4c614-153">Version of the device configuration.</span></span> <span data-ttu-id="4c614-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c614-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c614-155">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="4c614-155">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="4c614-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-156">Boolean</span></span>|<span data-ttu-id="4c614-157">Valor que indica se esta política se aplica somente ao Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="4c614-157">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="4c614-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c614-158">This property is read-only.</span></span>|
|<span data-ttu-id="4c614-159">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="4c614-159">appsBlockCopyPaste</span></span>|<span data-ttu-id="4c614-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-160">Boolean</span></span>|<span data-ttu-id="4c614-161">Indica se a função copiar/colar deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4c614-161">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="4c614-162">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="4c614-162">bluetoothBlocked</span></span>|<span data-ttu-id="4c614-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-163">Boolean</span></span>|<span data-ttu-id="4c614-164">Indica se o bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4c614-164">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="4c614-165">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="4c614-165">cameraBlocked</span></span>|<span data-ttu-id="4c614-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-166">Boolean</span></span>|<span data-ttu-id="4c614-167">Indica se a câmera deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4c614-167">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="4c614-168">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="4c614-168">cellularBlockWifiTethering</span></span>|<span data-ttu-id="4c614-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-169">Boolean</span></span>|<span data-ttu-id="4c614-170">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4c614-170">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="4c614-171">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4c614-171">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4c614-172">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="4c614-172">compliantAppsList</span></span>|<span data-ttu-id="4c614-173">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="4c614-173">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4c614-174">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="4c614-174">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="4c614-175">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="4c614-175">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4c614-176">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="4c614-176">compliantAppListType</span></span>|[<span data-ttu-id="4c614-177">appListType</span><span class="sxs-lookup"><span data-stu-id="4c614-177">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="4c614-178">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="4c614-178">List that is in the AppComplianceList.</span></span> <span data-ttu-id="4c614-179">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="4c614-179">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="4c614-180">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="4c614-180">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="4c614-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-181">Boolean</span></span>|<span data-ttu-id="4c614-182">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4c614-182">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="4c614-183">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="4c614-183">emailBlockAddingAccounts</span></span>|<span data-ttu-id="4c614-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-184">Boolean</span></span>|<span data-ttu-id="4c614-185">Indica se as contas de email personalizadas devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="4c614-185">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="4c614-186">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="4c614-186">locationServicesBlocked</span></span>|<span data-ttu-id="4c614-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-187">Boolean</span></span>|<span data-ttu-id="4c614-188">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="4c614-188">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="4c614-189">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="4c614-189">microsoftAccountBlocked</span></span>|<span data-ttu-id="4c614-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-190">Boolean</span></span>|<span data-ttu-id="4c614-191">Indica se o uso de uma conta da Microsoft deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4c614-191">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="4c614-192">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="4c614-192">nfcBlocked</span></span>|<span data-ttu-id="4c614-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-193">Boolean</span></span>|<span data-ttu-id="4c614-194">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4c614-194">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="4c614-195">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4c614-195">passwordBlockSimple</span></span>|<span data-ttu-id="4c614-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-196">Boolean</span></span>|<span data-ttu-id="4c614-197">Indica se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4c614-197">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="4c614-198">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4c614-198">passwordExpirationDays</span></span>|<span data-ttu-id="4c614-199">Int32</span><span class="sxs-lookup"><span data-stu-id="4c614-199">Int32</span></span>|<span data-ttu-id="4c614-200">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="4c614-200">Number of days before the password expires.</span></span>|
|<span data-ttu-id="4c614-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4c614-201">passwordMinimumLength</span></span>|<span data-ttu-id="4c614-202">Int32</span><span class="sxs-lookup"><span data-stu-id="4c614-202">Int32</span></span>|<span data-ttu-id="4c614-203">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="4c614-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="4c614-204">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4c614-204">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4c614-205">Int32</span><span class="sxs-lookup"><span data-stu-id="4c614-205">Int32</span></span>|<span data-ttu-id="4c614-206">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="4c614-206">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="4c614-207">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4c614-207">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4c614-208">Int32</span><span class="sxs-lookup"><span data-stu-id="4c614-208">Int32</span></span>|<span data-ttu-id="4c614-209">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="4c614-209">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="4c614-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4c614-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4c614-211">Int32</span><span class="sxs-lookup"><span data-stu-id="4c614-211">Int32</span></span>|<span data-ttu-id="4c614-212">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="4c614-212">Number of previous passwords to block.</span></span> <span data-ttu-id="4c614-213">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="4c614-213">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4c614-214">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4c614-214">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4c614-215">Int32</span><span class="sxs-lookup"><span data-stu-id="4c614-215">Int32</span></span>|<span data-ttu-id="4c614-216">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="4c614-216">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="4c614-217">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4c614-217">passwordRequiredType</span></span>|[<span data-ttu-id="4c614-218">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4c614-218">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4c614-219">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="4c614-219">Password type that is required.</span></span> <span data-ttu-id="4c614-220">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="4c614-220">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4c614-221">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4c614-221">passwordRequired</span></span>|<span data-ttu-id="4c614-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-222">Boolean</span></span>|<span data-ttu-id="4c614-223">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="4c614-223">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="4c614-224">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="4c614-224">screenCaptureBlocked</span></span>|<span data-ttu-id="4c614-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-225">Boolean</span></span>|<span data-ttu-id="4c614-226">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="4c614-226">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="4c614-227">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="4c614-227">storageBlockRemovableStorage</span></span>|<span data-ttu-id="4c614-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-228">Boolean</span></span>|<span data-ttu-id="4c614-229">Indica se o armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4c614-229">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="4c614-230">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4c614-230">storageRequireEncryption</span></span>|<span data-ttu-id="4c614-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-231">Boolean</span></span>|<span data-ttu-id="4c614-232">Indica se a criptografia é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="4c614-232">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="4c614-233">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="4c614-233">webBrowserBlocked</span></span>|<span data-ttu-id="4c614-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-234">Boolean</span></span>|<span data-ttu-id="4c614-235">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4c614-235">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="4c614-236">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="4c614-236">wifiBlocked</span></span>|<span data-ttu-id="4c614-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-237">Boolean</span></span>|<span data-ttu-id="4c614-238">Indica se o Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4c614-238">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="4c614-239">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="4c614-239">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="4c614-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-240">Boolean</span></span>|<span data-ttu-id="4c614-241">Indica se a conexão automática a hotspots Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4c614-241">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="4c614-242">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4c614-242">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4c614-243">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="4c614-243">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="4c614-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-244">Boolean</span></span>|<span data-ttu-id="4c614-245">Indica se os relatórios de hotspot Wi-Fi devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="4c614-245">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="4c614-246">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4c614-246">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4c614-247">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="4c614-247">windowsStoreBlocked</span></span>|<span data-ttu-id="4c614-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c614-248">Boolean</span></span>|<span data-ttu-id="4c614-249">Indica se a Windows Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4c614-249">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="4c614-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c614-250">Response</span></span>
<span data-ttu-id="4c614-251">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c614-251">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c614-252">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c614-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c614-253">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c614-253">Request</span></span>
<span data-ttu-id="4c614-254">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c614-254">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4c614-255">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c614-255">Response</span></span>
<span data-ttu-id="4c614-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c614-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



