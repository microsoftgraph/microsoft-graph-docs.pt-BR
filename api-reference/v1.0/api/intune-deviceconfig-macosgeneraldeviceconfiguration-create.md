---
title: Criar macOSGeneralDeviceConfiguration
description: Cria um novo objeto macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aeabb81862241f7c8813d6cf30799e961e6c20f3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756271"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="825b3-103">Criar macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="825b3-103">Create macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="825b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="825b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="825b3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="825b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="825b3-106">Cria um novo objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="825b3-106">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="825b3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="825b3-107">Prerequisites</span></span>
<span data-ttu-id="825b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="825b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="825b3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="825b3-110">Permission type</span></span>|<span data-ttu-id="825b3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="825b3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="825b3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="825b3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="825b3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="825b3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="825b3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="825b3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="825b3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="825b3-115">Not supported.</span></span>|
|<span data-ttu-id="825b3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="825b3-116">Application</span></span>|<span data-ttu-id="825b3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="825b3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="825b3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="825b3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="825b3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="825b3-119">Request headers</span></span>
|<span data-ttu-id="825b3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="825b3-120">Header</span></span>|<span data-ttu-id="825b3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="825b3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="825b3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="825b3-122">Authorization</span></span>|<span data-ttu-id="825b3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="825b3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="825b3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="825b3-124">Accept</span></span>|<span data-ttu-id="825b3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="825b3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="825b3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="825b3-126">Request body</span></span>
<span data-ttu-id="825b3-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="825b3-127">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="825b3-128">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="825b3-128">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="825b3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="825b3-129">Property</span></span>|<span data-ttu-id="825b3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="825b3-130">Type</span></span>|<span data-ttu-id="825b3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="825b3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="825b3-132">id</span><span class="sxs-lookup"><span data-stu-id="825b3-132">id</span></span>|<span data-ttu-id="825b3-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="825b3-133">String</span></span>|<span data-ttu-id="825b3-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="825b3-134">Key of the entity.</span></span> <span data-ttu-id="825b3-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="825b3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="825b3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="825b3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="825b3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="825b3-137">DateTimeOffset</span></span>|<span data-ttu-id="825b3-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="825b3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="825b3-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="825b3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="825b3-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="825b3-140">createdDateTime</span></span>|<span data-ttu-id="825b3-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="825b3-141">DateTimeOffset</span></span>|<span data-ttu-id="825b3-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="825b3-142">DateTime the object was created.</span></span> <span data-ttu-id="825b3-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="825b3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="825b3-144">descrição</span><span class="sxs-lookup"><span data-stu-id="825b3-144">description</span></span>|<span data-ttu-id="825b3-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="825b3-145">String</span></span>|<span data-ttu-id="825b3-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="825b3-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="825b3-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="825b3-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="825b3-148">displayName</span><span class="sxs-lookup"><span data-stu-id="825b3-148">displayName</span></span>|<span data-ttu-id="825b3-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="825b3-149">String</span></span>|<span data-ttu-id="825b3-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="825b3-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="825b3-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="825b3-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="825b3-152">versão</span><span class="sxs-lookup"><span data-stu-id="825b3-152">version</span></span>|<span data-ttu-id="825b3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="825b3-153">Int32</span></span>|<span data-ttu-id="825b3-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="825b3-154">Version of the device configuration.</span></span> <span data-ttu-id="825b3-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="825b3-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="825b3-156">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="825b3-156">compliantAppsList</span></span>|<span data-ttu-id="825b3-157">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="825b3-157">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="825b3-158">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="825b3-158">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="825b3-159">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="825b3-159">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="825b3-160">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="825b3-160">compliantAppListType</span></span>|[<span data-ttu-id="825b3-161">appListType</span><span class="sxs-lookup"><span data-stu-id="825b3-161">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="825b3-162">Lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="825b3-162">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="825b3-163">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="825b3-163">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="825b3-164">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="825b3-164">emailInDomainSuffixes</span></span>|<span data-ttu-id="825b3-165">String collection</span><span class="sxs-lookup"><span data-stu-id="825b3-165">String collection</span></span>|<span data-ttu-id="825b3-166">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="825b3-166">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="825b3-167">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="825b3-167">passwordBlockSimple</span></span>|<span data-ttu-id="825b3-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="825b3-168">Boolean</span></span>|<span data-ttu-id="825b3-169">Bloquear senhas simples.</span><span class="sxs-lookup"><span data-stu-id="825b3-169">Block simple passwords.</span></span>|
|<span data-ttu-id="825b3-170">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="825b3-170">passwordExpirationDays</span></span>|<span data-ttu-id="825b3-171">Int32</span><span class="sxs-lookup"><span data-stu-id="825b3-171">Int32</span></span>|<span data-ttu-id="825b3-172">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="825b3-172">Number of days before the password expires.</span></span>|
|<span data-ttu-id="825b3-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="825b3-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="825b3-174">Int32</span><span class="sxs-lookup"><span data-stu-id="825b3-174">Int32</span></span>|<span data-ttu-id="825b3-175">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="825b3-175">Number of character sets a password must contain.</span></span> <span data-ttu-id="825b3-176">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="825b3-176">Valid values 0 to 4</span></span>|
|<span data-ttu-id="825b3-177">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="825b3-177">passwordMinimumLength</span></span>|<span data-ttu-id="825b3-178">Int32</span><span class="sxs-lookup"><span data-stu-id="825b3-178">Int32</span></span>|<span data-ttu-id="825b3-179">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="825b3-179">Minimum length of passwords.</span></span>|
|<span data-ttu-id="825b3-180">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="825b3-180">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="825b3-181">Int32</span><span class="sxs-lookup"><span data-stu-id="825b3-181">Int32</span></span>|<span data-ttu-id="825b3-182">Minutos de inatividade necessários antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="825b3-182">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="825b3-183">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="825b3-183">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="825b3-184">Int32</span><span class="sxs-lookup"><span data-stu-id="825b3-184">Int32</span></span>|<span data-ttu-id="825b3-185">Minutos de inatividade necessários antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="825b3-185">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="825b3-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="825b3-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="825b3-187">Int32</span><span class="sxs-lookup"><span data-stu-id="825b3-187">Int32</span></span>|<span data-ttu-id="825b3-188">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="825b3-188">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="825b3-189">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="825b3-189">passwordRequiredType</span></span>|[<span data-ttu-id="825b3-190">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="825b3-190">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="825b3-191">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="825b3-191">Type of password that is required.</span></span> <span data-ttu-id="825b3-192">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="825b3-192">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="825b3-193">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="825b3-193">passwordRequired</span></span>|<span data-ttu-id="825b3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="825b3-194">Boolean</span></span>|<span data-ttu-id="825b3-195">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="825b3-195">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="825b3-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="825b3-196">Response</span></span>
<span data-ttu-id="825b3-197">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="825b3-197">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="825b3-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="825b3-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="825b3-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="825b3-199">Request</span></span>
<span data-ttu-id="825b3-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="825b3-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="825b3-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="825b3-201">Response</span></span>
<span data-ttu-id="825b3-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="825b3-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




