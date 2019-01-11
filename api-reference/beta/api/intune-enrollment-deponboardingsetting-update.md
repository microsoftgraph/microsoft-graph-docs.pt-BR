---
title: Atualizar depOnboardingSetting
description: Atualize as propriedades de um objeto depOnboardingSetting.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 05b31f007aece229dacee41af354fdf7ab2807ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891116"
---
# <a name="update-deponboardingsetting"></a><span data-ttu-id="e2b00-103">Atualizar depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="e2b00-103">Update depOnboardingSetting</span></span>

> <span data-ttu-id="e2b00-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e2b00-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2b00-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e2b00-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2b00-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e2b00-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2b00-107">Atualize as propriedades de um objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="e2b00-107">Update the properties of a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e2b00-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2b00-108">Prerequisites</span></span>
<span data-ttu-id="e2b00-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2b00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2b00-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2b00-111">Permission type</span></span>|<span data-ttu-id="e2b00-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e2b00-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2b00-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2b00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2b00-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2b00-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e2b00-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2b00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2b00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2b00-116">Not supported.</span></span>|
|<span data-ttu-id="e2b00-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2b00-117">Application</span></span>|<span data-ttu-id="e2b00-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2b00-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2b00-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2b00-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="e2b00-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2b00-120">Request headers</span></span>
|<span data-ttu-id="e2b00-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2b00-121">Header</span></span>|<span data-ttu-id="e2b00-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e2b00-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2b00-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2b00-123">Authorization</span></span>|<span data-ttu-id="e2b00-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2b00-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2b00-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e2b00-125">Accept</span></span>|<span data-ttu-id="e2b00-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2b00-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2b00-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2b00-127">Request body</span></span>
<span data-ttu-id="e2b00-128">No corpo da solicitação, fornece uma representação JSON para o objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="e2b00-128">In the request body, supply a JSON representation for the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

<span data-ttu-id="e2b00-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span><span class="sxs-lookup"><span data-stu-id="e2b00-129">The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span></span>

|<span data-ttu-id="e2b00-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2b00-130">Property</span></span>|<span data-ttu-id="e2b00-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2b00-131">Type</span></span>|<span data-ttu-id="e2b00-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2b00-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2b00-133">id</span><span class="sxs-lookup"><span data-stu-id="e2b00-133">id</span></span>|<span data-ttu-id="e2b00-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2b00-134">String</span></span>|<span data-ttu-id="e2b00-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="e2b00-135">UUID for the object</span></span>|
|<span data-ttu-id="e2b00-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="e2b00-136">appleIdentifier</span></span>|<span data-ttu-id="e2b00-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2b00-137">String</span></span>|<span data-ttu-id="e2b00-138">A ID do Apple usada para obter o token atual.</span><span class="sxs-lookup"><span data-stu-id="e2b00-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="e2b00-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e2b00-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="e2b00-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2b00-140">DateTimeOffset</span></span>|<span data-ttu-id="e2b00-141">Quando o token irá expirar.</span><span class="sxs-lookup"><span data-stu-id="e2b00-141">When the token will expire.</span></span>|
|<span data-ttu-id="e2b00-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2b00-142">lastModifiedDateTime</span></span>|<span data-ttu-id="e2b00-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2b00-143">DateTimeOffset</span></span>|<span data-ttu-id="e2b00-144">Quando o serviço foi onboarded.</span><span class="sxs-lookup"><span data-stu-id="e2b00-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="e2b00-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e2b00-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="e2b00-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2b00-146">DateTimeOffset</span></span>|<span data-ttu-id="e2b00-147">Quando o syned última do serviço com Intune</span><span class="sxs-lookup"><span data-stu-id="e2b00-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="e2b00-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="e2b00-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="e2b00-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2b00-149">DateTimeOffset</span></span>|<span data-ttu-id="e2b00-150">Quando o Intune solicitado último uma sincronização.</span><span class="sxs-lookup"><span data-stu-id="e2b00-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="e2b00-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="e2b00-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="e2b00-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2b00-152">Boolean</span></span>|<span data-ttu-id="e2b00-153">Ou não o compartilhamento token do Dep está habilitado com o serviço de sincronização de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="e2b00-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="e2b00-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="e2b00-154">lastSyncErrorCode</span></span>|<span data-ttu-id="e2b00-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e2b00-155">Int32</span></span>|<span data-ttu-id="e2b00-156">Código de erro relatado pelo Apple durante a última sincronização dep.</span><span class="sxs-lookup"><span data-stu-id="e2b00-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="e2b00-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="e2b00-157">tokenType</span></span>|[<span data-ttu-id="e2b00-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="e2b00-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="e2b00-159">Obtém ou define o tipo de Token do Dep.</span><span class="sxs-lookup"><span data-stu-id="e2b00-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="e2b00-160">Os valores possíveis são: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="e2b00-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="e2b00-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="e2b00-161">tokenName</span></span>|<span data-ttu-id="e2b00-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2b00-162">String</span></span>|<span data-ttu-id="e2b00-163">Nome amigável para o Token de Dep</span><span class="sxs-lookup"><span data-stu-id="e2b00-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="e2b00-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e2b00-164">syncedDeviceCount</span></span>|<span data-ttu-id="e2b00-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e2b00-165">Int32</span></span>|<span data-ttu-id="e2b00-166">Obtém sincronizados contagem de dispositivo</span><span class="sxs-lookup"><span data-stu-id="e2b00-166">Gets synced device count</span></span>|
|<span data-ttu-id="e2b00-167">defaultProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="e2b00-167">defaultProfileDisplayName</span></span>|<span data-ttu-id="e2b00-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2b00-168">String</span></span>|<span data-ttu-id="e2b00-169">Obtém sincronizados contagem de dispositivo</span><span class="sxs-lookup"><span data-stu-id="e2b00-169">Gets synced device count</span></span>|
|<span data-ttu-id="e2b00-170">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="e2b00-170">dataSharingConsentGranted</span></span>|<span data-ttu-id="e2b00-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2b00-171">Boolean</span></span>|<span data-ttu-id="e2b00-172">Concedido consentimento para o compartilhamento de dados com Apple Dep Service</span><span class="sxs-lookup"><span data-stu-id="e2b00-172">Consent granted for data sharing with Apple Dep Service</span></span>|



## <a name="response"></a><span data-ttu-id="e2b00-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2b00-173">Response</span></span>
<span data-ttu-id="e2b00-174">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2b00-174">If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2b00-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2b00-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2b00-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2b00-176">Request</span></span>
<span data-ttu-id="e2b00-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2b00-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 589

{
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "defaultProfileDisplayName": "Default Profile Display Name value",
  "dataSharingConsentGranted": true
}
```

### <a name="response"></a><span data-ttu-id="e2b00-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2b00-178">Response</span></span>
<span data-ttu-id="e2b00-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2b00-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "40342229-2229-4034-2922-344029223440",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "defaultProfileDisplayName": "Default Profile Display Name value",
  "dataSharingConsentGranted": true
}
```





