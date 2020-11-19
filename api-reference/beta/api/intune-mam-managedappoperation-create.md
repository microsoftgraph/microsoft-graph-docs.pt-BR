---
title: Criar managedAppOperation
description: Criar um novo objeto managedAppOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5238b4e5e1c796893e930929b2edc788ad7a134a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49277719"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="6b550-103">Criar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="6b550-103">Create managedAppOperation</span></span>

<span data-ttu-id="6b550-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b550-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b550-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b550-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b550-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b550-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b550-107">Criar um novo objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="6b550-107">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b550-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b550-108">Prerequisites</span></span>
<span data-ttu-id="6b550-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b550-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b550-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b550-111">Permission type</span></span>|<span data-ttu-id="6b550-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6b550-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b550-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b550-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b550-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b550-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6b550-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b550-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b550-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b550-116">Not supported.</span></span>|
|<span data-ttu-id="6b550-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b550-117">Application</span></span>|<span data-ttu-id="6b550-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b550-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b550-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b550-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="6b550-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b550-120">Request headers</span></span>
|<span data-ttu-id="6b550-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b550-121">Header</span></span>|<span data-ttu-id="6b550-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6b550-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b550-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b550-123">Authorization</span></span>|<span data-ttu-id="6b550-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b550-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b550-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b550-125">Accept</span></span>|<span data-ttu-id="6b550-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b550-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b550-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b550-127">Request body</span></span>
<span data-ttu-id="6b550-128">No corpo da solicitação, forneça uma representação JSON do objeto managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="6b550-128">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="6b550-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="6b550-129">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="6b550-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b550-130">Property</span></span>|<span data-ttu-id="6b550-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b550-131">Type</span></span>|<span data-ttu-id="6b550-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b550-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b550-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6b550-133">displayName</span></span>|<span data-ttu-id="6b550-134">String</span><span class="sxs-lookup"><span data-stu-id="6b550-134">String</span></span>|<span data-ttu-id="6b550-135">O nome da operação.</span><span class="sxs-lookup"><span data-stu-id="6b550-135">The operation name.</span></span>|
|<span data-ttu-id="6b550-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b550-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6b550-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b550-137">DateTimeOffset</span></span>|<span data-ttu-id="6b550-138">Última vez em que a operação de aplicativo foi modificada.</span><span class="sxs-lookup"><span data-stu-id="6b550-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="6b550-139">state</span><span class="sxs-lookup"><span data-stu-id="6b550-139">state</span></span>|<span data-ttu-id="6b550-140">String</span><span class="sxs-lookup"><span data-stu-id="6b550-140">String</span></span>|<span data-ttu-id="6b550-141">O estado atual da operação</span><span class="sxs-lookup"><span data-stu-id="6b550-141">The current state of the operation</span></span>|
|<span data-ttu-id="6b550-142">id</span><span class="sxs-lookup"><span data-stu-id="6b550-142">id</span></span>|<span data-ttu-id="6b550-143">String</span><span class="sxs-lookup"><span data-stu-id="6b550-143">String</span></span>|<span data-ttu-id="6b550-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6b550-144">Key of the entity.</span></span>|
|<span data-ttu-id="6b550-145">versão</span><span class="sxs-lookup"><span data-stu-id="6b550-145">version</span></span>|<span data-ttu-id="6b550-146">String</span><span class="sxs-lookup"><span data-stu-id="6b550-146">String</span></span>|<span data-ttu-id="6b550-147">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="6b550-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="6b550-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b550-148">Response</span></span>
<span data-ttu-id="6b550-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b550-149">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b550-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b550-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b550-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b550-151">Request</span></span>
<span data-ttu-id="6b550-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b550-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="6b550-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b550-153">Response</span></span>
<span data-ttu-id="6b550-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b550-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
  "version": "Version value"
}
```




