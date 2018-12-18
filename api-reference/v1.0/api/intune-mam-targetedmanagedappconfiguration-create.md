---
title: Criar targetedManagedAppConfiguration
description: Cria um novo objeto targetedManagedAppConfiguration.
author: tfitzmac
ms.openlocfilehash: 36183c117ecf3e8d6c48dbd3e92e02a16535dbc5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349032"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="77994-103">Criar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="77994-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="77994-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="77994-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77994-105">Cria um novo objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77994-105">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77994-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77994-106">Prerequisites</span></span>
<span data-ttu-id="77994-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77994-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77994-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77994-109">Permission type</span></span>|<span data-ttu-id="77994-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="77994-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77994-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77994-111">Delegated (work or school account)</span></span>|<span data-ttu-id="77994-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77994-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="77994-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77994-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77994-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77994-114">Not supported.</span></span>|
|<span data-ttu-id="77994-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77994-115">Application</span></span>|<span data-ttu-id="77994-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77994-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77994-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77994-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="77994-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77994-118">Request headers</span></span>
|<span data-ttu-id="77994-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77994-119">Header</span></span>|<span data-ttu-id="77994-120">Valor</span><span class="sxs-lookup"><span data-stu-id="77994-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77994-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="77994-121">Authorization</span></span>|<span data-ttu-id="77994-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77994-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77994-123">Accept</span><span class="sxs-lookup"><span data-stu-id="77994-123">Accept</span></span>|<span data-ttu-id="77994-124">application/json</span><span class="sxs-lookup"><span data-stu-id="77994-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77994-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77994-125">Request body</span></span>
<span data-ttu-id="77994-126">No corpo da solicitação, forneça uma representação JSON do objeto targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="77994-126">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="77994-127">A tabela a seguir mostra as propriedades obrigatórias ao criar targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="77994-127">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="77994-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77994-128">Property</span></span>|<span data-ttu-id="77994-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="77994-129">Type</span></span>|<span data-ttu-id="77994-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="77994-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77994-131">displayName</span><span class="sxs-lookup"><span data-stu-id="77994-131">displayName</span></span>|<span data-ttu-id="77994-132">String</span><span class="sxs-lookup"><span data-stu-id="77994-132">String</span></span>|<span data-ttu-id="77994-133">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="77994-133">Policy display name.</span></span> <span data-ttu-id="77994-134">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="77994-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="77994-135">description</span><span class="sxs-lookup"><span data-stu-id="77994-135">description</span></span>|<span data-ttu-id="77994-136">String</span><span class="sxs-lookup"><span data-stu-id="77994-136">String</span></span>|<span data-ttu-id="77994-137">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="77994-137">The policy's description.</span></span> <span data-ttu-id="77994-138">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="77994-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="77994-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77994-139">createdDateTime</span></span>|<span data-ttu-id="77994-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77994-140">DateTimeOffset</span></span>|<span data-ttu-id="77994-141">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="77994-141">The date and time the policy was created.</span></span> <span data-ttu-id="77994-142">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="77994-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="77994-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77994-143">lastModifiedDateTime</span></span>|<span data-ttu-id="77994-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77994-144">DateTimeOffset</span></span>|<span data-ttu-id="77994-145">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="77994-145">Last time the policy was modified.</span></span> <span data-ttu-id="77994-146">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="77994-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="77994-147">id</span><span class="sxs-lookup"><span data-stu-id="77994-147">id</span></span>|<span data-ttu-id="77994-148">String</span><span class="sxs-lookup"><span data-stu-id="77994-148">String</span></span>|<span data-ttu-id="77994-149">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="77994-149">Key of the entity.</span></span> <span data-ttu-id="77994-150">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="77994-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="77994-151">version</span><span class="sxs-lookup"><span data-stu-id="77994-151">version</span></span>|<span data-ttu-id="77994-152">String</span><span class="sxs-lookup"><span data-stu-id="77994-152">String</span></span>|<span data-ttu-id="77994-153">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="77994-153">Version of the entity.</span></span> <span data-ttu-id="77994-154">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="77994-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="77994-155">customSettings</span><span class="sxs-lookup"><span data-stu-id="77994-155">customSettings</span></span>|<span data-ttu-id="77994-156">Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="77994-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="77994-157">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77994-157">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="77994-158">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="77994-158">deployedAppCount</span></span>|<span data-ttu-id="77994-159">Int32</span><span class="sxs-lookup"><span data-stu-id="77994-159">Int32</span></span>|<span data-ttu-id="77994-160">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="77994-160">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="77994-161">isAssigned</span><span class="sxs-lookup"><span data-stu-id="77994-161">isAssigned</span></span>|<span data-ttu-id="77994-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="77994-162">Boolean</span></span>|<span data-ttu-id="77994-163">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="77994-163">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="77994-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="77994-164">Response</span></span>
<span data-ttu-id="77994-165">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77994-165">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77994-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77994-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="77994-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77994-167">Request</span></span>
<span data-ttu-id="77994-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77994-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="77994-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="77994-169">Response</span></span>
<span data-ttu-id="77994-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77994-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



