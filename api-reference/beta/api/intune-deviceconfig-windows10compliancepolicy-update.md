---
title: Atualizar windows10CompliancePolicy
description: Atualiza as propriedades de um objeto windows10CompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a333bfe10ded7168b873cd226fe3aa9d7111cc15
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42481835"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="b1d5c-103">Atualizar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b1d5c-103">Update windows10CompliancePolicy</span></span>

<span data-ttu-id="b1d5c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b1d5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1d5c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1d5c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1d5c-107">Atualiza as propriedades de um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1d5c-107">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1d5c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1d5c-108">Prerequisites</span></span>
<span data-ttu-id="b1d5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1d5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1d5c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1d5c-111">Permission type</span></span>|<span data-ttu-id="b1d5c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b1d5c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1d5c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1d5c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1d5c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1d5c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1d5c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1d5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1d5c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-116">Not supported.</span></span>|
|<span data-ttu-id="b1d5c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1d5c-117">Application</span></span>|<span data-ttu-id="b1d5c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1d5c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1d5c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1d5c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b1d5c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1d5c-120">Request headers</span></span>
|<span data-ttu-id="b1d5c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1d5c-121">Header</span></span>|<span data-ttu-id="b1d5c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b1d5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1d5c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1d5c-123">Authorization</span></span>|<span data-ttu-id="b1d5c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1d5c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1d5c-125">Accept</span></span>|<span data-ttu-id="b1d5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1d5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1d5c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1d5c-127">Request body</span></span>
<span data-ttu-id="b1d5c-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1d5c-128">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="b1d5c-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1d5c-129">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="b1d5c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1d5c-130">Property</span></span>|<span data-ttu-id="b1d5c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1d5c-131">Type</span></span>|<span data-ttu-id="b1d5c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1d5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1d5c-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b1d5c-133">roleScopeTagIds</span></span>|<span data-ttu-id="b1d5c-134">String collection</span><span class="sxs-lookup"><span data-stu-id="b1d5c-134">String collection</span></span>|<span data-ttu-id="b1d5c-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b1d5c-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1d5c-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1d5c-137">id</span><span class="sxs-lookup"><span data-stu-id="b1d5c-137">id</span></span>|<span data-ttu-id="b1d5c-138">String</span><span class="sxs-lookup"><span data-stu-id="b1d5c-138">String</span></span>|<span data-ttu-id="b1d5c-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-139">Key of the entity.</span></span> <span data-ttu-id="b1d5c-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1d5c-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1d5c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1d5c-141">createdDateTime</span></span>|<span data-ttu-id="b1d5c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1d5c-142">DateTimeOffset</span></span>|<span data-ttu-id="b1d5c-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-143">DateTime the object was created.</span></span> <span data-ttu-id="b1d5c-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1d5c-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1d5c-145">description</span><span class="sxs-lookup"><span data-stu-id="b1d5c-145">description</span></span>|<span data-ttu-id="b1d5c-146">String</span><span class="sxs-lookup"><span data-stu-id="b1d5c-146">String</span></span>|<span data-ttu-id="b1d5c-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b1d5c-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1d5c-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1d5c-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1d5c-149">lastModifiedDateTime</span></span>|<span data-ttu-id="b1d5c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1d5c-150">DateTimeOffset</span></span>|<span data-ttu-id="b1d5c-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-151">DateTime the object was last modified.</span></span> <span data-ttu-id="b1d5c-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1d5c-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1d5c-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b1d5c-153">displayName</span></span>|<span data-ttu-id="b1d5c-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1d5c-154">String</span></span>|<span data-ttu-id="b1d5c-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b1d5c-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1d5c-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1d5c-157">version</span><span class="sxs-lookup"><span data-stu-id="b1d5c-157">version</span></span>|<span data-ttu-id="b1d5c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b1d5c-158">Int32</span></span>|<span data-ttu-id="b1d5c-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-159">Version of the device configuration.</span></span> <span data-ttu-id="b1d5c-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1d5c-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1d5c-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b1d5c-161">passwordRequired</span></span>|<span data-ttu-id="b1d5c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-162">Boolean</span></span>|<span data-ttu-id="b1d5c-163">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="b1d5c-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b1d5c-164">passwordBlockSimple</span></span>|<span data-ttu-id="b1d5c-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-165">Boolean</span></span>|<span data-ttu-id="b1d5c-166">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="b1d5c-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="b1d5c-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="b1d5c-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-168">Boolean</span></span>|<span data-ttu-id="b1d5c-169">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="b1d5c-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b1d5c-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b1d5c-171">Int32</span><span class="sxs-lookup"><span data-stu-id="b1d5c-171">Int32</span></span>|<span data-ttu-id="b1d5c-172">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b1d5c-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b1d5c-173">passwordExpirationDays</span></span>|<span data-ttu-id="b1d5c-174">Int32</span><span class="sxs-lookup"><span data-stu-id="b1d5c-174">Int32</span></span>|<span data-ttu-id="b1d5c-175">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-175">The password expiration in days.</span></span>|
|<span data-ttu-id="b1d5c-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b1d5c-176">passwordMinimumLength</span></span>|<span data-ttu-id="b1d5c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b1d5c-177">Int32</span></span>|<span data-ttu-id="b1d5c-178">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-178">The minimum password length.</span></span>|
|<span data-ttu-id="b1d5c-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b1d5c-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b1d5c-180">Int32</span><span class="sxs-lookup"><span data-stu-id="b1d5c-180">Int32</span></span>|<span data-ttu-id="b1d5c-181">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b1d5c-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b1d5c-182">passwordRequiredType</span></span>|[<span data-ttu-id="b1d5c-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b1d5c-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b1d5c-184">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-184">The required password type.</span></span> <span data-ttu-id="b1d5c-185">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b1d5c-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b1d5c-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b1d5c-187">Int32</span><span class="sxs-lookup"><span data-stu-id="b1d5c-187">Int32</span></span>|<span data-ttu-id="b1d5c-188">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="b1d5c-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="b1d5c-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="b1d5c-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-190">Boolean</span></span>|<span data-ttu-id="b1d5c-191">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="b1d5c-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b1d5c-192">osMinimumVersion</span></span>|<span data-ttu-id="b1d5c-193">String</span><span class="sxs-lookup"><span data-stu-id="b1d5c-193">String</span></span>|<span data-ttu-id="b1d5c-194">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="b1d5c-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b1d5c-195">osMaximumVersion</span></span>|<span data-ttu-id="b1d5c-196">String</span><span class="sxs-lookup"><span data-stu-id="b1d5c-196">String</span></span>|<span data-ttu-id="b1d5c-197">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="b1d5c-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b1d5c-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="b1d5c-199">String</span><span class="sxs-lookup"><span data-stu-id="b1d5c-199">String</span></span>|<span data-ttu-id="b1d5c-200">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="b1d5c-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b1d5c-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="b1d5c-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1d5c-202">String</span></span>|<span data-ttu-id="b1d5c-203">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="b1d5c-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="b1d5c-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="b1d5c-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-205">Boolean</span></span>|<span data-ttu-id="b1d5c-206">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="b1d5c-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="b1d5c-207">bitLockerEnabled</span></span>|<span data-ttu-id="b1d5c-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-208">Boolean</span></span>|<span data-ttu-id="b1d5c-209">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="b1d5c-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="b1d5c-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="b1d5c-210">secureBootEnabled</span></span>|<span data-ttu-id="b1d5c-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-211">Boolean</span></span>|<span data-ttu-id="b1d5c-212">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="b1d5c-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="b1d5c-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="b1d5c-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-214">Boolean</span></span>|<span data-ttu-id="b1d5c-215">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="b1d5c-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b1d5c-216">storageRequireEncryption</span></span>|<span data-ttu-id="b1d5c-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-217">Boolean</span></span>|<span data-ttu-id="b1d5c-218">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="b1d5c-219">Propriedades activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="b1d5c-219">activeFirewallRequired</span></span>|<span data-ttu-id="b1d5c-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-220">Boolean</span></span>|<span data-ttu-id="b1d5c-221">Exigir firewall ativo em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="b1d5c-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="b1d5c-222">defenderEnabled</span></span>|<span data-ttu-id="b1d5c-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-223">Boolean</span></span>|<span data-ttu-id="b1d5c-224">Requer o Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="b1d5c-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="b1d5c-225">defenderVersion</span></span>|<span data-ttu-id="b1d5c-226">String</span><span class="sxs-lookup"><span data-stu-id="b1d5c-226">String</span></span>|<span data-ttu-id="b1d5c-227">Requer a versão mínima do Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="b1d5c-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="b1d5c-228">signatureOutOfDate</span></span>|<span data-ttu-id="b1d5c-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-229">Boolean</span></span>|<span data-ttu-id="b1d5c-230">Requer que a assinatura antimalware do Windows Defender esteja atualizada em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="b1d5c-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="b1d5c-231">rtpEnabled</span></span>|<span data-ttu-id="b1d5c-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-232">Boolean</span></span>|<span data-ttu-id="b1d5c-233">Requer a proteção em tempo real do Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="b1d5c-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="b1d5c-234">antivirusRequired</span></span>|<span data-ttu-id="b1d5c-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-235">Boolean</span></span>|<span data-ttu-id="b1d5c-236">Exigir que qualquer solução antivírus registrada com o Windows Decurity Center seja ativada e monitorando (por exemplo, Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="b1d5c-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="b1d5c-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="b1d5c-237">antiSpywareRequired</span></span>|<span data-ttu-id="b1d5c-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-238">Boolean</span></span>|<span data-ttu-id="b1d5c-239">Exija que qualquer solução AntiSpyware registrada com o Windows Decurity Center seja ativada e monitoramento (por exemplo, Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="b1d5c-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="b1d5c-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="b1d5c-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="b1d5c-241">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="b1d5c-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="b1d5c-242">Os intervalos válidos da compilação do sistema operacional em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="b1d5c-243">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b1d5c-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b1d5c-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="b1d5c-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-245">Boolean</span></span>|<span data-ttu-id="b1d5c-246">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="b1d5c-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b1d5c-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b1d5c-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="b1d5c-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b1d5c-249">Requer nível mínimo de risco de proteção contra ameaças ao dispositivo para relatar não conformidade.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b1d5c-250">Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b1d5c-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="b1d5c-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="b1d5c-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-252">Boolean</span></span>|<span data-ttu-id="b1d5c-253">Exigir que o estado de conformidade do SCCM seja considerado para o estado de conformidade do Intune.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="b1d5c-254">tpmRequired</span><span class="sxs-lookup"><span data-stu-id="b1d5c-254">tpmRequired</span></span>|<span data-ttu-id="b1d5c-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d5c-255">Boolean</span></span>|<span data-ttu-id="b1d5c-256">Requer o módulo de plataforma confiável (TPM) para estar presente.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-256">Require Trusted Platform Module(TPM) to be present.</span></span>|



## <a name="response"></a><span data-ttu-id="b1d5c-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1d5c-257">Response</span></span>
<span data-ttu-id="b1d5c-258">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-258">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1d5c-259">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1d5c-259">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1d5c-260">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1d5c-260">Request</span></span>
<span data-ttu-id="b1d5c-261">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-261">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1690

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true
}
```

### <a name="response"></a><span data-ttu-id="b1d5c-262">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1d5c-262">Response</span></span>
<span data-ttu-id="b1d5c-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1d5c-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1862

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true
}
```





