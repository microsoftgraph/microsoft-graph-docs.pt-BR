---
title: Atualizar windowsPhone81CompliancePolicy
description: Atualizar as propriedades de um objeto windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e039a6b9693b4507161fc57cfc4ad646b3c06a22
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264285"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="8e77f-103">Atualizar windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8e77f-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="8e77f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e77f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e77f-105">Atualizar as propriedades de um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8e77f-105">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e77f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e77f-106">Prerequisites</span></span>
<span data-ttu-id="8e77f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e77f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8e77f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e77f-109">Permission type</span></span>|<span data-ttu-id="8e77f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e77f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e77f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e77f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e77f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e77f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e77f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e77f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e77f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e77f-114">Not supported.</span></span>|
|<span data-ttu-id="8e77f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e77f-115">Application</span></span>|<span data-ttu-id="8e77f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e77f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e77f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e77f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="8e77f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e77f-118">Request headers</span></span>
|<span data-ttu-id="8e77f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e77f-119">Header</span></span>|<span data-ttu-id="8e77f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8e77f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e77f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e77f-121">Authorization</span></span>|<span data-ttu-id="8e77f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e77f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e77f-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e77f-123">Accept</span></span>|<span data-ttu-id="8e77f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8e77f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e77f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e77f-125">Request body</span></span>
<span data-ttu-id="8e77f-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8e77f-126">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="8e77f-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8e77f-127">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="8e77f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e77f-128">Property</span></span>|<span data-ttu-id="8e77f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e77f-129">Type</span></span>|<span data-ttu-id="8e77f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e77f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e77f-131">id</span><span class="sxs-lookup"><span data-stu-id="8e77f-131">id</span></span>|<span data-ttu-id="8e77f-132">String</span><span class="sxs-lookup"><span data-stu-id="8e77f-132">String</span></span>|<span data-ttu-id="8e77f-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8e77f-133">Key of the entity.</span></span> <span data-ttu-id="8e77f-134">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8e77f-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e77f-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e77f-135">createdDateTime</span></span>|<span data-ttu-id="8e77f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e77f-136">DateTimeOffset</span></span>|<span data-ttu-id="8e77f-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8e77f-137">DateTime the object was created.</span></span> <span data-ttu-id="8e77f-138">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8e77f-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e77f-139">description</span><span class="sxs-lookup"><span data-stu-id="8e77f-139">description</span></span>|<span data-ttu-id="8e77f-140">String</span><span class="sxs-lookup"><span data-stu-id="8e77f-140">String</span></span>|<span data-ttu-id="8e77f-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e77f-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8e77f-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8e77f-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e77f-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e77f-143">lastModifiedDateTime</span></span>|<span data-ttu-id="8e77f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e77f-144">DateTimeOffset</span></span>|<span data-ttu-id="8e77f-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8e77f-145">DateTime the object was last modified.</span></span> <span data-ttu-id="8e77f-146">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8e77f-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e77f-147">displayName</span><span class="sxs-lookup"><span data-stu-id="8e77f-147">displayName</span></span>|<span data-ttu-id="8e77f-148">String</span><span class="sxs-lookup"><span data-stu-id="8e77f-148">String</span></span>|<span data-ttu-id="8e77f-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e77f-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8e77f-150">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8e77f-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e77f-151">version</span><span class="sxs-lookup"><span data-stu-id="8e77f-151">version</span></span>|<span data-ttu-id="8e77f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8e77f-152">Int32</span></span>|<span data-ttu-id="8e77f-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e77f-153">Version of the device configuration.</span></span> <span data-ttu-id="8e77f-154">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8e77f-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e77f-155">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="8e77f-155">passwordBlockSimple</span></span>|<span data-ttu-id="8e77f-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e77f-156">Boolean</span></span>|<span data-ttu-id="8e77f-157">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="8e77f-157">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="8e77f-158">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8e77f-158">passwordExpirationDays</span></span>|<span data-ttu-id="8e77f-159">Int32</span><span class="sxs-lookup"><span data-stu-id="8e77f-159">Int32</span></span>|<span data-ttu-id="8e77f-160">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="8e77f-160">Number of days before the password expires.</span></span>|
|<span data-ttu-id="8e77f-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8e77f-161">passwordMinimumLength</span></span>|<span data-ttu-id="8e77f-162">Int32</span><span class="sxs-lookup"><span data-stu-id="8e77f-162">Int32</span></span>|<span data-ttu-id="8e77f-163">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="8e77f-163">Minimum length of passwords.</span></span>|
|<span data-ttu-id="8e77f-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8e77f-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8e77f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8e77f-165">Int32</span></span>|<span data-ttu-id="8e77f-166">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="8e77f-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="8e77f-167">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8e77f-167">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8e77f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="8e77f-168">Int32</span></span>|<span data-ttu-id="8e77f-169">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="8e77f-169">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8e77f-170">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8e77f-170">passwordRequiredType</span></span>|[<span data-ttu-id="8e77f-171">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8e77f-171">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="8e77f-172">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="8e77f-172">The required password type.</span></span> <span data-ttu-id="8e77f-173">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="8e77f-173">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8e77f-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8e77f-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8e77f-175">Int32</span><span class="sxs-lookup"><span data-stu-id="8e77f-175">Int32</span></span>|<span data-ttu-id="8e77f-176">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="8e77f-176">Number of previous passwords to block.</span></span> <span data-ttu-id="8e77f-177">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="8e77f-177">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8e77f-178">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8e77f-178">passwordRequired</span></span>|<span data-ttu-id="8e77f-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e77f-179">Boolean</span></span>|<span data-ttu-id="8e77f-180">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="8e77f-180">Whether or not to require a password.</span></span>|
|<span data-ttu-id="8e77f-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8e77f-181">osMinimumVersion</span></span>|<span data-ttu-id="8e77f-182">String</span><span class="sxs-lookup"><span data-stu-id="8e77f-182">String</span></span>|<span data-ttu-id="8e77f-183">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="8e77f-183">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="8e77f-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8e77f-184">osMaximumVersion</span></span>|<span data-ttu-id="8e77f-185">String</span><span class="sxs-lookup"><span data-stu-id="8e77f-185">String</span></span>|<span data-ttu-id="8e77f-186">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="8e77f-186">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="8e77f-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="8e77f-187">storageRequireEncryption</span></span>|<span data-ttu-id="8e77f-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e77f-188">Boolean</span></span>|<span data-ttu-id="8e77f-189">Exige criptografia em dispositivos Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="8e77f-189">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="8e77f-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e77f-190">Response</span></span>
<span data-ttu-id="8e77f-191">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e77f-191">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e77f-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e77f-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e77f-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e77f-193">Request</span></span>
<span data-ttu-id="8e77f-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e77f-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e77f-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e77f-195">Response</span></span>
<span data-ttu-id="8e77f-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e77f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



