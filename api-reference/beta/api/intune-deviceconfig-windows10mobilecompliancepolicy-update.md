---
title: Atualizar windows10MobileCompliancePolicy
description: Atualiza as propriedades de um objeto windows10MobileCompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f1627513307aeca2ab198ccd75a273a79ee3b1ea
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408499"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="67354-103">Atualizar windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="67354-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="67354-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="67354-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="67354-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="67354-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67354-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="67354-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67354-107">Atualiza as propriedades de um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="67354-107">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67354-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67354-108">Prerequisites</span></span>
<span data-ttu-id="67354-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="67354-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="67354-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67354-111">Permission type</span></span>|<span data-ttu-id="67354-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67354-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67354-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67354-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67354-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67354-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="67354-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67354-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67354-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67354-116">Not supported.</span></span>|
|<span data-ttu-id="67354-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67354-117">Application</span></span>|<span data-ttu-id="67354-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67354-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67354-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67354-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="67354-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67354-120">Request headers</span></span>
|<span data-ttu-id="67354-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67354-121">Header</span></span>|<span data-ttu-id="67354-122">Valor</span><span class="sxs-lookup"><span data-stu-id="67354-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67354-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="67354-123">Authorization</span></span>|<span data-ttu-id="67354-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67354-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67354-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67354-125">Accept</span></span>|<span data-ttu-id="67354-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67354-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67354-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67354-127">Request body</span></span>
<span data-ttu-id="67354-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="67354-128">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="67354-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="67354-129">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="67354-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67354-130">Property</span></span>|<span data-ttu-id="67354-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="67354-131">Type</span></span>|<span data-ttu-id="67354-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="67354-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67354-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="67354-133">roleScopeTagIds</span></span>|<span data-ttu-id="67354-134">String collection</span><span class="sxs-lookup"><span data-stu-id="67354-134">String collection</span></span>|<span data-ttu-id="67354-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="67354-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="67354-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="67354-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="67354-137">id</span><span class="sxs-lookup"><span data-stu-id="67354-137">id</span></span>|<span data-ttu-id="67354-138">String</span><span class="sxs-lookup"><span data-stu-id="67354-138">String</span></span>|<span data-ttu-id="67354-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="67354-139">Key of the entity.</span></span> <span data-ttu-id="67354-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="67354-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="67354-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67354-141">createdDateTime</span></span>|<span data-ttu-id="67354-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67354-142">DateTimeOffset</span></span>|<span data-ttu-id="67354-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="67354-143">DateTime the object was created.</span></span> <span data-ttu-id="67354-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="67354-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="67354-145">description</span><span class="sxs-lookup"><span data-stu-id="67354-145">description</span></span>|<span data-ttu-id="67354-146">String</span><span class="sxs-lookup"><span data-stu-id="67354-146">String</span></span>|<span data-ttu-id="67354-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67354-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="67354-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="67354-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="67354-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67354-149">lastModifiedDateTime</span></span>|<span data-ttu-id="67354-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67354-150">DateTimeOffset</span></span>|<span data-ttu-id="67354-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="67354-151">DateTime the object was last modified.</span></span> <span data-ttu-id="67354-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="67354-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="67354-153">displayName</span><span class="sxs-lookup"><span data-stu-id="67354-153">displayName</span></span>|<span data-ttu-id="67354-154">String</span><span class="sxs-lookup"><span data-stu-id="67354-154">String</span></span>|<span data-ttu-id="67354-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67354-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="67354-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="67354-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="67354-157">version</span><span class="sxs-lookup"><span data-stu-id="67354-157">version</span></span>|<span data-ttu-id="67354-158">Int32</span><span class="sxs-lookup"><span data-stu-id="67354-158">Int32</span></span>|<span data-ttu-id="67354-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67354-159">Version of the device configuration.</span></span> <span data-ttu-id="67354-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="67354-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="67354-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="67354-161">passwordRequired</span></span>|<span data-ttu-id="67354-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="67354-162">Boolean</span></span>|<span data-ttu-id="67354-163">Exige uma senha para desbloquear o dispositivo Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="67354-163">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="67354-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="67354-164">passwordBlockSimple</span></span>|<span data-ttu-id="67354-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="67354-165">Boolean</span></span>|<span data-ttu-id="67354-166">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="67354-166">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="67354-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="67354-167">passwordMinimumLength</span></span>|<span data-ttu-id="67354-168">Int32</span><span class="sxs-lookup"><span data-stu-id="67354-168">Int32</span></span>|<span data-ttu-id="67354-169">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="67354-169">Minimum password length.</span></span> <span data-ttu-id="67354-170">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="67354-170">Valid values 4 to 16</span></span>|
|<span data-ttu-id="67354-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="67354-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="67354-172">Int32</span><span class="sxs-lookup"><span data-stu-id="67354-172">Int32</span></span>|<span data-ttu-id="67354-173">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="67354-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="67354-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="67354-174">passwordRequiredType</span></span>|[<span data-ttu-id="67354-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="67354-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="67354-176">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="67354-176">The required password type.</span></span> <span data-ttu-id="67354-177">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="67354-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="67354-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="67354-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="67354-179">Int32</span><span class="sxs-lookup"><span data-stu-id="67354-179">Int32</span></span>|<span data-ttu-id="67354-180">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="67354-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="67354-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="67354-181">passwordExpirationDays</span></span>|<span data-ttu-id="67354-182">Int32</span><span class="sxs-lookup"><span data-stu-id="67354-182">Int32</span></span>|<span data-ttu-id="67354-183">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="67354-183">Number of days before password expiration.</span></span> <span data-ttu-id="67354-184">Valores válidos de 1 a 255</span><span class="sxs-lookup"><span data-stu-id="67354-184">Valid values 1 to 255</span></span>|
|<span data-ttu-id="67354-185">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="67354-185">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="67354-186">Int32</span><span class="sxs-lookup"><span data-stu-id="67354-186">Int32</span></span>|<span data-ttu-id="67354-187">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="67354-187">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="67354-188">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="67354-188">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="67354-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="67354-189">Boolean</span></span>|<span data-ttu-id="67354-190">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="67354-190">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="67354-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="67354-191">osMinimumVersion</span></span>|<span data-ttu-id="67354-192">String</span><span class="sxs-lookup"><span data-stu-id="67354-192">String</span></span>|<span data-ttu-id="67354-193">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="67354-193">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="67354-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="67354-194">osMaximumVersion</span></span>|<span data-ttu-id="67354-195">String</span><span class="sxs-lookup"><span data-stu-id="67354-195">String</span></span>|<span data-ttu-id="67354-196">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="67354-196">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="67354-197">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="67354-197">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="67354-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="67354-198">Boolean</span></span>|<span data-ttu-id="67354-199">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="67354-199">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="67354-200">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="67354-200">bitLockerEnabled</span></span>|<span data-ttu-id="67354-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="67354-201">Boolean</span></span>|<span data-ttu-id="67354-202">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="67354-202">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="67354-203">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="67354-203">secureBootEnabled</span></span>|<span data-ttu-id="67354-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="67354-204">Boolean</span></span>|<span data-ttu-id="67354-205">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="67354-205">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="67354-206">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="67354-206">codeIntegrityEnabled</span></span>|<span data-ttu-id="67354-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="67354-207">Boolean</span></span>|<span data-ttu-id="67354-208">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="67354-208">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="67354-209">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="67354-209">storageRequireEncryption</span></span>|<span data-ttu-id="67354-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="67354-210">Boolean</span></span>|<span data-ttu-id="67354-211">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="67354-211">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="67354-212">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="67354-212">activeFirewallRequired</span></span>|<span data-ttu-id="67354-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="67354-213">Boolean</span></span>|<span data-ttu-id="67354-214">Exigir um firewall ativas em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="67354-214">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="67354-215">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="67354-215">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="67354-216">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="67354-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="67354-217">O sistema operacional válido criar intervalos em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="67354-217">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="67354-218">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="67354-218">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="67354-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="67354-219">Response</span></span>
<span data-ttu-id="67354-220">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67354-220">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67354-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67354-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="67354-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67354-222">Request</span></span>
<span data-ttu-id="67354-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67354-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1158

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="67354-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="67354-224">Response</span></span>
<span data-ttu-id="67354-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67354-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1330

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "3d4237b0-37b0-3d42-b037-423db037423d",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```




