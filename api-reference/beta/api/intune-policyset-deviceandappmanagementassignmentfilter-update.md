---
title: Atualizar deviceAndAppManagementAssignmentFilter
description: Atualiza as propriedades de um objeto deviceAndAppManagementAssignmentFilter.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5fd7242879c9a086b08895637ad811b5fd48160
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791725"
---
# <a name="update-deviceandappmanagementassignmentfilter"></a><span data-ttu-id="3041d-103">Atualizar deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="3041d-103">Update deviceAndAppManagementAssignmentFilter</span></span>

<span data-ttu-id="3041d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3041d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3041d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3041d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3041d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3041d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3041d-107">Atualiza as propriedades de um objeto [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) .</span><span class="sxs-lookup"><span data-stu-id="3041d-107">Update the properties of a [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3041d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3041d-108">Prerequisites</span></span>
<span data-ttu-id="3041d-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3041d-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3041d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3041d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3041d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3041d-111">Permission type</span></span>|<span data-ttu-id="3041d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3041d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3041d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3041d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3041d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3041d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3041d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3041d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3041d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3041d-116">Not supported.</span></span>|
|<span data-ttu-id="3041d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3041d-117">Application</span></span>|<span data-ttu-id="3041d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3041d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3041d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3041d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
```

## <a name="request-headers"></a><span data-ttu-id="3041d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3041d-120">Request headers</span></span>
|<span data-ttu-id="3041d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3041d-121">Header</span></span>|<span data-ttu-id="3041d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3041d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3041d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3041d-123">Authorization</span></span>|<span data-ttu-id="3041d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3041d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3041d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3041d-125">Accept</span></span>|<span data-ttu-id="3041d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3041d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3041d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3041d-127">Request body</span></span>
<span data-ttu-id="3041d-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) .</span><span class="sxs-lookup"><span data-stu-id="3041d-128">In the request body, supply a JSON representation for the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

<span data-ttu-id="3041d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span><span class="sxs-lookup"><span data-stu-id="3041d-129">The following table shows the properties that are required when you create the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span></span>

|<span data-ttu-id="3041d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3041d-130">Property</span></span>|<span data-ttu-id="3041d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3041d-131">Type</span></span>|<span data-ttu-id="3041d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3041d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3041d-133">id</span><span class="sxs-lookup"><span data-stu-id="3041d-133">id</span></span>|<span data-ttu-id="3041d-134">String</span><span class="sxs-lookup"><span data-stu-id="3041d-134">String</span></span>|<span data-ttu-id="3041d-135">Chave do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="3041d-135">Key of the Assignment Filter.</span></span>|
|<span data-ttu-id="3041d-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3041d-136">createdDateTime</span></span>|<span data-ttu-id="3041d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3041d-137">DateTimeOffset</span></span>|<span data-ttu-id="3041d-138">Hora de criação do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="3041d-138">Creation time of the Assignment Filter.</span></span>|
|<span data-ttu-id="3041d-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3041d-139">lastModifiedDateTime</span></span>|<span data-ttu-id="3041d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3041d-140">DateTimeOffset</span></span>|<span data-ttu-id="3041d-141">Hora da última modificação do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="3041d-141">Last modified time of the Assignment Filter.</span></span>|
|<span data-ttu-id="3041d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="3041d-142">displayName</span></span>|<span data-ttu-id="3041d-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3041d-143">String</span></span>|<span data-ttu-id="3041d-144">DisplayName do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="3041d-144">DisplayName of the Assignment Filter.</span></span>|
|<span data-ttu-id="3041d-145">description</span><span class="sxs-lookup"><span data-stu-id="3041d-145">description</span></span>|<span data-ttu-id="3041d-146">String</span><span class="sxs-lookup"><span data-stu-id="3041d-146">String</span></span>|<span data-ttu-id="3041d-147">Descrição do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="3041d-147">Description of the Assignment Filter.</span></span>|
|<span data-ttu-id="3041d-148">platform</span><span class="sxs-lookup"><span data-stu-id="3041d-148">platform</span></span>|[<span data-ttu-id="3041d-149">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="3041d-149">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="3041d-150">Tipo de plataforma dos dispositivos nos quais o filtro de atribuição será aplicável.</span><span class="sxs-lookup"><span data-stu-id="3041d-150">Platform type of the devices on which the Assignment Filter will be applicable.</span></span> <span data-ttu-id="3041d-151">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3041d-151">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="3041d-152">norma</span><span class="sxs-lookup"><span data-stu-id="3041d-152">rule</span></span>|<span data-ttu-id="3041d-153">String</span><span class="sxs-lookup"><span data-stu-id="3041d-153">String</span></span>|<span data-ttu-id="3041d-154">Definição de regra do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="3041d-154">Rule definition of the Assignment Filter.</span></span>|
|<span data-ttu-id="3041d-155">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="3041d-155">roleScopeTags</span></span>|<span data-ttu-id="3041d-156">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3041d-156">String collection</span></span>|<span data-ttu-id="3041d-157">RoleScopeTags do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="3041d-157">RoleScopeTags of the Assignment Filter.</span></span>|



## <a name="response"></a><span data-ttu-id="3041d-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="3041d-158">Response</span></span>
<span data-ttu-id="3041d-159">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3041d-159">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3041d-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3041d-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="3041d-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3041d-161">Request</span></span>
<span data-ttu-id="3041d-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3041d-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
Content-type: application/json
Content-length: 274

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
  "displayName": "Display Name value",
  "description": "Description value",
  "platform": "androidForWork",
  "rule": "Rule value",
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="3041d-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="3041d-163">Response</span></span>
<span data-ttu-id="3041d-164">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="3041d-164">Here is an example of the response.</span></span> <span data-ttu-id="3041d-165">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="3041d-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3041d-166">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3041d-166">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 446

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
  "id": "819818db-18db-8198-db18-9881db189881",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "platform": "androidForWork",
  "rule": "Rule value",
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```



