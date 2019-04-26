---
title: Atualizar macOSGeneralDeviceConfiguration
description: Atualiza as propriedades de um objeto macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: beb53ec72e112dd576657bf31d20891419783dde
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554747"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="09fbc-103">Atualizar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="09fbc-103">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="09fbc-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09fbc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09fbc-105">Atualiza as propriedades de um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09fbc-105">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09fbc-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="09fbc-106">Prerequisites</span></span>
<span data-ttu-id="09fbc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09fbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09fbc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09fbc-109">Permission type</span></span>|<span data-ttu-id="09fbc-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="09fbc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09fbc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09fbc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="09fbc-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09fbc-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09fbc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09fbc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09fbc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09fbc-114">Not supported.</span></span>|
|<span data-ttu-id="09fbc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09fbc-115">Application</span></span>|<span data-ttu-id="09fbc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09fbc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09fbc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09fbc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="09fbc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09fbc-118">Request headers</span></span>
|<span data-ttu-id="09fbc-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="09fbc-119">Header</span></span>|<span data-ttu-id="09fbc-120">Valor</span><span class="sxs-lookup"><span data-stu-id="09fbc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09fbc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="09fbc-121">Authorization</span></span>|<span data-ttu-id="09fbc-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09fbc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09fbc-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="09fbc-123">Accept</span></span>|<span data-ttu-id="09fbc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="09fbc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09fbc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09fbc-125">Request body</span></span>
<span data-ttu-id="09fbc-126">No corpo da solicitação, forneça uma representação JSON do objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09fbc-126">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="09fbc-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09fbc-127">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="09fbc-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09fbc-128">Property</span></span>|<span data-ttu-id="09fbc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="09fbc-129">Type</span></span>|<span data-ttu-id="09fbc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="09fbc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09fbc-131">id</span><span class="sxs-lookup"><span data-stu-id="09fbc-131">id</span></span>|<span data-ttu-id="09fbc-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09fbc-132">String</span></span>|<span data-ttu-id="09fbc-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="09fbc-133">Key of the entity.</span></span> <span data-ttu-id="09fbc-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09fbc-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09fbc-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09fbc-135">lastModifiedDateTime</span></span>|<span data-ttu-id="09fbc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09fbc-136">DateTimeOffset</span></span>|<span data-ttu-id="09fbc-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="09fbc-137">DateTime the object was last modified.</span></span> <span data-ttu-id="09fbc-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09fbc-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09fbc-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09fbc-139">createdDateTime</span></span>|<span data-ttu-id="09fbc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09fbc-140">DateTimeOffset</span></span>|<span data-ttu-id="09fbc-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="09fbc-141">DateTime the object was created.</span></span> <span data-ttu-id="09fbc-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09fbc-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09fbc-143">description</span><span class="sxs-lookup"><span data-stu-id="09fbc-143">description</span></span>|<span data-ttu-id="09fbc-144">String</span><span class="sxs-lookup"><span data-stu-id="09fbc-144">String</span></span>|<span data-ttu-id="09fbc-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="09fbc-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="09fbc-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09fbc-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09fbc-147">displayName</span><span class="sxs-lookup"><span data-stu-id="09fbc-147">displayName</span></span>|<span data-ttu-id="09fbc-148">String</span><span class="sxs-lookup"><span data-stu-id="09fbc-148">String</span></span>|<span data-ttu-id="09fbc-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="09fbc-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="09fbc-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09fbc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09fbc-151">versão</span><span class="sxs-lookup"><span data-stu-id="09fbc-151">version</span></span>|<span data-ttu-id="09fbc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="09fbc-152">Int32</span></span>|<span data-ttu-id="09fbc-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="09fbc-153">Version of the device configuration.</span></span> <span data-ttu-id="09fbc-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09fbc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09fbc-155">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="09fbc-155">compliantAppsList</span></span>|<span data-ttu-id="09fbc-156">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="09fbc-156">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="09fbc-157">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="09fbc-157">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="09fbc-158">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="09fbc-158">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="09fbc-159">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="09fbc-159">compliantAppListType</span></span>|[<span data-ttu-id="09fbc-160">appListType</span><span class="sxs-lookup"><span data-stu-id="09fbc-160">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="09fbc-161">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="09fbc-161">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="09fbc-162">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="09fbc-162">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="09fbc-163">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="09fbc-163">emailInDomainSuffixes</span></span>|<span data-ttu-id="09fbc-164">String collection</span><span class="sxs-lookup"><span data-stu-id="09fbc-164">String collection</span></span>|<span data-ttu-id="09fbc-165">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="09fbc-165">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="09fbc-166">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="09fbc-166">passwordBlockSimple</span></span>|<span data-ttu-id="09fbc-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="09fbc-167">Boolean</span></span>|<span data-ttu-id="09fbc-168">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="09fbc-168">Block simple passwords.</span></span>|
|<span data-ttu-id="09fbc-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="09fbc-169">passwordExpirationDays</span></span>|<span data-ttu-id="09fbc-170">Int32</span><span class="sxs-lookup"><span data-stu-id="09fbc-170">Int32</span></span>|<span data-ttu-id="09fbc-171">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="09fbc-171">Number of days before the password expires.</span></span>|
|<span data-ttu-id="09fbc-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="09fbc-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="09fbc-173">Int32</span><span class="sxs-lookup"><span data-stu-id="09fbc-173">Int32</span></span>|<span data-ttu-id="09fbc-174">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="09fbc-174">Number of character sets a password must contain.</span></span> <span data-ttu-id="09fbc-175">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="09fbc-175">Valid values 0 to 4</span></span>|
|<span data-ttu-id="09fbc-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="09fbc-176">passwordMinimumLength</span></span>|<span data-ttu-id="09fbc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="09fbc-177">Int32</span></span>|<span data-ttu-id="09fbc-178">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="09fbc-178">Minimum length of passwords.</span></span>|
|<span data-ttu-id="09fbc-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="09fbc-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="09fbc-180">Int32</span><span class="sxs-lookup"><span data-stu-id="09fbc-180">Int32</span></span>|<span data-ttu-id="09fbc-181">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="09fbc-181">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="09fbc-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="09fbc-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="09fbc-183">Int32</span><span class="sxs-lookup"><span data-stu-id="09fbc-183">Int32</span></span>|<span data-ttu-id="09fbc-184">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="09fbc-184">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="09fbc-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="09fbc-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="09fbc-186">Int32</span><span class="sxs-lookup"><span data-stu-id="09fbc-186">Int32</span></span>|<span data-ttu-id="09fbc-187">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="09fbc-187">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="09fbc-188">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="09fbc-188">passwordRequiredType</span></span>|[<span data-ttu-id="09fbc-189">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="09fbc-189">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="09fbc-190">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="09fbc-190">Type of password that is required.</span></span> <span data-ttu-id="09fbc-191">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="09fbc-191">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="09fbc-192">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="09fbc-192">passwordRequired</span></span>|<span data-ttu-id="09fbc-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="09fbc-193">Boolean</span></span>|<span data-ttu-id="09fbc-194">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="09fbc-194">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="09fbc-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="09fbc-195">Response</span></span>
<span data-ttu-id="09fbc-196">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09fbc-196">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09fbc-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09fbc-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="09fbc-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09fbc-198">Request</span></span>
<span data-ttu-id="09fbc-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09fbc-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 906

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```

### <a name="response"></a><span data-ttu-id="09fbc-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="09fbc-200">Response</span></span>
<span data-ttu-id="09fbc-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09fbc-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1078

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```



