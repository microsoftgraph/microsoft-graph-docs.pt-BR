---
title: Criar targetedManagedAppConfiguration
description: Cria um novo objeto targetedManagedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b3117e5122004c01bcb3d94c6d59ac337a9b362
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465341"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="65922-103">Criar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="65922-103">Create targetedManagedAppConfiguration</span></span>

<span data-ttu-id="65922-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65922-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65922-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65922-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65922-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65922-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65922-107">Cria um novo objeto [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65922-107">Create a new [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65922-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="65922-108">Prerequisites</span></span>
<span data-ttu-id="65922-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65922-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65922-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65922-111">Permission type</span></span>|<span data-ttu-id="65922-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="65922-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65922-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65922-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="65922-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="65922-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="65922-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65922-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="65922-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="65922-116">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="65922-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65922-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="65922-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65922-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65922-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65922-119">Not supported.</span></span>|
|<span data-ttu-id="65922-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65922-120">Application</span></span>||
| <span data-ttu-id="65922-121">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="65922-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="65922-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65922-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="65922-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="65922-123">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="65922-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65922-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65922-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65922-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="65922-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65922-126">Request headers</span></span>
|<span data-ttu-id="65922-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65922-127">Header</span></span>|<span data-ttu-id="65922-128">Valor</span><span class="sxs-lookup"><span data-stu-id="65922-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65922-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="65922-129">Authorization</span></span>|<span data-ttu-id="65922-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65922-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65922-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="65922-131">Accept</span></span>|<span data-ttu-id="65922-132">application/json</span><span class="sxs-lookup"><span data-stu-id="65922-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65922-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65922-133">Request body</span></span>
<span data-ttu-id="65922-134">No corpo da solicitação, forneça uma representação JSON do objeto targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="65922-134">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="65922-135">A tabela a seguir mostra as propriedades obrigatórias ao criar targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="65922-135">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="65922-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65922-136">Property</span></span>|<span data-ttu-id="65922-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="65922-137">Type</span></span>|<span data-ttu-id="65922-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="65922-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65922-139">displayName</span><span class="sxs-lookup"><span data-stu-id="65922-139">displayName</span></span>|<span data-ttu-id="65922-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65922-140">String</span></span>|<span data-ttu-id="65922-141">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="65922-141">Policy display name.</span></span> <span data-ttu-id="65922-142">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65922-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="65922-143">description</span><span class="sxs-lookup"><span data-stu-id="65922-143">description</span></span>|<span data-ttu-id="65922-144">String</span><span class="sxs-lookup"><span data-stu-id="65922-144">String</span></span>|<span data-ttu-id="65922-145">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="65922-145">The policy's description.</span></span> <span data-ttu-id="65922-146">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65922-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="65922-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65922-147">createdDateTime</span></span>|<span data-ttu-id="65922-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65922-148">DateTimeOffset</span></span>|<span data-ttu-id="65922-149">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="65922-149">The date and time the policy was created.</span></span> <span data-ttu-id="65922-150">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65922-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="65922-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65922-151">lastModifiedDateTime</span></span>|<span data-ttu-id="65922-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65922-152">DateTimeOffset</span></span>|<span data-ttu-id="65922-153">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="65922-153">Last time the policy was modified.</span></span> <span data-ttu-id="65922-154">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65922-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="65922-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="65922-155">roleScopeTagIds</span></span>|<span data-ttu-id="65922-156">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="65922-156">String collection</span></span>|<span data-ttu-id="65922-157">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="65922-157">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="65922-158">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65922-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="65922-159">id</span><span class="sxs-lookup"><span data-stu-id="65922-159">id</span></span>|<span data-ttu-id="65922-160">String</span><span class="sxs-lookup"><span data-stu-id="65922-160">String</span></span>|<span data-ttu-id="65922-161">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="65922-161">Key of the entity.</span></span> <span data-ttu-id="65922-162">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65922-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="65922-163">version</span><span class="sxs-lookup"><span data-stu-id="65922-163">version</span></span>|<span data-ttu-id="65922-164">String</span><span class="sxs-lookup"><span data-stu-id="65922-164">String</span></span>|<span data-ttu-id="65922-165">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="65922-165">Version of the entity.</span></span> <span data-ttu-id="65922-166">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="65922-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="65922-167">customSettings</span><span class="sxs-lookup"><span data-stu-id="65922-167">customSettings</span></span>|<span data-ttu-id="65922-168">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="65922-168">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="65922-169">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65922-169">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="65922-170">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="65922-170">deployedAppCount</span></span>|<span data-ttu-id="65922-171">Int32</span><span class="sxs-lookup"><span data-stu-id="65922-171">Int32</span></span>|<span data-ttu-id="65922-172">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="65922-172">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="65922-173">isAssigned</span><span class="sxs-lookup"><span data-stu-id="65922-173">isAssigned</span></span>|<span data-ttu-id="65922-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="65922-174">Boolean</span></span>|<span data-ttu-id="65922-175">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="65922-175">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="65922-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="65922-176">Response</span></span>
<span data-ttu-id="65922-177">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65922-177">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65922-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65922-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="65922-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65922-179">Request</span></span>
<span data-ttu-id="65922-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65922-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
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

### <a name="response"></a><span data-ttu-id="65922-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="65922-181">Response</span></span>
<span data-ttu-id="65922-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65922-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






