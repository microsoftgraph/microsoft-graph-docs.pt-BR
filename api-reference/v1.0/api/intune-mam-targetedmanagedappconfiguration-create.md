---
title: Criar targetedManagedAppConfiguration
description: Cria um novo objeto targetedManagedAppConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58aa199b2f1a75b4fe6952bf182e96ce84791034
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512976"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="30beb-103">Criar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="30beb-103">Create targetedManagedAppConfiguration</span></span>

<span data-ttu-id="30beb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30beb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30beb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30beb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30beb-106">Cria um novo objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30beb-106">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30beb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30beb-107">Prerequisites</span></span>
<span data-ttu-id="30beb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30beb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30beb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30beb-110">Permission type</span></span>|<span data-ttu-id="30beb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30beb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30beb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30beb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30beb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30beb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30beb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30beb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30beb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30beb-115">Not supported.</span></span>|
|<span data-ttu-id="30beb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30beb-116">Application</span></span>|<span data-ttu-id="30beb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30beb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30beb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30beb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="30beb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30beb-119">Request headers</span></span>
|<span data-ttu-id="30beb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30beb-120">Header</span></span>|<span data-ttu-id="30beb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="30beb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30beb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="30beb-122">Authorization</span></span>|<span data-ttu-id="30beb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30beb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30beb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30beb-124">Accept</span></span>|<span data-ttu-id="30beb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30beb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30beb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30beb-126">Request body</span></span>
<span data-ttu-id="30beb-127">No corpo da solicitação, forneça uma representação JSON do objeto targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="30beb-127">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="30beb-128">A tabela a seguir mostra as propriedades obrigatórias ao criar targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="30beb-128">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="30beb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30beb-129">Property</span></span>|<span data-ttu-id="30beb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="30beb-130">Type</span></span>|<span data-ttu-id="30beb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="30beb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30beb-132">displayName</span><span class="sxs-lookup"><span data-stu-id="30beb-132">displayName</span></span>|<span data-ttu-id="30beb-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30beb-133">String</span></span>|<span data-ttu-id="30beb-134">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="30beb-134">Policy display name.</span></span> <span data-ttu-id="30beb-135">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="30beb-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="30beb-136">description</span><span class="sxs-lookup"><span data-stu-id="30beb-136">description</span></span>|<span data-ttu-id="30beb-137">String</span><span class="sxs-lookup"><span data-stu-id="30beb-137">String</span></span>|<span data-ttu-id="30beb-138">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="30beb-138">The policy's description.</span></span> <span data-ttu-id="30beb-139">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="30beb-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="30beb-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30beb-140">createdDateTime</span></span>|<span data-ttu-id="30beb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30beb-141">DateTimeOffset</span></span>|<span data-ttu-id="30beb-142">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="30beb-142">The date and time the policy was created.</span></span> <span data-ttu-id="30beb-143">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="30beb-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="30beb-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30beb-144">lastModifiedDateTime</span></span>|<span data-ttu-id="30beb-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30beb-145">DateTimeOffset</span></span>|<span data-ttu-id="30beb-146">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="30beb-146">Last time the policy was modified.</span></span> <span data-ttu-id="30beb-147">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="30beb-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="30beb-148">id</span><span class="sxs-lookup"><span data-stu-id="30beb-148">id</span></span>|<span data-ttu-id="30beb-149">String</span><span class="sxs-lookup"><span data-stu-id="30beb-149">String</span></span>|<span data-ttu-id="30beb-150">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="30beb-150">Key of the entity.</span></span> <span data-ttu-id="30beb-151">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="30beb-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="30beb-152">version</span><span class="sxs-lookup"><span data-stu-id="30beb-152">version</span></span>|<span data-ttu-id="30beb-153">String</span><span class="sxs-lookup"><span data-stu-id="30beb-153">String</span></span>|<span data-ttu-id="30beb-154">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="30beb-154">Version of the entity.</span></span> <span data-ttu-id="30beb-155">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="30beb-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="30beb-156">customSettings</span><span class="sxs-lookup"><span data-stu-id="30beb-156">customSettings</span></span>|<span data-ttu-id="30beb-157">Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="30beb-157">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="30beb-158">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30beb-158">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="30beb-159">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="30beb-159">deployedAppCount</span></span>|<span data-ttu-id="30beb-160">Int32</span><span class="sxs-lookup"><span data-stu-id="30beb-160">Int32</span></span>|<span data-ttu-id="30beb-161">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="30beb-161">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="30beb-162">isAssigned</span><span class="sxs-lookup"><span data-stu-id="30beb-162">isAssigned</span></span>|<span data-ttu-id="30beb-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="30beb-163">Boolean</span></span>|<span data-ttu-id="30beb-164">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="30beb-164">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="30beb-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="30beb-165">Response</span></span>
<span data-ttu-id="30beb-166">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30beb-166">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30beb-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30beb-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="30beb-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30beb-168">Request</span></span>
<span data-ttu-id="30beb-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30beb-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 388

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="30beb-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="30beb-170">Response</span></span>
<span data-ttu-id="30beb-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30beb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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




