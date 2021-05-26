---
title: Criar aospDeviceOwnerCompliancePolicy
description: Crie um novo objeto aospDeviceOwnerCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02e80fa9e55b7b44751fb426cc12f8360045c80d
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665679"
---
# <a name="create-aospdeviceownercompliancepolicy"></a><span data-ttu-id="aaec2-103">Criar aospDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="aaec2-103">Create aospDeviceOwnerCompliancePolicy</span></span>

<span data-ttu-id="aaec2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaec2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aaec2-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aaec2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aaec2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aaec2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaec2-107">Crie um [novo objeto aospDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aaec2-107">Create a new [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aaec2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aaec2-108">Prerequisites</span></span>
<span data-ttu-id="aaec2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaec2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaec2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aaec2-111">Permission type</span></span>|<span data-ttu-id="aaec2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aaec2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaec2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aaec2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aaec2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaec2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aaec2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aaec2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaec2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aaec2-116">Not supported.</span></span>|
|<span data-ttu-id="aaec2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aaec2-117">Application</span></span>|<span data-ttu-id="aaec2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaec2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaec2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aaec2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="aaec2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aaec2-120">Request headers</span></span>
|<span data-ttu-id="aaec2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aaec2-121">Header</span></span>|<span data-ttu-id="aaec2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aaec2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaec2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aaec2-123">Authorization</span></span>|<span data-ttu-id="aaec2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aaec2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaec2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aaec2-125">Accept</span></span>|<span data-ttu-id="aaec2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aaec2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaec2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aaec2-127">Request body</span></span>
<span data-ttu-id="aaec2-128">No corpo da solicitação, fornece uma representação JSON para o objeto aospDeviceOwnerCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="aaec2-128">In the request body, supply a JSON representation for the aospDeviceOwnerCompliancePolicy object.</span></span>

<span data-ttu-id="aaec2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o aospDeviceOwnerCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="aaec2-129">The following table shows the properties that are required when you create the aospDeviceOwnerCompliancePolicy.</span></span>

|<span data-ttu-id="aaec2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aaec2-130">Property</span></span>|<span data-ttu-id="aaec2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aaec2-131">Type</span></span>|<span data-ttu-id="aaec2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aaec2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaec2-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aaec2-133">roleScopeTagIds</span></span>|<span data-ttu-id="aaec2-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aaec2-134">String collection</span></span>|<span data-ttu-id="aaec2-135">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="aaec2-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aaec2-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aaec2-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aaec2-137">id</span><span class="sxs-lookup"><span data-stu-id="aaec2-137">id</span></span>|<span data-ttu-id="aaec2-138">String</span><span class="sxs-lookup"><span data-stu-id="aaec2-138">String</span></span>|<span data-ttu-id="aaec2-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aaec2-139">Key of the entity.</span></span> <span data-ttu-id="aaec2-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aaec2-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aaec2-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aaec2-141">createdDateTime</span></span>|<span data-ttu-id="aaec2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaec2-142">DateTimeOffset</span></span>|<span data-ttu-id="aaec2-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="aaec2-143">DateTime the object was created.</span></span> <span data-ttu-id="aaec2-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aaec2-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aaec2-145">descrição</span><span class="sxs-lookup"><span data-stu-id="aaec2-145">description</span></span>|<span data-ttu-id="aaec2-146">String</span><span class="sxs-lookup"><span data-stu-id="aaec2-146">String</span></span>|<span data-ttu-id="aaec2-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aaec2-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aaec2-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aaec2-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aaec2-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aaec2-149">lastModifiedDateTime</span></span>|<span data-ttu-id="aaec2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaec2-150">DateTimeOffset</span></span>|<span data-ttu-id="aaec2-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="aaec2-151">DateTime the object was last modified.</span></span> <span data-ttu-id="aaec2-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aaec2-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aaec2-153">displayName</span><span class="sxs-lookup"><span data-stu-id="aaec2-153">displayName</span></span>|<span data-ttu-id="aaec2-154">String</span><span class="sxs-lookup"><span data-stu-id="aaec2-154">String</span></span>|<span data-ttu-id="aaec2-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aaec2-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aaec2-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aaec2-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aaec2-157">version</span><span class="sxs-lookup"><span data-stu-id="aaec2-157">version</span></span>|<span data-ttu-id="aaec2-158">Int32</span><span class="sxs-lookup"><span data-stu-id="aaec2-158">Int32</span></span>|<span data-ttu-id="aaec2-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aaec2-159">Version of the device configuration.</span></span> <span data-ttu-id="aaec2-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aaec2-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aaec2-161">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="aaec2-161">osMinimumVersion</span></span>|<span data-ttu-id="aaec2-162">String</span><span class="sxs-lookup"><span data-stu-id="aaec2-162">String</span></span>|<span data-ttu-id="aaec2-163">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="aaec2-163">Minimum Android version.</span></span>|
|<span data-ttu-id="aaec2-164">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="aaec2-164">osMaximumVersion</span></span>|<span data-ttu-id="aaec2-165">String</span><span class="sxs-lookup"><span data-stu-id="aaec2-165">String</span></span>|<span data-ttu-id="aaec2-166">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="aaec2-166">Maximum Android version.</span></span>|
|<span data-ttu-id="aaec2-167">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="aaec2-167">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="aaec2-168">String</span><span class="sxs-lookup"><span data-stu-id="aaec2-168">String</span></span>|<span data-ttu-id="aaec2-169">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="aaec2-169">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="aaec2-170">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="aaec2-170">passwordRequired</span></span>|<span data-ttu-id="aaec2-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="aaec2-171">Boolean</span></span>|<span data-ttu-id="aaec2-172">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aaec2-172">Require a password to unlock device.</span></span>|
|<span data-ttu-id="aaec2-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="aaec2-173">passwordRequiredType</span></span>|[<span data-ttu-id="aaec2-174">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="aaec2-174">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="aaec2-175">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="aaec2-175">Type of characters in password.</span></span> <span data-ttu-id="aaec2-176">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="aaec2-176">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="aaec2-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="aaec2-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="aaec2-178">Int32</span><span class="sxs-lookup"><span data-stu-id="aaec2-178">Int32</span></span>|<span data-ttu-id="aaec2-179">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="aaec2-179">Minutes of inactivity before a password is required.</span></span> <span data-ttu-id="aaec2-180">Valores válidos de 1 a 8640</span><span class="sxs-lookup"><span data-stu-id="aaec2-180">Valid values 1 to 8640</span></span>|
|<span data-ttu-id="aaec2-181">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="aaec2-181">passwordMinimumLength</span></span>|<span data-ttu-id="aaec2-182">Int32</span><span class="sxs-lookup"><span data-stu-id="aaec2-182">Int32</span></span>|<span data-ttu-id="aaec2-183">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="aaec2-183">Minimum password length.</span></span> <span data-ttu-id="aaec2-184">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="aaec2-184">Valid values 4 to 16</span></span>|
|<span data-ttu-id="aaec2-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="aaec2-185">storageRequireEncryption</span></span>|<span data-ttu-id="aaec2-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="aaec2-186">Boolean</span></span>|<span data-ttu-id="aaec2-187">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="aaec2-187">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="aaec2-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaec2-188">Response</span></span>
<span data-ttu-id="aaec2-189">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aaec2-189">If successful, this method returns a `201 Created` response code and a [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaec2-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aaec2-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaec2-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aaec2-191">Request</span></span>
<span data-ttu-id="aaec2-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aaec2-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 593

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumLength": 5,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="aaec2-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaec2-193">Response</span></span>
<span data-ttu-id="aaec2-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aaec2-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 765

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "0837b942-b942-0837-42b9-370842b93708",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumLength": 5,
  "storageRequireEncryption": true
}
```




