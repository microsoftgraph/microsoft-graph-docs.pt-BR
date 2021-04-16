---
title: Atualizar targetedManagedAppConfiguration
description: Atualizar as propriedades de um objeto targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40d96d22dc5437ce07e07f24e1c219802a674ad5
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868131"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="ef518-103">Atualizar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ef518-103">Update targetedManagedAppConfiguration</span></span>

<span data-ttu-id="ef518-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef518-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef518-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ef518-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef518-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef518-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef518-107">Atualizar as propriedades de um objeto [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef518-107">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef518-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef518-108">Prerequisites</span></span>
<span data-ttu-id="ef518-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef518-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef518-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef518-111">Permission type</span></span>|<span data-ttu-id="ef518-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef518-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef518-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef518-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ef518-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="ef518-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="ef518-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef518-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="ef518-116">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="ef518-116">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="ef518-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef518-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ef518-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef518-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef518-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef518-119">Not supported.</span></span>|
|<span data-ttu-id="ef518-120">Application</span><span class="sxs-lookup"><span data-stu-id="ef518-120">Application</span></span>||
| <span data-ttu-id="ef518-121">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="ef518-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="ef518-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef518-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="ef518-123">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="ef518-123">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="ef518-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef518-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef518-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef518-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ef518-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef518-126">Request headers</span></span>
|<span data-ttu-id="ef518-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef518-127">Header</span></span>|<span data-ttu-id="ef518-128">Valor</span><span class="sxs-lookup"><span data-stu-id="ef518-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef518-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef518-129">Authorization</span></span>|<span data-ttu-id="ef518-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef518-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef518-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef518-131">Accept</span></span>|<span data-ttu-id="ef518-132">application/json</span><span class="sxs-lookup"><span data-stu-id="ef518-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef518-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef518-133">Request body</span></span>
<span data-ttu-id="ef518-134">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef518-134">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="ef518-135">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef518-135">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="ef518-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef518-136">Property</span></span>|<span data-ttu-id="ef518-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef518-137">Type</span></span>|<span data-ttu-id="ef518-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef518-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef518-139">displayName</span><span class="sxs-lookup"><span data-stu-id="ef518-139">displayName</span></span>|<span data-ttu-id="ef518-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef518-140">String</span></span>|<span data-ttu-id="ef518-141">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="ef518-141">Policy display name.</span></span> <span data-ttu-id="ef518-142">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ef518-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ef518-143">description</span><span class="sxs-lookup"><span data-stu-id="ef518-143">description</span></span>|<span data-ttu-id="ef518-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef518-144">String</span></span>|<span data-ttu-id="ef518-145">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="ef518-145">The policy's description.</span></span> <span data-ttu-id="ef518-146">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ef518-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ef518-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef518-147">createdDateTime</span></span>|<span data-ttu-id="ef518-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef518-148">DateTimeOffset</span></span>|<span data-ttu-id="ef518-149">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="ef518-149">The date and time the policy was created.</span></span> <span data-ttu-id="ef518-150">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ef518-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ef518-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef518-151">lastModifiedDateTime</span></span>|<span data-ttu-id="ef518-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef518-152">DateTimeOffset</span></span>|<span data-ttu-id="ef518-153">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="ef518-153">Last time the policy was modified.</span></span> <span data-ttu-id="ef518-154">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ef518-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ef518-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef518-155">roleScopeTagIds</span></span>|<span data-ttu-id="ef518-156">Coleção String</span><span class="sxs-lookup"><span data-stu-id="ef518-156">String collection</span></span>|<span data-ttu-id="ef518-157">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="ef518-157">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ef518-158">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ef518-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ef518-159">id</span><span class="sxs-lookup"><span data-stu-id="ef518-159">id</span></span>|<span data-ttu-id="ef518-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef518-160">String</span></span>|<span data-ttu-id="ef518-161">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ef518-161">Key of the entity.</span></span> <span data-ttu-id="ef518-162">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ef518-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ef518-163">version</span><span class="sxs-lookup"><span data-stu-id="ef518-163">version</span></span>|<span data-ttu-id="ef518-164">String</span><span class="sxs-lookup"><span data-stu-id="ef518-164">String</span></span>|<span data-ttu-id="ef518-165">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="ef518-165">Version of the entity.</span></span> <span data-ttu-id="ef518-166">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ef518-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ef518-167">customSettings</span><span class="sxs-lookup"><span data-stu-id="ef518-167">customSettings</span></span>|<span data-ttu-id="ef518-168">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ef518-168">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ef518-169">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef518-169">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="ef518-170">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="ef518-170">deployedAppCount</span></span>|<span data-ttu-id="ef518-171">Int32</span><span class="sxs-lookup"><span data-stu-id="ef518-171">Int32</span></span>|<span data-ttu-id="ef518-172">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="ef518-172">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="ef518-173">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ef518-173">isAssigned</span></span>|<span data-ttu-id="ef518-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef518-174">Boolean</span></span>|<span data-ttu-id="ef518-175">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="ef518-175">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="ef518-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef518-176">Response</span></span>
<span data-ttu-id="ef518-177">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef518-177">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef518-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef518-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef518-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef518-179">Request</span></span>
<span data-ttu-id="ef518-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef518-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ef518-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef518-181">Response</span></span>
<span data-ttu-id="ef518-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef518-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







