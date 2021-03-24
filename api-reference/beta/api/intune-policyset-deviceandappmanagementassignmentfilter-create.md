---
title: Criar deviceAndAppManagementAssignmentFilter
description: Crie um novo objeto deviceAndAppManagementAssignmentFilter.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3245d4a22a84ab0dea72146f7724cfdd83a88c9b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125279"
---
# <a name="create-deviceandappmanagementassignmentfilter"></a><span data-ttu-id="c802e-103">Criar deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="c802e-103">Create deviceAndAppManagementAssignmentFilter</span></span>

<span data-ttu-id="c802e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c802e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c802e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c802e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c802e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c802e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c802e-107">Crie um novo [objeto deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)</span><span class="sxs-lookup"><span data-stu-id="c802e-107">Create a new [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c802e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c802e-108">Prerequisites</span></span>
<span data-ttu-id="c802e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c802e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c802e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c802e-111">Permission type</span></span>|<span data-ttu-id="c802e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c802e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c802e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c802e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c802e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c802e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c802e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c802e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c802e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c802e-116">Not supported.</span></span>|
|<span data-ttu-id="c802e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c802e-117">Application</span></span>|<span data-ttu-id="c802e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c802e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c802e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c802e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/assignmentFilters
```

## <a name="request-headers"></a><span data-ttu-id="c802e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c802e-120">Request headers</span></span>
|<span data-ttu-id="c802e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c802e-121">Header</span></span>|<span data-ttu-id="c802e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c802e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c802e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c802e-123">Authorization</span></span>|<span data-ttu-id="c802e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c802e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c802e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c802e-125">Accept</span></span>|<span data-ttu-id="c802e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c802e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c802e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c802e-127">Request body</span></span>
<span data-ttu-id="c802e-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceAndAppManagementAssignmentFilter.</span><span class="sxs-lookup"><span data-stu-id="c802e-128">In the request body, supply a JSON representation for the deviceAndAppManagementAssignmentFilter object.</span></span>

<span data-ttu-id="c802e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceAndAppManagementAssignmentFilter.</span><span class="sxs-lookup"><span data-stu-id="c802e-129">The following table shows the properties that are required when you create the deviceAndAppManagementAssignmentFilter.</span></span>

|<span data-ttu-id="c802e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c802e-130">Property</span></span>|<span data-ttu-id="c802e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c802e-131">Type</span></span>|<span data-ttu-id="c802e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c802e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c802e-133">id</span><span class="sxs-lookup"><span data-stu-id="c802e-133">id</span></span>|<span data-ttu-id="c802e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c802e-134">String</span></span>|<span data-ttu-id="c802e-135">Chave do Filtro de Atribuição.</span><span class="sxs-lookup"><span data-stu-id="c802e-135">Key of the Assignment Filter.</span></span>|
|<span data-ttu-id="c802e-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c802e-136">createdDateTime</span></span>|<span data-ttu-id="c802e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c802e-137">DateTimeOffset</span></span>|<span data-ttu-id="c802e-138">Hora de criação do Filtro de Atribuição.</span><span class="sxs-lookup"><span data-stu-id="c802e-138">Creation time of the Assignment Filter.</span></span>|
|<span data-ttu-id="c802e-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c802e-139">lastModifiedDateTime</span></span>|<span data-ttu-id="c802e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c802e-140">DateTimeOffset</span></span>|<span data-ttu-id="c802e-141">Última hora modificada do Filtro de Atribuição.</span><span class="sxs-lookup"><span data-stu-id="c802e-141">Last modified time of the Assignment Filter.</span></span>|
|<span data-ttu-id="c802e-142">displayName</span><span class="sxs-lookup"><span data-stu-id="c802e-142">displayName</span></span>|<span data-ttu-id="c802e-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c802e-143">String</span></span>|<span data-ttu-id="c802e-144">DisplayName do Filtro de Atribuição.</span><span class="sxs-lookup"><span data-stu-id="c802e-144">DisplayName of the Assignment Filter.</span></span>|
|<span data-ttu-id="c802e-145">descrição</span><span class="sxs-lookup"><span data-stu-id="c802e-145">description</span></span>|<span data-ttu-id="c802e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c802e-146">String</span></span>|<span data-ttu-id="c802e-147">Descrição do Filtro de Atribuição.</span><span class="sxs-lookup"><span data-stu-id="c802e-147">Description of the Assignment Filter.</span></span>|
|<span data-ttu-id="c802e-148">plataforma</span><span class="sxs-lookup"><span data-stu-id="c802e-148">platform</span></span>|[<span data-ttu-id="c802e-149">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="c802e-149">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="c802e-150">Tipo de plataforma dos dispositivos nos quais o Filtro de Atribuição será aplicável.</span><span class="sxs-lookup"><span data-stu-id="c802e-150">Platform type of the devices on which the Assignment Filter will be applicable.</span></span> <span data-ttu-id="c802e-151">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c802e-151">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="c802e-152">rule</span><span class="sxs-lookup"><span data-stu-id="c802e-152">rule</span></span>|<span data-ttu-id="c802e-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c802e-153">String</span></span>|<span data-ttu-id="c802e-154">Definição de regra do Filtro de Atribuição.</span><span class="sxs-lookup"><span data-stu-id="c802e-154">Rule definition of the Assignment Filter.</span></span>|
|<span data-ttu-id="c802e-155">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="c802e-155">roleScopeTags</span></span>|<span data-ttu-id="c802e-156">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c802e-156">String collection</span></span>|<span data-ttu-id="c802e-157">RoleScopeTags do Filtro de Atribuição.</span><span class="sxs-lookup"><span data-stu-id="c802e-157">RoleScopeTags of the Assignment Filter.</span></span>|



## <a name="response"></a><span data-ttu-id="c802e-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="c802e-158">Response</span></span>
<span data-ttu-id="c802e-159">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c802e-159">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c802e-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c802e-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="c802e-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c802e-161">Request</span></span>
<span data-ttu-id="c802e-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c802e-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c802e-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="c802e-163">Response</span></span>
<span data-ttu-id="c802e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c802e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




