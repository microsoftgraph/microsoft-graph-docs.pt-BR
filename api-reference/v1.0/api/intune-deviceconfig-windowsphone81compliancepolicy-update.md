---
title: Atualizar windowsPhone81CompliancePolicy
description: Atualizar as propriedades de um objeto windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 840504bf54f70e6a15cbf486946247fa33c0b3b5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520009"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="f3935-103">Atualizar windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f3935-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="f3935-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3935-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3935-105">Atualizar as propriedades de um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f3935-105">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3935-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f3935-106">Prerequisites</span></span>
<span data-ttu-id="f3935-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3935-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3935-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3935-109">Permission type</span></span>|<span data-ttu-id="f3935-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f3935-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3935-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3935-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3935-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3935-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3935-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3935-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3935-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3935-114">Not supported.</span></span>|
|<span data-ttu-id="f3935-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3935-115">Application</span></span>|<span data-ttu-id="f3935-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3935-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3935-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3935-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="f3935-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3935-118">Request headers</span></span>
|<span data-ttu-id="f3935-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3935-119">Header</span></span>|<span data-ttu-id="f3935-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f3935-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3935-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3935-121">Authorization</span></span>|<span data-ttu-id="f3935-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3935-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3935-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f3935-123">Accept</span></span>|<span data-ttu-id="f3935-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f3935-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3935-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3935-125">Request body</span></span>
<span data-ttu-id="f3935-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f3935-126">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="f3935-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f3935-127">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="f3935-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3935-128">Property</span></span>|<span data-ttu-id="f3935-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3935-129">Type</span></span>|<span data-ttu-id="f3935-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3935-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3935-131">id</span><span class="sxs-lookup"><span data-stu-id="f3935-131">id</span></span>|<span data-ttu-id="f3935-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3935-132">String</span></span>|<span data-ttu-id="f3935-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f3935-133">Key of the entity.</span></span> <span data-ttu-id="f3935-134">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f3935-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f3935-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3935-135">createdDateTime</span></span>|<span data-ttu-id="f3935-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3935-136">DateTimeOffset</span></span>|<span data-ttu-id="f3935-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f3935-137">DateTime the object was created.</span></span> <span data-ttu-id="f3935-138">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f3935-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f3935-139">description</span><span class="sxs-lookup"><span data-stu-id="f3935-139">description</span></span>|<span data-ttu-id="f3935-140">String</span><span class="sxs-lookup"><span data-stu-id="f3935-140">String</span></span>|<span data-ttu-id="f3935-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3935-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f3935-142">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f3935-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f3935-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3935-143">lastModifiedDateTime</span></span>|<span data-ttu-id="f3935-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3935-144">DateTimeOffset</span></span>|<span data-ttu-id="f3935-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f3935-145">DateTime the object was last modified.</span></span> <span data-ttu-id="f3935-146">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f3935-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f3935-147">displayName</span><span class="sxs-lookup"><span data-stu-id="f3935-147">displayName</span></span>|<span data-ttu-id="f3935-148">String</span><span class="sxs-lookup"><span data-stu-id="f3935-148">String</span></span>|<span data-ttu-id="f3935-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3935-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f3935-150">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f3935-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f3935-151">version</span><span class="sxs-lookup"><span data-stu-id="f3935-151">version</span></span>|<span data-ttu-id="f3935-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f3935-152">Int32</span></span>|<span data-ttu-id="f3935-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3935-153">Version of the device configuration.</span></span> <span data-ttu-id="f3935-154">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f3935-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f3935-155">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f3935-155">passwordBlockSimple</span></span>|<span data-ttu-id="f3935-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3935-156">Boolean</span></span>|<span data-ttu-id="f3935-157">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="f3935-157">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="f3935-158">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f3935-158">passwordExpirationDays</span></span>|<span data-ttu-id="f3935-159">Int32</span><span class="sxs-lookup"><span data-stu-id="f3935-159">Int32</span></span>|<span data-ttu-id="f3935-160">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="f3935-160">Number of days before the password expires.</span></span>|
|<span data-ttu-id="f3935-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f3935-161">passwordMinimumLength</span></span>|<span data-ttu-id="f3935-162">Int32</span><span class="sxs-lookup"><span data-stu-id="f3935-162">Int32</span></span>|<span data-ttu-id="f3935-163">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="f3935-163">Minimum length of passwords.</span></span>|
|<span data-ttu-id="f3935-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f3935-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f3935-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f3935-165">Int32</span></span>|<span data-ttu-id="f3935-166">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="f3935-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f3935-167">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f3935-167">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f3935-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f3935-168">Int32</span></span>|<span data-ttu-id="f3935-169">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="f3935-169">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f3935-170">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f3935-170">passwordRequiredType</span></span>|[<span data-ttu-id="f3935-171">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f3935-171">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f3935-172">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="f3935-172">The required password type.</span></span> <span data-ttu-id="f3935-173">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f3935-173">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f3935-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f3935-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f3935-175">Int32</span><span class="sxs-lookup"><span data-stu-id="f3935-175">Int32</span></span>|<span data-ttu-id="f3935-176">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="f3935-176">Number of previous passwords to block.</span></span> <span data-ttu-id="f3935-177">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="f3935-177">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f3935-178">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f3935-178">passwordRequired</span></span>|<span data-ttu-id="f3935-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3935-179">Boolean</span></span>|<span data-ttu-id="f3935-180">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="f3935-180">Whether or not to require a password.</span></span>|
|<span data-ttu-id="f3935-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f3935-181">osMinimumVersion</span></span>|<span data-ttu-id="f3935-182">String</span><span class="sxs-lookup"><span data-stu-id="f3935-182">String</span></span>|<span data-ttu-id="f3935-183">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f3935-183">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="f3935-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f3935-184">osMaximumVersion</span></span>|<span data-ttu-id="f3935-185">String</span><span class="sxs-lookup"><span data-stu-id="f3935-185">String</span></span>|<span data-ttu-id="f3935-186">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f3935-186">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="f3935-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f3935-187">storageRequireEncryption</span></span>|<span data-ttu-id="f3935-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3935-188">Boolean</span></span>|<span data-ttu-id="f3935-189">Exige criptografia em dispositivos Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f3935-189">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="f3935-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3935-190">Response</span></span>
<span data-ttu-id="f3935-191">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3935-191">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3935-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3935-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3935-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3935-193">Request</span></span>
<span data-ttu-id="f3935-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3935-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 607

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="f3935-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3935-195">Response</span></span>
<span data-ttu-id="f3935-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3935-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 779

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```



