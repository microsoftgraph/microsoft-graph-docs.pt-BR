---
title: Criar raProfileDatabaseEntity
description: Criar um novo objeto raProfileDatabaseEntity.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb892f1a64dd1223956f3fda73a6aeb8512edf00
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124180"
---
# <a name="create-raprofiledatabaseentity"></a><span data-ttu-id="d238d-103">Criar raProfileDatabaseEntity</span><span class="sxs-lookup"><span data-stu-id="d238d-103">Create raProfileDatabaseEntity</span></span>

<span data-ttu-id="d238d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d238d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d238d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d238d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d238d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d238d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d238d-107">Criar um novo objeto [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) .</span><span class="sxs-lookup"><span data-stu-id="d238d-107">Create a new [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d238d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d238d-108">Prerequisites</span></span>
<span data-ttu-id="d238d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d238d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d238d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d238d-111">Permission type</span></span>|<span data-ttu-id="d238d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d238d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d238d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d238d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d238d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d238d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d238d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d238d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d238d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d238d-116">Not supported.</span></span>|
|<span data-ttu-id="d238d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d238d-117">Application</span></span>|<span data-ttu-id="d238d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d238d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d238d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d238d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /resourceAccessProfileEntities
```

## <a name="request-headers"></a><span data-ttu-id="d238d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d238d-120">Request headers</span></span>
|<span data-ttu-id="d238d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d238d-121">Header</span></span>|<span data-ttu-id="d238d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d238d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d238d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d238d-123">Authorization</span></span>|<span data-ttu-id="d238d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d238d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d238d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d238d-125">Accept</span></span>|<span data-ttu-id="d238d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d238d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d238d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d238d-127">Request body</span></span>
<span data-ttu-id="d238d-128">No corpo da solicitação, forneça uma representação JSON do objeto raProfileDatabaseEntity.</span><span class="sxs-lookup"><span data-stu-id="d238d-128">In the request body, supply a JSON representation for the raProfileDatabaseEntity object.</span></span>

<span data-ttu-id="d238d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar raProfileDatabaseEntity.</span><span class="sxs-lookup"><span data-stu-id="d238d-129">The following table shows the properties that are required when you create the raProfileDatabaseEntity.</span></span>

|<span data-ttu-id="d238d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d238d-130">Property</span></span>|<span data-ttu-id="d238d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d238d-131">Type</span></span>|<span data-ttu-id="d238d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d238d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d238d-133">versão</span><span class="sxs-lookup"><span data-stu-id="d238d-133">version</span></span>|<span data-ttu-id="d238d-134">Int32</span><span class="sxs-lookup"><span data-stu-id="d238d-134">Int32</span></span>|<span data-ttu-id="d238d-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-135">Not yet documented</span></span>|
|<span data-ttu-id="d238d-136">isDeleted</span><span class="sxs-lookup"><span data-stu-id="d238d-136">isDeleted</span></span>|<span data-ttu-id="d238d-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="d238d-137">Boolean</span></span>|<span data-ttu-id="d238d-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-138">Not yet documented</span></span>|
|<span data-ttu-id="d238d-139">softDeletedTime</span><span class="sxs-lookup"><span data-stu-id="d238d-139">softDeletedTime</span></span>|<span data-ttu-id="d238d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d238d-140">DateTimeOffset</span></span>|<span data-ttu-id="d238d-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-141">Not yet documented</span></span>|
|<span data-ttu-id="d238d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="d238d-142">displayName</span></span>|<span data-ttu-id="d238d-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d238d-143">String</span></span>|<span data-ttu-id="d238d-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-144">Not yet documented</span></span>|
|<span data-ttu-id="d238d-145">linkedProfileIds</span><span class="sxs-lookup"><span data-stu-id="d238d-145">linkedProfileIds</span></span>|<span data-ttu-id="d238d-146">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="d238d-146">Guid collection</span></span>|<span data-ttu-id="d238d-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-147">Not yet documented</span></span>|
|<span data-ttu-id="d238d-148">outfiletypename</span><span class="sxs-lookup"><span data-stu-id="d238d-148">profileTypeName</span></span>|<span data-ttu-id="d238d-149">String</span><span class="sxs-lookup"><span data-stu-id="d238d-149">String</span></span>|<span data-ttu-id="d238d-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-150">Not yet documented</span></span>|
|<span data-ttu-id="d238d-151">profileBody</span><span class="sxs-lookup"><span data-stu-id="d238d-151">profileBody</span></span>|<span data-ttu-id="d238d-152">String</span><span class="sxs-lookup"><span data-stu-id="d238d-152">String</span></span>|<span data-ttu-id="d238d-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-153">Not yet documented</span></span>|
|<span data-ttu-id="d238d-154">profileBodyHash</span><span class="sxs-lookup"><span data-stu-id="d238d-154">profileBodyHash</span></span>|<span data-ttu-id="d238d-155">String</span><span class="sxs-lookup"><span data-stu-id="d238d-155">String</span></span>|<span data-ttu-id="d238d-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-156">Not yet documented</span></span>|
|<span data-ttu-id="d238d-157">platformType</span><span class="sxs-lookup"><span data-stu-id="d238d-157">platformType</span></span>|<span data-ttu-id="d238d-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d238d-158">Int32</span></span>|<span data-ttu-id="d238d-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-159">Not yet documented</span></span>|
|<span data-ttu-id="d238d-160">transformedProfileBody</span><span class="sxs-lookup"><span data-stu-id="d238d-160">transformedProfileBody</span></span>|<span data-ttu-id="d238d-161">String</span><span class="sxs-lookup"><span data-stu-id="d238d-161">String</span></span>|<span data-ttu-id="d238d-162">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-162">Not yet documented</span></span>|
|<span data-ttu-id="d238d-163">transformedProfileBodyHash</span><span class="sxs-lookup"><span data-stu-id="d238d-163">transformedProfileBodyHash</span></span>|<span data-ttu-id="d238d-164">String</span><span class="sxs-lookup"><span data-stu-id="d238d-164">String</span></span>|<span data-ttu-id="d238d-165">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-165">Not yet documented</span></span>|
|<span data-ttu-id="d238d-166">tenantId</span><span class="sxs-lookup"><span data-stu-id="d238d-166">tenantId</span></span>|<span data-ttu-id="d238d-167">Guid</span><span class="sxs-lookup"><span data-stu-id="d238d-167">Guid</span></span>|<span data-ttu-id="d238d-168">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-168">Not yet documented</span></span>|
|<span data-ttu-id="d238d-169">ProfileId</span><span class="sxs-lookup"><span data-stu-id="d238d-169">profileId</span></span>|<span data-ttu-id="d238d-170">Guid</span><span class="sxs-lookup"><span data-stu-id="d238d-170">Guid</span></span>|<span data-ttu-id="d238d-171">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-171">Not yet documented</span></span>|
|<span data-ttu-id="d238d-172">eTag</span><span class="sxs-lookup"><span data-stu-id="d238d-172">eTag</span></span>|<span data-ttu-id="d238d-173">String</span><span class="sxs-lookup"><span data-stu-id="d238d-173">String</span></span>|<span data-ttu-id="d238d-174">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-174">Not yet documented</span></span>|
|<span data-ttu-id="d238d-175">schemaVersion</span><span class="sxs-lookup"><span data-stu-id="d238d-175">schemaVersion</span></span>|[<span data-ttu-id="d238d-176">raPolicyServiceVersions</span><span class="sxs-lookup"><span data-stu-id="d238d-176">raPolicyServiceVersions</span></span>](../resources/intune-rapolicy-rapolicyserviceversions.md)|<span data-ttu-id="d238d-177">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="d238d-177">Not yet documented.</span></span> <span data-ttu-id="d238d-178">Os valores possíveis são: `initial`, `betaStart`, `experimentStart`, `mmpcStart`, `iosStart`.</span><span class="sxs-lookup"><span data-stu-id="d238d-178">Possible values are: `initial`, `betaStart`, `experimentStart`, `mmpcStart`, `iosStart`.</span></span>|
|<span data-ttu-id="d238d-179">lastModified</span><span class="sxs-lookup"><span data-stu-id="d238d-179">lastModified</span></span>|<span data-ttu-id="d238d-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d238d-180">DateTimeOffset</span></span>|<span data-ttu-id="d238d-181">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d238d-181">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d238d-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="d238d-182">Response</span></span>
<span data-ttu-id="d238d-183">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d238d-183">If successful, this method returns a `201 Created` response code and a [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d238d-184">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d238d-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="d238d-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d238d-185">Request</span></span>
<span data-ttu-id="d238d-186">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d238d-186">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/resourceAccessProfileEntities
Content-type: application/json
Content-length: 799

{
  "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
  "version": 7,
  "isDeleted": true,
  "softDeletedTime": "2016-12-31T23:59:22.6041454-08:00",
  "displayName": "Display Name value",
  "linkedProfileIds": [
    "5b59ac1a-ac1a-5b59-1aac-595b1aac595b"
  ],
  "profileTypeName": "Profile Type Name value",
  "profileBody": "Profile Body value",
  "profileBodyHash": "Profile Body Hash value",
  "platformType": 12,
  "transformedProfileBody": "Transformed Profile Body value",
  "transformedProfileBodyHash": "Transformed Profile Body Hash value",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "profileId": "6389d896-d896-6389-96d8-896396d88963",
  "eTag": "ETag value",
  "schemaVersion": "betaStart",
  "lastModified": "2017-01-01T00:03:14.6651031-08:00"
}
```

### <a name="response"></a><span data-ttu-id="d238d-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="d238d-187">Response</span></span>
<span data-ttu-id="d238d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d238d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 799

{
  "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
  "version": 7,
  "isDeleted": true,
  "softDeletedTime": "2016-12-31T23:59:22.6041454-08:00",
  "displayName": "Display Name value",
  "linkedProfileIds": [
    "5b59ac1a-ac1a-5b59-1aac-595b1aac595b"
  ],
  "profileTypeName": "Profile Type Name value",
  "profileBody": "Profile Body value",
  "profileBodyHash": "Profile Body Hash value",
  "platformType": 12,
  "transformedProfileBody": "Transformed Profile Body value",
  "transformedProfileBodyHash": "Transformed Profile Body Hash value",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "profileId": "6389d896-d896-6389-96d8-896396d88963",
  "eTag": "ETag value",
  "schemaVersion": "betaStart",
  "lastModified": "2017-01-01T00:03:14.6651031-08:00"
}
```



