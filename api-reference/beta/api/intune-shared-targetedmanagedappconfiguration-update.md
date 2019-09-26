---
title: Atualizar targetedManagedAppConfiguration
description: Atualizar as propriedades de um objeto targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0fced4d51de11bfbb95b5404233ed3a41d4e1880
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199529"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="1d472-103">Atualizar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1d472-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="1d472-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d472-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d472-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d472-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d472-106">Atualizar as propriedades de um objeto [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d472-106">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d472-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1d472-107">Prerequisites</span></span>
<span data-ttu-id="1d472-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d472-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d472-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d472-110">Permission type</span></span>|<span data-ttu-id="1d472-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1d472-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d472-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d472-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1d472-113">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="1d472-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="1d472-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d472-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="1d472-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="1d472-115">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="1d472-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d472-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1d472-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d472-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d472-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d472-118">Not supported.</span></span>|
|<span data-ttu-id="1d472-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d472-119">Application</span></span>||
| <span data-ttu-id="1d472-120">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="1d472-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="1d472-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d472-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="1d472-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="1d472-122">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="1d472-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d472-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d472-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d472-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1d472-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d472-125">Request headers</span></span>
|<span data-ttu-id="1d472-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d472-126">Header</span></span>|<span data-ttu-id="1d472-127">Valor</span><span class="sxs-lookup"><span data-stu-id="1d472-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d472-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d472-128">Authorization</span></span>|<span data-ttu-id="1d472-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d472-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d472-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1d472-130">Accept</span></span>|<span data-ttu-id="1d472-131">application/json</span><span class="sxs-lookup"><span data-stu-id="1d472-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d472-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d472-132">Request body</span></span>
<span data-ttu-id="1d472-133">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d472-133">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="1d472-134">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d472-134">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="1d472-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d472-135">Property</span></span>|<span data-ttu-id="1d472-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d472-136">Type</span></span>|<span data-ttu-id="1d472-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d472-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d472-138">displayName</span><span class="sxs-lookup"><span data-stu-id="1d472-138">displayName</span></span>|<span data-ttu-id="1d472-139">String</span><span class="sxs-lookup"><span data-stu-id="1d472-139">String</span></span>|<span data-ttu-id="1d472-140">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="1d472-140">Policy display name.</span></span> <span data-ttu-id="1d472-141">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1d472-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1d472-142">descrição</span><span class="sxs-lookup"><span data-stu-id="1d472-142">description</span></span>|<span data-ttu-id="1d472-143">String</span><span class="sxs-lookup"><span data-stu-id="1d472-143">String</span></span>|<span data-ttu-id="1d472-144">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="1d472-144">The policy's description.</span></span> <span data-ttu-id="1d472-145">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1d472-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1d472-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d472-146">createdDateTime</span></span>|<span data-ttu-id="1d472-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d472-147">DateTimeOffset</span></span>|<span data-ttu-id="1d472-148">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="1d472-148">The date and time the policy was created.</span></span> <span data-ttu-id="1d472-149">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1d472-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1d472-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d472-150">lastModifiedDateTime</span></span>|<span data-ttu-id="1d472-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d472-151">DateTimeOffset</span></span>|<span data-ttu-id="1d472-152">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="1d472-152">Last time the policy was modified.</span></span> <span data-ttu-id="1d472-153">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1d472-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1d472-154">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1d472-154">roleScopeTagIds</span></span>|<span data-ttu-id="1d472-155">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d472-155">String collection</span></span>|<span data-ttu-id="1d472-156">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="1d472-156">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1d472-157">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1d472-157">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1d472-158">id</span><span class="sxs-lookup"><span data-stu-id="1d472-158">id</span></span>|<span data-ttu-id="1d472-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d472-159">String</span></span>|<span data-ttu-id="1d472-160">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1d472-160">Key of the entity.</span></span> <span data-ttu-id="1d472-161">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1d472-161">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1d472-162">version</span><span class="sxs-lookup"><span data-stu-id="1d472-162">version</span></span>|<span data-ttu-id="1d472-163">String</span><span class="sxs-lookup"><span data-stu-id="1d472-163">String</span></span>|<span data-ttu-id="1d472-164">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="1d472-164">Version of the entity.</span></span> <span data-ttu-id="1d472-165">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1d472-165">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1d472-166">customSettings</span><span class="sxs-lookup"><span data-stu-id="1d472-166">customSettings</span></span>|<span data-ttu-id="1d472-167">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="1d472-167">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="1d472-168">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d472-168">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="1d472-169">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="1d472-169">deployedAppCount</span></span>|<span data-ttu-id="1d472-170">Int32</span><span class="sxs-lookup"><span data-stu-id="1d472-170">Int32</span></span>|<span data-ttu-id="1d472-171">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="1d472-171">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="1d472-172">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1d472-172">isAssigned</span></span>|<span data-ttu-id="1d472-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d472-173">Boolean</span></span>|<span data-ttu-id="1d472-174">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="1d472-174">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="1d472-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d472-175">Response</span></span>
<span data-ttu-id="1d472-176">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d472-176">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d472-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d472-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d472-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d472-178">Request</span></span>
<span data-ttu-id="1d472-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d472-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 450

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="1d472-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d472-180">Response</span></span>
<span data-ttu-id="1d472-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d472-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 622

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```




