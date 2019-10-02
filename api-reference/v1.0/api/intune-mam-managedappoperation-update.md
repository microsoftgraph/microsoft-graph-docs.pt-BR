---
title: Atualizar managedAppOperation
description: Atualizar as propriedades de um objeto managedAppOperation.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8be5619d16474fc8f606c41172bd107a1aa0c56a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363651"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="b0dc7-103">Atualizar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b0dc7-103">Update managedAppOperation</span></span>

> <span data-ttu-id="b0dc7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0dc7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0dc7-105">Atualizar as propriedades de um objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b0dc7-105">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0dc7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0dc7-106">Prerequisites</span></span>
<span data-ttu-id="b0dc7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0dc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0dc7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0dc7-109">Permission type</span></span>|<span data-ttu-id="b0dc7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0dc7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0dc7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0dc7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b0dc7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0dc7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b0dc7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0dc7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0dc7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0dc7-114">Not supported.</span></span>|
|<span data-ttu-id="b0dc7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0dc7-115">Application</span></span>|<span data-ttu-id="b0dc7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0dc7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0dc7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0dc7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="b0dc7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0dc7-118">Request headers</span></span>
|<span data-ttu-id="b0dc7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0dc7-119">Header</span></span>|<span data-ttu-id="b0dc7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b0dc7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0dc7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0dc7-121">Authorization</span></span>|<span data-ttu-id="b0dc7-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0dc7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0dc7-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b0dc7-123">Accept</span></span>|<span data-ttu-id="b0dc7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b0dc7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0dc7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0dc7-125">Request body</span></span>
<span data-ttu-id="b0dc7-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b0dc7-126">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="b0dc7-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b0dc7-127">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="b0dc7-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0dc7-128">Property</span></span>|<span data-ttu-id="b0dc7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0dc7-129">Type</span></span>|<span data-ttu-id="b0dc7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0dc7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0dc7-131">displayName</span><span class="sxs-lookup"><span data-stu-id="b0dc7-131">displayName</span></span>|<span data-ttu-id="b0dc7-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0dc7-132">String</span></span>|<span data-ttu-id="b0dc7-133">O nome da operação.</span><span class="sxs-lookup"><span data-stu-id="b0dc7-133">The operation name.</span></span>|
|<span data-ttu-id="b0dc7-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0dc7-134">lastModifiedDateTime</span></span>|<span data-ttu-id="b0dc7-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0dc7-135">DateTimeOffset</span></span>|<span data-ttu-id="b0dc7-136">Última vez em que a operação de aplicativo foi modificada.</span><span class="sxs-lookup"><span data-stu-id="b0dc7-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="b0dc7-137">state</span><span class="sxs-lookup"><span data-stu-id="b0dc7-137">state</span></span>|<span data-ttu-id="b0dc7-138">String</span><span class="sxs-lookup"><span data-stu-id="b0dc7-138">String</span></span>|<span data-ttu-id="b0dc7-139">O estado atual da operação</span><span class="sxs-lookup"><span data-stu-id="b0dc7-139">The current state of the operation</span></span>|
|<span data-ttu-id="b0dc7-140">id</span><span class="sxs-lookup"><span data-stu-id="b0dc7-140">id</span></span>|<span data-ttu-id="b0dc7-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0dc7-141">String</span></span>|<span data-ttu-id="b0dc7-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b0dc7-142">Key of the entity.</span></span>|
|<span data-ttu-id="b0dc7-143">versão</span><span class="sxs-lookup"><span data-stu-id="b0dc7-143">version</span></span>|<span data-ttu-id="b0dc7-144">String</span><span class="sxs-lookup"><span data-stu-id="b0dc7-144">String</span></span>|<span data-ttu-id="b0dc7-145">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="b0dc7-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b0dc7-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0dc7-146">Response</span></span>
<span data-ttu-id="b0dc7-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0dc7-147">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0dc7-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0dc7-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0dc7-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0dc7-149">Request</span></span>
<span data-ttu-id="b0dc7-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0dc7-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="b0dc7-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0dc7-151">Response</span></span>
<span data-ttu-id="b0dc7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0dc7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




