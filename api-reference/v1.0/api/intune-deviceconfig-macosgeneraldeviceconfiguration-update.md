---
title: Atualizar macOSGeneralDeviceConfiguration
description: Atualiza as propriedades de um objeto macOSGeneralDeviceConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75349dff8d00d06f99f3b1c7c832e274c894de72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514295"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="5e663-103">Atualizar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5e663-103">Update macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="5e663-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e663-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e663-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e663-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e663-106">Atualiza as propriedades de um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5e663-106">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e663-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e663-107">Prerequisites</span></span>
<span data-ttu-id="5e663-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e663-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e663-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e663-110">Permission type</span></span>|<span data-ttu-id="5e663-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5e663-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e663-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e663-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e663-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e663-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5e663-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e663-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e663-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e663-115">Not supported.</span></span>|
|<span data-ttu-id="5e663-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e663-116">Application</span></span>|<span data-ttu-id="5e663-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e663-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e663-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e663-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5e663-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e663-119">Request headers</span></span>
|<span data-ttu-id="5e663-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e663-120">Header</span></span>|<span data-ttu-id="5e663-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5e663-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e663-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e663-122">Authorization</span></span>|<span data-ttu-id="5e663-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e663-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e663-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5e663-124">Accept</span></span>|<span data-ttu-id="5e663-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5e663-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e663-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e663-126">Request body</span></span>
<span data-ttu-id="5e663-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5e663-127">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="5e663-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5e663-128">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="5e663-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e663-129">Property</span></span>|<span data-ttu-id="5e663-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e663-130">Type</span></span>|<span data-ttu-id="5e663-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e663-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e663-132">id</span><span class="sxs-lookup"><span data-stu-id="5e663-132">id</span></span>|<span data-ttu-id="5e663-133">String</span><span class="sxs-lookup"><span data-stu-id="5e663-133">String</span></span>|<span data-ttu-id="5e663-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5e663-134">Key of the entity.</span></span> <span data-ttu-id="5e663-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e663-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e663-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e663-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5e663-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e663-137">DateTimeOffset</span></span>|<span data-ttu-id="5e663-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5e663-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5e663-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e663-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e663-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e663-140">createdDateTime</span></span>|<span data-ttu-id="5e663-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e663-141">DateTimeOffset</span></span>|<span data-ttu-id="5e663-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5e663-142">DateTime the object was created.</span></span> <span data-ttu-id="5e663-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e663-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e663-144">description</span><span class="sxs-lookup"><span data-stu-id="5e663-144">description</span></span>|<span data-ttu-id="5e663-145">String</span><span class="sxs-lookup"><span data-stu-id="5e663-145">String</span></span>|<span data-ttu-id="5e663-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e663-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5e663-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e663-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e663-148">displayName</span><span class="sxs-lookup"><span data-stu-id="5e663-148">displayName</span></span>|<span data-ttu-id="5e663-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e663-149">String</span></span>|<span data-ttu-id="5e663-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e663-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5e663-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e663-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e663-152">versão</span><span class="sxs-lookup"><span data-stu-id="5e663-152">version</span></span>|<span data-ttu-id="5e663-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5e663-153">Int32</span></span>|<span data-ttu-id="5e663-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e663-154">Version of the device configuration.</span></span> <span data-ttu-id="5e663-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e663-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e663-156">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="5e663-156">compliantAppsList</span></span>|<span data-ttu-id="5e663-157">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="5e663-157">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="5e663-158">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="5e663-158">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="5e663-159">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="5e663-159">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="5e663-160">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="5e663-160">compliantAppListType</span></span>|[<span data-ttu-id="5e663-161">appListType</span><span class="sxs-lookup"><span data-stu-id="5e663-161">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="5e663-162">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="5e663-162">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="5e663-163">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="5e663-163">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="5e663-164">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="5e663-164">emailInDomainSuffixes</span></span>|<span data-ttu-id="5e663-165">String collection</span><span class="sxs-lookup"><span data-stu-id="5e663-165">String collection</span></span>|<span data-ttu-id="5e663-166">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="5e663-166">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="5e663-167">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5e663-167">passwordBlockSimple</span></span>|<span data-ttu-id="5e663-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="5e663-168">Boolean</span></span>|<span data-ttu-id="5e663-169">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="5e663-169">Block simple passwords.</span></span>|
|<span data-ttu-id="5e663-170">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5e663-170">passwordExpirationDays</span></span>|<span data-ttu-id="5e663-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5e663-171">Int32</span></span>|<span data-ttu-id="5e663-172">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="5e663-172">Number of days before the password expires.</span></span>|
|<span data-ttu-id="5e663-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5e663-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="5e663-174">Int32</span><span class="sxs-lookup"><span data-stu-id="5e663-174">Int32</span></span>|<span data-ttu-id="5e663-175">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="5e663-175">Number of character sets a password must contain.</span></span> <span data-ttu-id="5e663-176">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="5e663-176">Valid values 0 to 4</span></span>|
|<span data-ttu-id="5e663-177">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5e663-177">passwordMinimumLength</span></span>|<span data-ttu-id="5e663-178">Int32</span><span class="sxs-lookup"><span data-stu-id="5e663-178">Int32</span></span>|<span data-ttu-id="5e663-179">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="5e663-179">Minimum length of passwords.</span></span>|
|<span data-ttu-id="5e663-180">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5e663-180">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5e663-181">Int32</span><span class="sxs-lookup"><span data-stu-id="5e663-181">Int32</span></span>|<span data-ttu-id="5e663-182">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="5e663-182">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="5e663-183">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="5e663-183">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="5e663-184">Int32</span><span class="sxs-lookup"><span data-stu-id="5e663-184">Int32</span></span>|<span data-ttu-id="5e663-185">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="5e663-185">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="5e663-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5e663-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5e663-187">Int32</span><span class="sxs-lookup"><span data-stu-id="5e663-187">Int32</span></span>|<span data-ttu-id="5e663-188">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="5e663-188">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="5e663-189">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5e663-189">passwordRequiredType</span></span>|[<span data-ttu-id="5e663-190">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5e663-190">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5e663-191">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="5e663-191">Type of password that is required.</span></span> <span data-ttu-id="5e663-192">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="5e663-192">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5e663-193">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5e663-193">passwordRequired</span></span>|<span data-ttu-id="5e663-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e663-194">Boolean</span></span>|<span data-ttu-id="5e663-195">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="5e663-195">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="5e663-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e663-196">Response</span></span>
<span data-ttu-id="5e663-197">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e663-197">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e663-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e663-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e663-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e663-199">Request</span></span>
<span data-ttu-id="5e663-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e663-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5e663-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e663-201">Response</span></span>
<span data-ttu-id="5e663-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e663-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




