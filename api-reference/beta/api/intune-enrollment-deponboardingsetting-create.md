---
title: Criar depOnboardingSetting
description: Criar um novo objeto depOnboardingSetting.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9abf9fbb618c76960e0ffecde8d61ccb6ce1afd7
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943926"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="2c7a1-103">Criar depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="2c7a1-103">Create depOnboardingSetting</span></span>

> <span data-ttu-id="2c7a1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c7a1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c7a1-106">Criar um novo objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="2c7a1-106">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c7a1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2c7a1-107">Prerequisites</span></span>
<span data-ttu-id="2c7a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c7a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c7a1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c7a1-110">Permission type</span></span>|<span data-ttu-id="2c7a1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2c7a1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c7a1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c7a1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c7a1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c7a1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2c7a1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c7a1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c7a1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-115">Not supported.</span></span>|
|<span data-ttu-id="2c7a1-116">Application</span><span class="sxs-lookup"><span data-stu-id="2c7a1-116">Application</span></span>|<span data-ttu-id="2c7a1-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c7a1-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c7a1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c7a1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="2c7a1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c7a1-119">Request headers</span></span>
|<span data-ttu-id="2c7a1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2c7a1-120">Header</span></span>|<span data-ttu-id="2c7a1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2c7a1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c7a1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c7a1-122">Authorization</span></span>|<span data-ttu-id="2c7a1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c7a1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2c7a1-124">Accept</span></span>|<span data-ttu-id="2c7a1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c7a1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c7a1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c7a1-126">Request body</span></span>
<span data-ttu-id="2c7a1-127">No corpo da solicitação, forneça uma representação JSON do objeto depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-127">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="2c7a1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-128">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="2c7a1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c7a1-129">Property</span></span>|<span data-ttu-id="2c7a1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c7a1-130">Type</span></span>|<span data-ttu-id="2c7a1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c7a1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c7a1-132">id</span><span class="sxs-lookup"><span data-stu-id="2c7a1-132">id</span></span>|<span data-ttu-id="2c7a1-133">String</span><span class="sxs-lookup"><span data-stu-id="2c7a1-133">String</span></span>|<span data-ttu-id="2c7a1-134">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-134">UUID for the object</span></span>|
|<span data-ttu-id="2c7a1-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="2c7a1-135">appleIdentifier</span></span>|<span data-ttu-id="2c7a1-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c7a1-136">String</span></span>|<span data-ttu-id="2c7a1-137">A ID da Apple usada para obter o token atual.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-137">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="2c7a1-138">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2c7a1-138">tokenExpirationDateTime</span></span>|<span data-ttu-id="2c7a1-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c7a1-139">DateTimeOffset</span></span>|<span data-ttu-id="2c7a1-140">Quando o token expirará.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-140">When the token will expire.</span></span>|
|<span data-ttu-id="2c7a1-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c7a1-141">lastModifiedDateTime</span></span>|<span data-ttu-id="2c7a1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c7a1-142">DateTimeOffset</span></span>|<span data-ttu-id="2c7a1-143">Quando o serviço foi integrado.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-143">When the service was onboarded.</span></span>|
|<span data-ttu-id="2c7a1-144">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2c7a1-144">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="2c7a1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c7a1-145">DateTimeOffset</span></span>|<span data-ttu-id="2c7a1-146">Quando o serviço última syned com o Intune</span><span class="sxs-lookup"><span data-stu-id="2c7a1-146">When the service last syned with Intune</span></span>|
|<span data-ttu-id="2c7a1-147">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="2c7a1-147">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="2c7a1-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c7a1-148">DateTimeOffset</span></span>|<span data-ttu-id="2c7a1-149">Quando o Intune solicitou uma sincronização pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-149">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="2c7a1-150">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="2c7a1-150">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="2c7a1-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c7a1-151">Boolean</span></span>|<span data-ttu-id="2c7a1-152">Se o compartilhamento de token DEP está ou não habilitado com o serviço de sincronização de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-152">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="2c7a1-153">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="2c7a1-153">lastSyncErrorCode</span></span>|<span data-ttu-id="2c7a1-154">Int32</span><span class="sxs-lookup"><span data-stu-id="2c7a1-154">Int32</span></span>|<span data-ttu-id="2c7a1-155">Código de erro relatado pela Apple durante a última sincronização de Dep.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-155">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="2c7a1-156">TokenType</span><span class="sxs-lookup"><span data-stu-id="2c7a1-156">tokenType</span></span>|[<span data-ttu-id="2c7a1-157">depTokenType</span><span class="sxs-lookup"><span data-stu-id="2c7a1-157">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="2c7a1-158">Obtém ou define o tipo de token Dep.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-158">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="2c7a1-159">Os valores possíveis são: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-159">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="2c7a1-160">tokenname</span><span class="sxs-lookup"><span data-stu-id="2c7a1-160">tokenName</span></span>|<span data-ttu-id="2c7a1-161">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2c7a1-161">String</span></span>|<span data-ttu-id="2c7a1-162">Nome amigável para token Dep</span><span class="sxs-lookup"><span data-stu-id="2c7a1-162">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="2c7a1-163">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2c7a1-163">syncedDeviceCount</span></span>|<span data-ttu-id="2c7a1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="2c7a1-164">Int32</span></span>|<span data-ttu-id="2c7a1-165">Obtém a contagem de dispositivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="2c7a1-165">Gets synced device count</span></span>|
|<span data-ttu-id="2c7a1-166">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="2c7a1-166">dataSharingConsentGranted</span></span>|<span data-ttu-id="2c7a1-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c7a1-167">Boolean</span></span>|<span data-ttu-id="2c7a1-168">Consentimento concedido para compartilhamento de dados com o serviço Apple Dep</span><span class="sxs-lookup"><span data-stu-id="2c7a1-168">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="2c7a1-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2c7a1-169">roleScopeTagIds</span></span>|<span data-ttu-id="2c7a1-170">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c7a1-170">String collection</span></span>|<span data-ttu-id="2c7a1-171">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="2c7a1-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c7a1-172">Response</span></span>
<span data-ttu-id="2c7a1-173">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-173">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c7a1-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c7a1-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c7a1-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c7a1-175">Request</span></span>
<span data-ttu-id="2c7a1-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2c7a1-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c7a1-177">Response</span></span>
<span data-ttu-id="2c7a1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c7a1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





