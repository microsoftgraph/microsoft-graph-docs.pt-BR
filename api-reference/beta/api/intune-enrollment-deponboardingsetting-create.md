---
title: Criar depOnboardingSetting
description: Crie um novo objeto depOnboardingSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e4417c01a435ceb8392eff280992877ebdeb79e4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135730"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="a96ce-103">Criar depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="a96ce-103">Create depOnboardingSetting</span></span>

<span data-ttu-id="a96ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a96ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a96ce-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a96ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a96ce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a96ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a96ce-107">Crie um novo [objeto depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)</span><span class="sxs-lookup"><span data-stu-id="a96ce-107">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a96ce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a96ce-108">Prerequisites</span></span>
<span data-ttu-id="a96ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a96ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a96ce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a96ce-111">Permission type</span></span>|<span data-ttu-id="a96ce-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a96ce-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a96ce-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a96ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a96ce-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a96ce-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a96ce-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a96ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a96ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a96ce-116">Not supported.</span></span>|
|<span data-ttu-id="a96ce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a96ce-117">Application</span></span>|<span data-ttu-id="a96ce-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a96ce-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a96ce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a96ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="a96ce-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a96ce-120">Request headers</span></span>
|<span data-ttu-id="a96ce-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a96ce-121">Header</span></span>|<span data-ttu-id="a96ce-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a96ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a96ce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a96ce-123">Authorization</span></span>|<span data-ttu-id="a96ce-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a96ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a96ce-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a96ce-125">Accept</span></span>|<span data-ttu-id="a96ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a96ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a96ce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a96ce-127">Request body</span></span>
<span data-ttu-id="a96ce-128">No corpo da solicitação, fornece uma representação JSON para o objeto depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="a96ce-128">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="a96ce-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="a96ce-129">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="a96ce-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a96ce-130">Property</span></span>|<span data-ttu-id="a96ce-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a96ce-131">Type</span></span>|<span data-ttu-id="a96ce-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a96ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a96ce-133">id</span><span class="sxs-lookup"><span data-stu-id="a96ce-133">id</span></span>|<span data-ttu-id="a96ce-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a96ce-134">String</span></span>|<span data-ttu-id="a96ce-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="a96ce-135">UUID for the object</span></span>|
|<span data-ttu-id="a96ce-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="a96ce-136">appleIdentifier</span></span>|<span data-ttu-id="a96ce-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a96ce-137">String</span></span>|<span data-ttu-id="a96ce-138">A ID da Apple usada para obter o token atual.</span><span class="sxs-lookup"><span data-stu-id="a96ce-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="a96ce-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a96ce-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="a96ce-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a96ce-140">DateTimeOffset</span></span>|<span data-ttu-id="a96ce-141">Quando o token expirar.</span><span class="sxs-lookup"><span data-stu-id="a96ce-141">When the token will expire.</span></span>|
|<span data-ttu-id="a96ce-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a96ce-142">lastModifiedDateTime</span></span>|<span data-ttu-id="a96ce-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a96ce-143">DateTimeOffset</span></span>|<span data-ttu-id="a96ce-144">Quando o serviço foi integrado.</span><span class="sxs-lookup"><span data-stu-id="a96ce-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="a96ce-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a96ce-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="a96ce-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a96ce-146">DateTimeOffset</span></span>|<span data-ttu-id="a96ce-147">Quando o serviço foi sintetizado pela última vez com o Intune</span><span class="sxs-lookup"><span data-stu-id="a96ce-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="a96ce-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="a96ce-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="a96ce-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a96ce-149">DateTimeOffset</span></span>|<span data-ttu-id="a96ce-150">Quando o Intune solicitou pela última vez uma sincronização.</span><span class="sxs-lookup"><span data-stu-id="a96ce-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="a96ce-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="a96ce-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="a96ce-152">Booleano</span><span class="sxs-lookup"><span data-stu-id="a96ce-152">Boolean</span></span>|<span data-ttu-id="a96ce-153">Se o compartilhamento de token Dep está habilitado ou não com o serviço de Sincronização de Dados escolares.</span><span class="sxs-lookup"><span data-stu-id="a96ce-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="a96ce-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="a96ce-154">lastSyncErrorCode</span></span>|<span data-ttu-id="a96ce-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a96ce-155">Int32</span></span>|<span data-ttu-id="a96ce-156">Código de erro relatado pela Apple durante a última sincronização de dep.</span><span class="sxs-lookup"><span data-stu-id="a96ce-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="a96ce-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="a96ce-157">tokenType</span></span>|[<span data-ttu-id="a96ce-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="a96ce-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="a96ce-159">Obtém ou define o Tipo de Token de Dep.</span><span class="sxs-lookup"><span data-stu-id="a96ce-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="a96ce-160">Os valores possíveis são: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="a96ce-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="a96ce-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="a96ce-161">tokenName</span></span>|<span data-ttu-id="a96ce-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a96ce-162">String</span></span>|<span data-ttu-id="a96ce-163">Nome amigável para Token de Dep</span><span class="sxs-lookup"><span data-stu-id="a96ce-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="a96ce-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a96ce-164">syncedDeviceCount</span></span>|<span data-ttu-id="a96ce-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a96ce-165">Int32</span></span>|<span data-ttu-id="a96ce-166">Obtém contagem de dispositivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="a96ce-166">Gets synced device count</span></span>|
|<span data-ttu-id="a96ce-167">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="a96ce-167">dataSharingConsentGranted</span></span>|<span data-ttu-id="a96ce-168">Booleano</span><span class="sxs-lookup"><span data-stu-id="a96ce-168">Boolean</span></span>|<span data-ttu-id="a96ce-169">Consentimento concedido para compartilhamento de dados com o Serviço de Dep da Apple</span><span class="sxs-lookup"><span data-stu-id="a96ce-169">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="a96ce-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a96ce-170">roleScopeTagIds</span></span>|<span data-ttu-id="a96ce-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a96ce-171">String collection</span></span>|<span data-ttu-id="a96ce-172">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="a96ce-172">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="a96ce-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="a96ce-173">Response</span></span>
<span data-ttu-id="a96ce-174">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a96ce-174">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a96ce-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a96ce-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="a96ce-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a96ce-176">Request</span></span>
<span data-ttu-id="a96ce-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a96ce-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a96ce-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="a96ce-178">Response</span></span>
<span data-ttu-id="a96ce-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a96ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




