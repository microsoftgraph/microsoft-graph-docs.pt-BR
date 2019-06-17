---
title: Criar managedAppOperation
description: Criar um novo objeto managedAppOperation.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b79845a9210fd34bb585196fd37fcd189d34f19a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985903"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="0ee37-103">Criar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="0ee37-103">Create managedAppOperation</span></span>

> <span data-ttu-id="0ee37-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ee37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ee37-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ee37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee37-106">Criar um novo objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0ee37-106">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ee37-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ee37-107">Prerequisites</span></span>
<span data-ttu-id="0ee37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ee37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ee37-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ee37-110">Permission type</span></span>|<span data-ttu-id="0ee37-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0ee37-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ee37-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ee37-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ee37-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ee37-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0ee37-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ee37-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ee37-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ee37-115">Not supported.</span></span>|
|<span data-ttu-id="0ee37-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ee37-116">Application</span></span>|<span data-ttu-id="0ee37-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ee37-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ee37-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ee37-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="0ee37-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee37-119">Request headers</span></span>
|<span data-ttu-id="0ee37-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ee37-120">Header</span></span>|<span data-ttu-id="0ee37-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0ee37-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ee37-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ee37-122">Authorization</span></span>|<span data-ttu-id="0ee37-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ee37-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ee37-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0ee37-124">Accept</span></span>|<span data-ttu-id="0ee37-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ee37-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ee37-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee37-126">Request body</span></span>
<span data-ttu-id="0ee37-127">No corpo da solicitação, forneça uma representação JSON do objeto managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="0ee37-127">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="0ee37-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="0ee37-128">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="0ee37-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ee37-129">Property</span></span>|<span data-ttu-id="0ee37-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ee37-130">Type</span></span>|<span data-ttu-id="0ee37-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ee37-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ee37-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0ee37-132">displayName</span></span>|<span data-ttu-id="0ee37-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ee37-133">String</span></span>|<span data-ttu-id="0ee37-134">O nome da operação.</span><span class="sxs-lookup"><span data-stu-id="0ee37-134">The operation name.</span></span>|
|<span data-ttu-id="0ee37-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ee37-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0ee37-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ee37-136">DateTimeOffset</span></span>|<span data-ttu-id="0ee37-137">Última vez em que a operação de aplicativo foi modificada.</span><span class="sxs-lookup"><span data-stu-id="0ee37-137">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="0ee37-138">state</span><span class="sxs-lookup"><span data-stu-id="0ee37-138">state</span></span>|<span data-ttu-id="0ee37-139">String</span><span class="sxs-lookup"><span data-stu-id="0ee37-139">String</span></span>|<span data-ttu-id="0ee37-140">O estado atual da operação</span><span class="sxs-lookup"><span data-stu-id="0ee37-140">The current state of the operation</span></span>|
|<span data-ttu-id="0ee37-141">id</span><span class="sxs-lookup"><span data-stu-id="0ee37-141">id</span></span>|<span data-ttu-id="0ee37-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ee37-142">String</span></span>|<span data-ttu-id="0ee37-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0ee37-143">Key of the entity.</span></span>|
|<span data-ttu-id="0ee37-144">versão</span><span class="sxs-lookup"><span data-stu-id="0ee37-144">version</span></span>|<span data-ttu-id="0ee37-145">String</span><span class="sxs-lookup"><span data-stu-id="0ee37-145">String</span></span>|<span data-ttu-id="0ee37-146">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="0ee37-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="0ee37-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ee37-147">Response</span></span>
<span data-ttu-id="0ee37-148">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ee37-148">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ee37-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ee37-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ee37-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee37-150">Request</span></span>
<span data-ttu-id="0ee37-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ee37-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ee37-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ee37-152">Response</span></span>
<span data-ttu-id="0ee37-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ee37-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





