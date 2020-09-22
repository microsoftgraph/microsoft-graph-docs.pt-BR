---
title: Criar depOnboardingSetting
description: Criar um novo objeto depOnboardingSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b1c592d0fba917fc1254c982523514d73828dc7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050553"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="afb4b-103">Criar depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="afb4b-103">Create depOnboardingSetting</span></span>

<span data-ttu-id="afb4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afb4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afb4b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="afb4b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afb4b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="afb4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afb4b-107">Criar um novo objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="afb4b-107">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afb4b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="afb4b-108">Prerequisites</span></span>
<span data-ttu-id="afb4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afb4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afb4b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afb4b-111">Permission type</span></span>|<span data-ttu-id="afb4b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="afb4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afb4b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afb4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afb4b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afb4b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="afb4b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afb4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afb4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afb4b-116">Not supported.</span></span>|
|<span data-ttu-id="afb4b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afb4b-117">Application</span></span>|<span data-ttu-id="afb4b-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afb4b-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="afb4b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afb4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="afb4b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afb4b-120">Request headers</span></span>
|<span data-ttu-id="afb4b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="afb4b-121">Header</span></span>|<span data-ttu-id="afb4b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="afb4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afb4b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="afb4b-123">Authorization</span></span>|<span data-ttu-id="afb4b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afb4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afb4b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="afb4b-125">Accept</span></span>|<span data-ttu-id="afb4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afb4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afb4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afb4b-127">Request body</span></span>
<span data-ttu-id="afb4b-128">No corpo da solicitação, forneça uma representação JSON do objeto depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="afb4b-128">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="afb4b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="afb4b-129">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="afb4b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="afb4b-130">Property</span></span>|<span data-ttu-id="afb4b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="afb4b-131">Type</span></span>|<span data-ttu-id="afb4b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="afb4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afb4b-133">id</span><span class="sxs-lookup"><span data-stu-id="afb4b-133">id</span></span>|<span data-ttu-id="afb4b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afb4b-134">String</span></span>|<span data-ttu-id="afb4b-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="afb4b-135">UUID for the object</span></span>|
|<span data-ttu-id="afb4b-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="afb4b-136">appleIdentifier</span></span>|<span data-ttu-id="afb4b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afb4b-137">String</span></span>|<span data-ttu-id="afb4b-138">A ID da Apple usada para obter o token atual.</span><span class="sxs-lookup"><span data-stu-id="afb4b-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="afb4b-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="afb4b-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="afb4b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afb4b-140">DateTimeOffset</span></span>|<span data-ttu-id="afb4b-141">Quando o token expirará.</span><span class="sxs-lookup"><span data-stu-id="afb4b-141">When the token will expire.</span></span>|
|<span data-ttu-id="afb4b-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="afb4b-142">lastModifiedDateTime</span></span>|<span data-ttu-id="afb4b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afb4b-143">DateTimeOffset</span></span>|<span data-ttu-id="afb4b-144">Quando o serviço foi integrado.</span><span class="sxs-lookup"><span data-stu-id="afb4b-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="afb4b-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="afb4b-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="afb4b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afb4b-146">DateTimeOffset</span></span>|<span data-ttu-id="afb4b-147">Quando o serviço última syned com o Intune</span><span class="sxs-lookup"><span data-stu-id="afb4b-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="afb4b-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="afb4b-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="afb4b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afb4b-149">DateTimeOffset</span></span>|<span data-ttu-id="afb4b-150">Quando o Intune solicitou uma sincronização pela última vez.</span><span class="sxs-lookup"><span data-stu-id="afb4b-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="afb4b-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="afb4b-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="afb4b-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="afb4b-152">Boolean</span></span>|<span data-ttu-id="afb4b-153">Se o compartilhamento de token DEP está ou não habilitado com o serviço de sincronização de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="afb4b-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="afb4b-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="afb4b-154">lastSyncErrorCode</span></span>|<span data-ttu-id="afb4b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="afb4b-155">Int32</span></span>|<span data-ttu-id="afb4b-156">Código de erro relatado pela Apple durante a última sincronização de Dep.</span><span class="sxs-lookup"><span data-stu-id="afb4b-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="afb4b-157">TokenType</span><span class="sxs-lookup"><span data-stu-id="afb4b-157">tokenType</span></span>|[<span data-ttu-id="afb4b-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="afb4b-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="afb4b-159">Obtém ou define o tipo de token Dep.</span><span class="sxs-lookup"><span data-stu-id="afb4b-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="afb4b-160">Os valores possíveis são: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="afb4b-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="afb4b-161">tokenname</span><span class="sxs-lookup"><span data-stu-id="afb4b-161">tokenName</span></span>|<span data-ttu-id="afb4b-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afb4b-162">String</span></span>|<span data-ttu-id="afb4b-163">Nome amigável para token Dep</span><span class="sxs-lookup"><span data-stu-id="afb4b-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="afb4b-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="afb4b-164">syncedDeviceCount</span></span>|<span data-ttu-id="afb4b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="afb4b-165">Int32</span></span>|<span data-ttu-id="afb4b-166">Obtém a contagem de dispositivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="afb4b-166">Gets synced device count</span></span>|
|<span data-ttu-id="afb4b-167">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="afb4b-167">dataSharingConsentGranted</span></span>|<span data-ttu-id="afb4b-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="afb4b-168">Boolean</span></span>|<span data-ttu-id="afb4b-169">Consentimento concedido para compartilhamento de dados com o serviço Apple Dep</span><span class="sxs-lookup"><span data-stu-id="afb4b-169">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="afb4b-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="afb4b-170">roleScopeTagIds</span></span>|<span data-ttu-id="afb4b-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="afb4b-171">String collection</span></span>|<span data-ttu-id="afb4b-172">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="afb4b-172">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="afb4b-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="afb4b-173">Response</span></span>
<span data-ttu-id="afb4b-174">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afb4b-174">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afb4b-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afb4b-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="afb4b-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afb4b-176">Request</span></span>
<span data-ttu-id="afb4b-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="afb4b-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
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

### <a name="response"></a><span data-ttu-id="afb4b-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="afb4b-178">Response</span></span>
<span data-ttu-id="afb4b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afb4b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






