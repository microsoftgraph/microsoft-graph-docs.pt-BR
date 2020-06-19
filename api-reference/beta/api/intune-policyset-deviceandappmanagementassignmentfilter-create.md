---
title: Criar deviceAndAppManagementAssignmentFilter
description: Criar um novo objeto deviceAndAppManagementAssignmentFilter.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c72cb53c03c88843a252ebb8230800d1a4c7a5e1
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791753"
---
# <a name="create-deviceandappmanagementassignmentfilter"></a><span data-ttu-id="88549-103">Criar deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="88549-103">Create deviceAndAppManagementAssignmentFilter</span></span>

<span data-ttu-id="88549-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88549-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88549-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88549-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88549-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88549-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88549-107">Criar um novo objeto [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) .</span><span class="sxs-lookup"><span data-stu-id="88549-107">Create a new [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88549-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88549-108">Prerequisites</span></span>
<span data-ttu-id="88549-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="88549-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="88549-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88549-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88549-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88549-111">Permission type</span></span>|<span data-ttu-id="88549-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88549-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88549-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88549-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88549-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88549-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88549-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88549-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88549-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88549-116">Not supported.</span></span>|
|<span data-ttu-id="88549-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88549-117">Application</span></span>|<span data-ttu-id="88549-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88549-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88549-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88549-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/assignmentFilters
```

## <a name="request-headers"></a><span data-ttu-id="88549-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88549-120">Request headers</span></span>
|<span data-ttu-id="88549-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88549-121">Header</span></span>|<span data-ttu-id="88549-122">Valor</span><span class="sxs-lookup"><span data-stu-id="88549-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88549-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="88549-123">Authorization</span></span>|<span data-ttu-id="88549-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88549-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88549-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88549-125">Accept</span></span>|<span data-ttu-id="88549-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88549-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88549-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88549-127">Request body</span></span>
<span data-ttu-id="88549-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementAssignmentFilter.</span><span class="sxs-lookup"><span data-stu-id="88549-128">In the request body, supply a JSON representation for the deviceAndAppManagementAssignmentFilter object.</span></span>

<span data-ttu-id="88549-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceAndAppManagementAssignmentFilter.</span><span class="sxs-lookup"><span data-stu-id="88549-129">The following table shows the properties that are required when you create the deviceAndAppManagementAssignmentFilter.</span></span>

|<span data-ttu-id="88549-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88549-130">Property</span></span>|<span data-ttu-id="88549-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="88549-131">Type</span></span>|<span data-ttu-id="88549-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="88549-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88549-133">id</span><span class="sxs-lookup"><span data-stu-id="88549-133">id</span></span>|<span data-ttu-id="88549-134">String</span><span class="sxs-lookup"><span data-stu-id="88549-134">String</span></span>|<span data-ttu-id="88549-135">Chave do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="88549-135">Key of the Assignment Filter.</span></span>|
|<span data-ttu-id="88549-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88549-136">createdDateTime</span></span>|<span data-ttu-id="88549-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88549-137">DateTimeOffset</span></span>|<span data-ttu-id="88549-138">Hora de criação do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="88549-138">Creation time of the Assignment Filter.</span></span>|
|<span data-ttu-id="88549-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88549-139">lastModifiedDateTime</span></span>|<span data-ttu-id="88549-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88549-140">DateTimeOffset</span></span>|<span data-ttu-id="88549-141">Hora da última modificação do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="88549-141">Last modified time of the Assignment Filter.</span></span>|
|<span data-ttu-id="88549-142">displayName</span><span class="sxs-lookup"><span data-stu-id="88549-142">displayName</span></span>|<span data-ttu-id="88549-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88549-143">String</span></span>|<span data-ttu-id="88549-144">DisplayName do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="88549-144">DisplayName of the Assignment Filter.</span></span>|
|<span data-ttu-id="88549-145">description</span><span class="sxs-lookup"><span data-stu-id="88549-145">description</span></span>|<span data-ttu-id="88549-146">String</span><span class="sxs-lookup"><span data-stu-id="88549-146">String</span></span>|<span data-ttu-id="88549-147">Descrição do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="88549-147">Description of the Assignment Filter.</span></span>|
|<span data-ttu-id="88549-148">platform</span><span class="sxs-lookup"><span data-stu-id="88549-148">platform</span></span>|[<span data-ttu-id="88549-149">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="88549-149">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="88549-150">Tipo de plataforma dos dispositivos nos quais o filtro de atribuição será aplicável.</span><span class="sxs-lookup"><span data-stu-id="88549-150">Platform type of the devices on which the Assignment Filter will be applicable.</span></span> <span data-ttu-id="88549-151">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="88549-151">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="88549-152">norma</span><span class="sxs-lookup"><span data-stu-id="88549-152">rule</span></span>|<span data-ttu-id="88549-153">String</span><span class="sxs-lookup"><span data-stu-id="88549-153">String</span></span>|<span data-ttu-id="88549-154">Definição de regra do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="88549-154">Rule definition of the Assignment Filter.</span></span>|
|<span data-ttu-id="88549-155">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="88549-155">roleScopeTags</span></span>|<span data-ttu-id="88549-156">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="88549-156">String collection</span></span>|<span data-ttu-id="88549-157">RoleScopeTags do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="88549-157">RoleScopeTags of the Assignment Filter.</span></span>|



## <a name="response"></a><span data-ttu-id="88549-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="88549-158">Response</span></span>
<span data-ttu-id="88549-159">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88549-159">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88549-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88549-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="88549-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88549-161">Request</span></span>
<span data-ttu-id="88549-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88549-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/assignmentFilters
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

### <a name="response"></a><span data-ttu-id="88549-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="88549-163">Response</span></span>
<span data-ttu-id="88549-164">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="88549-164">Here is an example of the response.</span></span> <span data-ttu-id="88549-165">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="88549-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="88549-166">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="88549-166">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



