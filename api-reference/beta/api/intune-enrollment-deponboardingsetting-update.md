---
title: Atualizar depOnboardingSetting
description: Atualiza as propriedades de um objeto depOnboardingSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fd32ba5e867f60b36c0bf8ebe499ecc8d81c908f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731201"
---
# <a name="update-deponboardingsetting"></a><span data-ttu-id="6300f-103">Atualizar depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="6300f-103">Update depOnboardingSetting</span></span>

<span data-ttu-id="6300f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6300f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6300f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6300f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6300f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6300f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6300f-107">Atualiza as propriedades de um objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="6300f-107">Update the properties of a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6300f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6300f-108">Prerequisites</span></span>
<span data-ttu-id="6300f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6300f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6300f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6300f-111">Permission type</span></span>|<span data-ttu-id="6300f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6300f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6300f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6300f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6300f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6300f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6300f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6300f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6300f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6300f-116">Not supported.</span></span>|
|<span data-ttu-id="6300f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6300f-117">Application</span></span>|<span data-ttu-id="6300f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6300f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6300f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6300f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="6300f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6300f-120">Request headers</span></span>
|<span data-ttu-id="6300f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6300f-121">Header</span></span>|<span data-ttu-id="6300f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6300f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6300f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6300f-123">Authorization</span></span>|<span data-ttu-id="6300f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6300f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6300f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6300f-125">Accept</span></span>|<span data-ttu-id="6300f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6300f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6300f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6300f-127">Request body</span></span>
<span data-ttu-id="6300f-128">No corpo da solicitação, forneça uma representação JSON do objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="6300f-128">In the request body, supply a JSON representation for the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

<span data-ttu-id="6300f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span><span class="sxs-lookup"><span data-stu-id="6300f-129">The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span></span>

|<span data-ttu-id="6300f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6300f-130">Property</span></span>|<span data-ttu-id="6300f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6300f-131">Type</span></span>|<span data-ttu-id="6300f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6300f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6300f-133">id</span><span class="sxs-lookup"><span data-stu-id="6300f-133">id</span></span>|<span data-ttu-id="6300f-134">String</span><span class="sxs-lookup"><span data-stu-id="6300f-134">String</span></span>|<span data-ttu-id="6300f-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="6300f-135">UUID for the object</span></span>|
|<span data-ttu-id="6300f-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="6300f-136">appleIdentifier</span></span>|<span data-ttu-id="6300f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6300f-137">String</span></span>|<span data-ttu-id="6300f-138">A ID da Apple usada para obter o token atual.</span><span class="sxs-lookup"><span data-stu-id="6300f-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="6300f-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6300f-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="6300f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6300f-140">DateTimeOffset</span></span>|<span data-ttu-id="6300f-141">Quando o token expirará.</span><span class="sxs-lookup"><span data-stu-id="6300f-141">When the token will expire.</span></span>|
|<span data-ttu-id="6300f-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6300f-142">lastModifiedDateTime</span></span>|<span data-ttu-id="6300f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6300f-143">DateTimeOffset</span></span>|<span data-ttu-id="6300f-144">Quando o serviço foi integrado.</span><span class="sxs-lookup"><span data-stu-id="6300f-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="6300f-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6300f-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="6300f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6300f-146">DateTimeOffset</span></span>|<span data-ttu-id="6300f-147">Quando o serviço última syned com o Intune</span><span class="sxs-lookup"><span data-stu-id="6300f-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="6300f-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="6300f-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="6300f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6300f-149">DateTimeOffset</span></span>|<span data-ttu-id="6300f-150">Quando o Intune solicitou uma sincronização pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6300f-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="6300f-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="6300f-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="6300f-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="6300f-152">Boolean</span></span>|<span data-ttu-id="6300f-153">Se o compartilhamento de token DEP está ou não habilitado com o serviço de sincronização de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="6300f-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="6300f-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="6300f-154">lastSyncErrorCode</span></span>|<span data-ttu-id="6300f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="6300f-155">Int32</span></span>|<span data-ttu-id="6300f-156">Código de erro relatado pela Apple durante a última sincronização de Dep.</span><span class="sxs-lookup"><span data-stu-id="6300f-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="6300f-157">TokenType</span><span class="sxs-lookup"><span data-stu-id="6300f-157">tokenType</span></span>|[<span data-ttu-id="6300f-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="6300f-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="6300f-159">Obtém ou define o tipo de token Dep.</span><span class="sxs-lookup"><span data-stu-id="6300f-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="6300f-160">Os valores possíveis são: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="6300f-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="6300f-161">tokenname</span><span class="sxs-lookup"><span data-stu-id="6300f-161">tokenName</span></span>|<span data-ttu-id="6300f-162">String</span><span class="sxs-lookup"><span data-stu-id="6300f-162">String</span></span>|<span data-ttu-id="6300f-163">Nome amigável para token Dep</span><span class="sxs-lookup"><span data-stu-id="6300f-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="6300f-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6300f-164">syncedDeviceCount</span></span>|<span data-ttu-id="6300f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6300f-165">Int32</span></span>|<span data-ttu-id="6300f-166">Obtém a contagem de dispositivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="6300f-166">Gets synced device count</span></span>|
|<span data-ttu-id="6300f-167">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="6300f-167">dataSharingConsentGranted</span></span>|<span data-ttu-id="6300f-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="6300f-168">Boolean</span></span>|<span data-ttu-id="6300f-169">Consentimento concedido para compartilhamento de dados com o serviço Apple Dep</span><span class="sxs-lookup"><span data-stu-id="6300f-169">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="6300f-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6300f-170">roleScopeTagIds</span></span>|<span data-ttu-id="6300f-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6300f-171">String collection</span></span>|<span data-ttu-id="6300f-172">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6300f-172">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="6300f-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="6300f-173">Response</span></span>
<span data-ttu-id="6300f-174">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6300f-174">If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6300f-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6300f-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="6300f-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6300f-176">Request</span></span>
<span data-ttu-id="6300f-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6300f-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 576

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="6300f-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="6300f-178">Response</span></span>
<span data-ttu-id="6300f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6300f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 689

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
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





