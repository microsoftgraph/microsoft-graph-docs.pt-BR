---
title: Criar windowsPhone81CompliancePolicy
description: Cria um novo objeto windowsPhone81CompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ebb179f582abe617b931ec1fb83bc1b92d7a983f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513798"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="53913-103">Criar windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="53913-103">Create windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="53913-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53913-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53913-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53913-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53913-106">Cria um novo objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="53913-106">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53913-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53913-107">Prerequisites</span></span>
<span data-ttu-id="53913-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53913-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53913-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53913-110">Permission type</span></span>|<span data-ttu-id="53913-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="53913-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53913-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53913-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53913-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53913-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53913-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53913-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53913-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53913-115">Not supported.</span></span>|
|<span data-ttu-id="53913-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53913-116">Application</span></span>|<span data-ttu-id="53913-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53913-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53913-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53913-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="53913-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53913-119">Request headers</span></span>
|<span data-ttu-id="53913-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53913-120">Header</span></span>|<span data-ttu-id="53913-121">Valor</span><span class="sxs-lookup"><span data-stu-id="53913-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53913-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="53913-122">Authorization</span></span>|<span data-ttu-id="53913-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53913-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53913-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53913-124">Accept</span></span>|<span data-ttu-id="53913-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53913-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53913-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53913-126">Request body</span></span>
<span data-ttu-id="53913-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="53913-127">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="53913-128">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsPhone81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="53913-128">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="53913-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53913-129">Property</span></span>|<span data-ttu-id="53913-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="53913-130">Type</span></span>|<span data-ttu-id="53913-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="53913-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53913-132">id</span><span class="sxs-lookup"><span data-stu-id="53913-132">id</span></span>|<span data-ttu-id="53913-133">String</span><span class="sxs-lookup"><span data-stu-id="53913-133">String</span></span>|<span data-ttu-id="53913-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="53913-134">Key of the entity.</span></span> <span data-ttu-id="53913-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="53913-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="53913-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53913-136">createdDateTime</span></span>|<span data-ttu-id="53913-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53913-137">DateTimeOffset</span></span>|<span data-ttu-id="53913-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="53913-138">DateTime the object was created.</span></span> <span data-ttu-id="53913-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="53913-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="53913-140">description</span><span class="sxs-lookup"><span data-stu-id="53913-140">description</span></span>|<span data-ttu-id="53913-141">String</span><span class="sxs-lookup"><span data-stu-id="53913-141">String</span></span>|<span data-ttu-id="53913-142">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53913-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="53913-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="53913-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="53913-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53913-144">lastModifiedDateTime</span></span>|<span data-ttu-id="53913-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53913-145">DateTimeOffset</span></span>|<span data-ttu-id="53913-146">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="53913-146">DateTime the object was last modified.</span></span> <span data-ttu-id="53913-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="53913-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="53913-148">displayName</span><span class="sxs-lookup"><span data-stu-id="53913-148">displayName</span></span>|<span data-ttu-id="53913-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53913-149">String</span></span>|<span data-ttu-id="53913-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53913-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="53913-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="53913-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="53913-152">version</span><span class="sxs-lookup"><span data-stu-id="53913-152">version</span></span>|<span data-ttu-id="53913-153">Int32</span><span class="sxs-lookup"><span data-stu-id="53913-153">Int32</span></span>|<span data-ttu-id="53913-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53913-154">Version of the device configuration.</span></span> <span data-ttu-id="53913-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="53913-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="53913-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="53913-156">passwordBlockSimple</span></span>|<span data-ttu-id="53913-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="53913-157">Boolean</span></span>|<span data-ttu-id="53913-158">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="53913-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="53913-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="53913-159">passwordExpirationDays</span></span>|<span data-ttu-id="53913-160">Int32</span><span class="sxs-lookup"><span data-stu-id="53913-160">Int32</span></span>|<span data-ttu-id="53913-161">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="53913-161">Number of days before the password expires.</span></span>|
|<span data-ttu-id="53913-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="53913-162">passwordMinimumLength</span></span>|<span data-ttu-id="53913-163">Int32</span><span class="sxs-lookup"><span data-stu-id="53913-163">Int32</span></span>|<span data-ttu-id="53913-164">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="53913-164">Minimum length of passwords.</span></span>|
|<span data-ttu-id="53913-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="53913-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="53913-166">Int32</span><span class="sxs-lookup"><span data-stu-id="53913-166">Int32</span></span>|<span data-ttu-id="53913-167">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="53913-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="53913-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="53913-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="53913-169">Int32</span><span class="sxs-lookup"><span data-stu-id="53913-169">Int32</span></span>|<span data-ttu-id="53913-170">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="53913-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="53913-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="53913-171">passwordRequiredType</span></span>|[<span data-ttu-id="53913-172">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="53913-172">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="53913-173">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="53913-173">The required password type.</span></span> <span data-ttu-id="53913-174">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="53913-174">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="53913-175">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="53913-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="53913-176">Int32</span><span class="sxs-lookup"><span data-stu-id="53913-176">Int32</span></span>|<span data-ttu-id="53913-177">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="53913-177">Number of previous passwords to block.</span></span> <span data-ttu-id="53913-178">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="53913-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="53913-179">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="53913-179">passwordRequired</span></span>|<span data-ttu-id="53913-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="53913-180">Boolean</span></span>|<span data-ttu-id="53913-181">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="53913-181">Whether or not to require a password.</span></span>|
|<span data-ttu-id="53913-182">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="53913-182">osMinimumVersion</span></span>|<span data-ttu-id="53913-183">String</span><span class="sxs-lookup"><span data-stu-id="53913-183">String</span></span>|<span data-ttu-id="53913-184">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="53913-184">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="53913-185">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="53913-185">osMaximumVersion</span></span>|<span data-ttu-id="53913-186">String</span><span class="sxs-lookup"><span data-stu-id="53913-186">String</span></span>|<span data-ttu-id="53913-187">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="53913-187">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="53913-188">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="53913-188">storageRequireEncryption</span></span>|<span data-ttu-id="53913-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="53913-189">Boolean</span></span>|<span data-ttu-id="53913-190">Exige criptografia em dispositivos Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="53913-190">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="53913-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="53913-191">Response</span></span>
<span data-ttu-id="53913-192">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53913-192">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53913-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53913-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="53913-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53913-194">Request</span></span>
<span data-ttu-id="53913-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53913-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="53913-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="53913-196">Response</span></span>
<span data-ttu-id="53913-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53913-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




