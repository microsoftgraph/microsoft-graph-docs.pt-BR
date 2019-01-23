---
title: Atualizar targetedManagedAppConfiguration
description: Atualizar as propriedades de um objeto targetedManagedAppConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eded21015054073b6f6711faecd5c01da52fece0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403690"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="ee5c6-103">Atualizar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee5c6-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="ee5c6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ee5c6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee5c6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee5c6-107">Atualizar as propriedades de um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee5c6-107">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee5c6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ee5c6-108">Prerequisites</span></span>
<span data-ttu-id="ee5c6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ee5c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ee5c6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee5c6-111">Permission type</span></span>|<span data-ttu-id="ee5c6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ee5c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee5c6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee5c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee5c6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee5c6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ee5c6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee5c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee5c6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-116">Not supported.</span></span>|
|<span data-ttu-id="ee5c6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee5c6-117">Application</span></span>|<span data-ttu-id="ee5c6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee5c6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee5c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ee5c6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee5c6-120">Request headers</span></span>
|<span data-ttu-id="ee5c6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee5c6-121">Header</span></span>|<span data-ttu-id="ee5c6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ee5c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee5c6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee5c6-123">Authorization</span></span>|<span data-ttu-id="ee5c6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee5c6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ee5c6-125">Accept</span></span>|<span data-ttu-id="ee5c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee5c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee5c6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee5c6-127">Request body</span></span>
<span data-ttu-id="ee5c6-128">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee5c6-128">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="ee5c6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee5c6-129">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="ee5c6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee5c6-130">Property</span></span>|<span data-ttu-id="ee5c6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee5c6-131">Type</span></span>|<span data-ttu-id="ee5c6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee5c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee5c6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ee5c6-133">displayName</span></span>|<span data-ttu-id="ee5c6-134">String</span><span class="sxs-lookup"><span data-stu-id="ee5c6-134">String</span></span>|<span data-ttu-id="ee5c6-135">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-135">Policy display name.</span></span> <span data-ttu-id="ee5c6-136">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ee5c6-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ee5c6-137">description</span><span class="sxs-lookup"><span data-stu-id="ee5c6-137">description</span></span>|<span data-ttu-id="ee5c6-138">String</span><span class="sxs-lookup"><span data-stu-id="ee5c6-138">String</span></span>|<span data-ttu-id="ee5c6-139">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-139">The policy's description.</span></span> <span data-ttu-id="ee5c6-140">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ee5c6-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ee5c6-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee5c6-141">createdDateTime</span></span>|<span data-ttu-id="ee5c6-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee5c6-142">DateTimeOffset</span></span>|<span data-ttu-id="ee5c6-143">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-143">The date and time the policy was created.</span></span> <span data-ttu-id="ee5c6-144">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ee5c6-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ee5c6-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee5c6-145">lastModifiedDateTime</span></span>|<span data-ttu-id="ee5c6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee5c6-146">DateTimeOffset</span></span>|<span data-ttu-id="ee5c6-147">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-147">Last time the policy was modified.</span></span> <span data-ttu-id="ee5c6-148">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ee5c6-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ee5c6-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ee5c6-149">roleScopeTagIds</span></span>|<span data-ttu-id="ee5c6-150">String collection</span><span class="sxs-lookup"><span data-stu-id="ee5c6-150">String collection</span></span>|<span data-ttu-id="ee5c6-151">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ee5c6-152">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ee5c6-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ee5c6-153">id</span><span class="sxs-lookup"><span data-stu-id="ee5c6-153">id</span></span>|<span data-ttu-id="ee5c6-154">String</span><span class="sxs-lookup"><span data-stu-id="ee5c6-154">String</span></span>|<span data-ttu-id="ee5c6-155">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-155">Key of the entity.</span></span> <span data-ttu-id="ee5c6-156">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ee5c6-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ee5c6-157">version</span><span class="sxs-lookup"><span data-stu-id="ee5c6-157">version</span></span>|<span data-ttu-id="ee5c6-158">String</span><span class="sxs-lookup"><span data-stu-id="ee5c6-158">String</span></span>|<span data-ttu-id="ee5c6-159">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-159">Version of the entity.</span></span> <span data-ttu-id="ee5c6-160">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ee5c6-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ee5c6-161">customSettings</span><span class="sxs-lookup"><span data-stu-id="ee5c6-161">customSettings</span></span>|<span data-ttu-id="ee5c6-162">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ee5c6-162">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ee5c6-163">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ee5c6-163">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="ee5c6-164">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="ee5c6-164">deployedAppCount</span></span>|<span data-ttu-id="ee5c6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ee5c6-165">Int32</span></span>|<span data-ttu-id="ee5c6-166">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-166">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="ee5c6-167">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ee5c6-167">isAssigned</span></span>|<span data-ttu-id="ee5c6-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee5c6-168">Boolean</span></span>|<span data-ttu-id="ee5c6-169">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-169">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="ee5c6-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee5c6-170">Response</span></span>
<span data-ttu-id="ee5c6-171">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-171">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee5c6-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee5c6-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee5c6-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee5c6-173">Request</span></span>
<span data-ttu-id="ee5c6-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee5c6-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee5c6-175">Response</span></span>
<span data-ttu-id="ee5c6-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee5c6-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




