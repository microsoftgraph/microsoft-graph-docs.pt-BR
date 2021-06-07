---
title: Criar windowsPhone81GeneralConfiguration
description: Criar um novo objeto windowsPhone81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 267d3bbf4065e6e2f7c270efdab31cbe02f3d090
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760409"
---
# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="f74e2-103">Criar windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="f74e2-103">Create windowsPhone81GeneralConfiguration</span></span>

<span data-ttu-id="f74e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f74e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f74e2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f74e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f74e2-106">Criar um novo objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f74e2-106">Create a new [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f74e2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f74e2-107">Prerequisites</span></span>
<span data-ttu-id="f74e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f74e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f74e2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f74e2-110">Permission type</span></span>|<span data-ttu-id="f74e2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f74e2-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f74e2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f74e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f74e2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f74e2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f74e2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f74e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f74e2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f74e2-115">Not supported.</span></span>|
|<span data-ttu-id="f74e2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f74e2-116">Application</span></span>|<span data-ttu-id="f74e2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f74e2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f74e2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f74e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f74e2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f74e2-119">Request headers</span></span>
|<span data-ttu-id="f74e2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f74e2-120">Header</span></span>|<span data-ttu-id="f74e2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f74e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f74e2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f74e2-122">Authorization</span></span>|<span data-ttu-id="f74e2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f74e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f74e2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f74e2-124">Accept</span></span>|<span data-ttu-id="f74e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f74e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f74e2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f74e2-126">Request body</span></span>
<span data-ttu-id="f74e2-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f74e2-127">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="f74e2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f74e2-128">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="f74e2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f74e2-129">Property</span></span>|<span data-ttu-id="f74e2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f74e2-130">Type</span></span>|<span data-ttu-id="f74e2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f74e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f74e2-132">id</span><span class="sxs-lookup"><span data-stu-id="f74e2-132">id</span></span>|<span data-ttu-id="f74e2-133">String</span><span class="sxs-lookup"><span data-stu-id="f74e2-133">String</span></span>|<span data-ttu-id="f74e2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f74e2-134">Key of the entity.</span></span> <span data-ttu-id="f74e2-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f74e2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f74e2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f74e2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f74e2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f74e2-137">DateTimeOffset</span></span>|<span data-ttu-id="f74e2-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f74e2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f74e2-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f74e2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f74e2-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f74e2-140">createdDateTime</span></span>|<span data-ttu-id="f74e2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f74e2-141">DateTimeOffset</span></span>|<span data-ttu-id="f74e2-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f74e2-142">DateTime the object was created.</span></span> <span data-ttu-id="f74e2-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f74e2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f74e2-144">description</span><span class="sxs-lookup"><span data-stu-id="f74e2-144">description</span></span>|<span data-ttu-id="f74e2-145">String</span><span class="sxs-lookup"><span data-stu-id="f74e2-145">String</span></span>|<span data-ttu-id="f74e2-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f74e2-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f74e2-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f74e2-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f74e2-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f74e2-148">displayName</span></span>|<span data-ttu-id="f74e2-149">String</span><span class="sxs-lookup"><span data-stu-id="f74e2-149">String</span></span>|<span data-ttu-id="f74e2-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f74e2-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f74e2-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f74e2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f74e2-152">versão</span><span class="sxs-lookup"><span data-stu-id="f74e2-152">version</span></span>|<span data-ttu-id="f74e2-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f74e2-153">Int32</span></span>|<span data-ttu-id="f74e2-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f74e2-154">Version of the device configuration.</span></span> <span data-ttu-id="f74e2-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f74e2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f74e2-156">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="f74e2-156">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="f74e2-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-157">Boolean</span></span>|<span data-ttu-id="f74e2-158">Valor que indica se esta política se aplica somente ao Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="f74e2-158">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="f74e2-159">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f74e2-159">This property is read-only.</span></span>|
|<span data-ttu-id="f74e2-160">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="f74e2-160">appsBlockCopyPaste</span></span>|<span data-ttu-id="f74e2-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-161">Boolean</span></span>|<span data-ttu-id="f74e2-162">Indica se a função copiar/colar deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="f74e2-162">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="f74e2-163">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="f74e2-163">bluetoothBlocked</span></span>|<span data-ttu-id="f74e2-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-164">Boolean</span></span>|<span data-ttu-id="f74e2-165">Indica se o bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f74e2-165">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="f74e2-166">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="f74e2-166">cameraBlocked</span></span>|<span data-ttu-id="f74e2-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-167">Boolean</span></span>|<span data-ttu-id="f74e2-168">Indica se a câmera deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="f74e2-168">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="f74e2-169">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="f74e2-169">cellularBlockWifiTethering</span></span>|<span data-ttu-id="f74e2-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-170">Boolean</span></span>|<span data-ttu-id="f74e2-171">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f74e2-171">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="f74e2-172">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f74e2-172">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="f74e2-173">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="f74e2-173">compliantAppsList</span></span>|<span data-ttu-id="f74e2-174">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f74e2-174">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f74e2-175">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="f74e2-175">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="f74e2-176">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="f74e2-176">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f74e2-177">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="f74e2-177">compliantAppListType</span></span>|[<span data-ttu-id="f74e2-178">appListType</span><span class="sxs-lookup"><span data-stu-id="f74e2-178">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="f74e2-179">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="f74e2-179">List that is in the AppComplianceList.</span></span> <span data-ttu-id="f74e2-180">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="f74e2-180">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="f74e2-181">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="f74e2-181">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="f74e2-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-182">Boolean</span></span>|<span data-ttu-id="f74e2-183">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f74e2-183">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="f74e2-184">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="f74e2-184">emailBlockAddingAccounts</span></span>|<span data-ttu-id="f74e2-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-185">Boolean</span></span>|<span data-ttu-id="f74e2-186">Indica se as contas de email personalizadas devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="f74e2-186">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="f74e2-187">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="f74e2-187">locationServicesBlocked</span></span>|<span data-ttu-id="f74e2-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-188">Boolean</span></span>|<span data-ttu-id="f74e2-189">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="f74e2-189">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="f74e2-190">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="f74e2-190">microsoftAccountBlocked</span></span>|<span data-ttu-id="f74e2-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-191">Boolean</span></span>|<span data-ttu-id="f74e2-192">Indica se o uso de uma conta da Microsoft deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f74e2-192">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="f74e2-193">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="f74e2-193">nfcBlocked</span></span>|<span data-ttu-id="f74e2-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-194">Boolean</span></span>|<span data-ttu-id="f74e2-195">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="f74e2-195">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="f74e2-196">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f74e2-196">passwordBlockSimple</span></span>|<span data-ttu-id="f74e2-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-197">Boolean</span></span>|<span data-ttu-id="f74e2-198">Indica se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="f74e2-198">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="f74e2-199">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f74e2-199">passwordExpirationDays</span></span>|<span data-ttu-id="f74e2-200">Int32</span><span class="sxs-lookup"><span data-stu-id="f74e2-200">Int32</span></span>|<span data-ttu-id="f74e2-201">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="f74e2-201">Number of days before the password expires.</span></span>|
|<span data-ttu-id="f74e2-202">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f74e2-202">passwordMinimumLength</span></span>|<span data-ttu-id="f74e2-203">Int32</span><span class="sxs-lookup"><span data-stu-id="f74e2-203">Int32</span></span>|<span data-ttu-id="f74e2-204">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="f74e2-204">Minimum length of passwords.</span></span>|
|<span data-ttu-id="f74e2-205">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f74e2-205">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f74e2-206">Int32</span><span class="sxs-lookup"><span data-stu-id="f74e2-206">Int32</span></span>|<span data-ttu-id="f74e2-207">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="f74e2-207">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="f74e2-208">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f74e2-208">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f74e2-209">Int32</span><span class="sxs-lookup"><span data-stu-id="f74e2-209">Int32</span></span>|<span data-ttu-id="f74e2-210">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="f74e2-210">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="f74e2-211">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f74e2-211">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f74e2-212">Int32</span><span class="sxs-lookup"><span data-stu-id="f74e2-212">Int32</span></span>|<span data-ttu-id="f74e2-213">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="f74e2-213">Number of previous passwords to block.</span></span> <span data-ttu-id="f74e2-214">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="f74e2-214">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f74e2-215">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f74e2-215">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f74e2-216">Int32</span><span class="sxs-lookup"><span data-stu-id="f74e2-216">Int32</span></span>|<span data-ttu-id="f74e2-217">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="f74e2-217">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="f74e2-218">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f74e2-218">passwordRequiredType</span></span>|[<span data-ttu-id="f74e2-219">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f74e2-219">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f74e2-220">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="f74e2-220">Password type that is required.</span></span> <span data-ttu-id="f74e2-221">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f74e2-221">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f74e2-222">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f74e2-222">passwordRequired</span></span>|<span data-ttu-id="f74e2-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-223">Boolean</span></span>|<span data-ttu-id="f74e2-224">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="f74e2-224">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="f74e2-225">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="f74e2-225">screenCaptureBlocked</span></span>|<span data-ttu-id="f74e2-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-226">Boolean</span></span>|<span data-ttu-id="f74e2-227">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="f74e2-227">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="f74e2-228">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="f74e2-228">storageBlockRemovableStorage</span></span>|<span data-ttu-id="f74e2-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-229">Boolean</span></span>|<span data-ttu-id="f74e2-230">Indica se o armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f74e2-230">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="f74e2-231">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f74e2-231">storageRequireEncryption</span></span>|<span data-ttu-id="f74e2-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-232">Boolean</span></span>|<span data-ttu-id="f74e2-233">Indica se a criptografia é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="f74e2-233">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="f74e2-234">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="f74e2-234">webBrowserBlocked</span></span>|<span data-ttu-id="f74e2-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-235">Boolean</span></span>|<span data-ttu-id="f74e2-236">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f74e2-236">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="f74e2-237">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="f74e2-237">wifiBlocked</span></span>|<span data-ttu-id="f74e2-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-238">Boolean</span></span>|<span data-ttu-id="f74e2-239">Indica se o Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f74e2-239">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="f74e2-240">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="f74e2-240">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="f74e2-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-241">Boolean</span></span>|<span data-ttu-id="f74e2-242">Indica se a conexão automática a hotspots Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="f74e2-242">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="f74e2-243">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f74e2-243">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="f74e2-244">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="f74e2-244">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="f74e2-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-245">Boolean</span></span>|<span data-ttu-id="f74e2-246">Indica se os relatórios de hotspot Wi-Fi devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="f74e2-246">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="f74e2-247">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f74e2-247">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="f74e2-248">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f74e2-248">windowsStoreBlocked</span></span>|<span data-ttu-id="f74e2-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="f74e2-249">Boolean</span></span>|<span data-ttu-id="f74e2-250">Indica se a Windows Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="f74e2-250">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="f74e2-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="f74e2-251">Response</span></span>
<span data-ttu-id="f74e2-252">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f74e2-252">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f74e2-253">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f74e2-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="f74e2-254">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f74e2-254">Request</span></span>
<span data-ttu-id="f74e2-255">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f74e2-255">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="f74e2-256">Resposta</span><span class="sxs-lookup"><span data-stu-id="f74e2-256">Response</span></span>
<span data-ttu-id="f74e2-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f74e2-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




