---
title: Atualizar managedAppOperation
description: Atualizar as propriedades de um objeto managedAppOperation.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4b91f2d0c40c0dede51bd936fce42fd59b72b2fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513165"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="0cf41-103">Atualizar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="0cf41-103">Update managedAppOperation</span></span>

<span data-ttu-id="0cf41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cf41-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cf41-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0cf41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cf41-106">Atualizar as propriedades de um objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0cf41-106">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cf41-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0cf41-107">Prerequisites</span></span>
<span data-ttu-id="0cf41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cf41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cf41-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cf41-110">Permission type</span></span>|<span data-ttu-id="0cf41-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0cf41-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cf41-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cf41-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0cf41-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cf41-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0cf41-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cf41-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cf41-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cf41-115">Not supported.</span></span>|
|<span data-ttu-id="0cf41-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cf41-116">Application</span></span>|<span data-ttu-id="0cf41-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cf41-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cf41-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cf41-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="0cf41-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cf41-119">Request headers</span></span>
|<span data-ttu-id="0cf41-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0cf41-120">Header</span></span>|<span data-ttu-id="0cf41-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0cf41-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cf41-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cf41-122">Authorization</span></span>|<span data-ttu-id="0cf41-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cf41-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cf41-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0cf41-124">Accept</span></span>|<span data-ttu-id="0cf41-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0cf41-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cf41-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cf41-126">Request body</span></span>
<span data-ttu-id="0cf41-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0cf41-127">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="0cf41-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0cf41-128">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="0cf41-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cf41-129">Property</span></span>|<span data-ttu-id="0cf41-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cf41-130">Type</span></span>|<span data-ttu-id="0cf41-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cf41-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cf41-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0cf41-132">displayName</span></span>|<span data-ttu-id="0cf41-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cf41-133">String</span></span>|<span data-ttu-id="0cf41-134">O nome da operação.</span><span class="sxs-lookup"><span data-stu-id="0cf41-134">The operation name.</span></span>|
|<span data-ttu-id="0cf41-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0cf41-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0cf41-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cf41-136">DateTimeOffset</span></span>|<span data-ttu-id="0cf41-137">Última vez em que a operação de aplicativo foi modificada.</span><span class="sxs-lookup"><span data-stu-id="0cf41-137">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="0cf41-138">state</span><span class="sxs-lookup"><span data-stu-id="0cf41-138">state</span></span>|<span data-ttu-id="0cf41-139">String</span><span class="sxs-lookup"><span data-stu-id="0cf41-139">String</span></span>|<span data-ttu-id="0cf41-140">O estado atual da operação</span><span class="sxs-lookup"><span data-stu-id="0cf41-140">The current state of the operation</span></span>|
|<span data-ttu-id="0cf41-141">id</span><span class="sxs-lookup"><span data-stu-id="0cf41-141">id</span></span>|<span data-ttu-id="0cf41-142">String</span><span class="sxs-lookup"><span data-stu-id="0cf41-142">String</span></span>|<span data-ttu-id="0cf41-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0cf41-143">Key of the entity.</span></span>|
|<span data-ttu-id="0cf41-144">versão</span><span class="sxs-lookup"><span data-stu-id="0cf41-144">version</span></span>|<span data-ttu-id="0cf41-145">String</span><span class="sxs-lookup"><span data-stu-id="0cf41-145">String</span></span>|<span data-ttu-id="0cf41-146">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="0cf41-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="0cf41-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cf41-147">Response</span></span>
<span data-ttu-id="0cf41-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cf41-148">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cf41-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cf41-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cf41-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cf41-150">Request</span></span>
<span data-ttu-id="0cf41-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cf41-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0cf41-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cf41-152">Response</span></span>
<span data-ttu-id="0cf41-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0cf41-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




