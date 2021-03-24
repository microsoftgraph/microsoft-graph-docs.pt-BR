---
title: Criar managedAppOperation
description: Criar um novo objeto managedAppOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9cdef2642ee2a3158723cf286708dc21ad3d14e3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149300"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="009c2-103">Criar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="009c2-103">Create managedAppOperation</span></span>

<span data-ttu-id="009c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="009c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="009c2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="009c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="009c2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="009c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="009c2-107">Criar um novo objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="009c2-107">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="009c2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="009c2-108">Prerequisites</span></span>
<span data-ttu-id="009c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="009c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="009c2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="009c2-111">Permission type</span></span>|<span data-ttu-id="009c2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="009c2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="009c2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="009c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="009c2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="009c2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="009c2-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="009c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="009c2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="009c2-116">Not supported.</span></span>|
|<span data-ttu-id="009c2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="009c2-117">Application</span></span>|<span data-ttu-id="009c2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="009c2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="009c2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="009c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="009c2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="009c2-120">Request headers</span></span>
|<span data-ttu-id="009c2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="009c2-121">Header</span></span>|<span data-ttu-id="009c2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="009c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="009c2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="009c2-123">Authorization</span></span>|<span data-ttu-id="009c2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="009c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="009c2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="009c2-125">Accept</span></span>|<span data-ttu-id="009c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="009c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="009c2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="009c2-127">Request body</span></span>
<span data-ttu-id="009c2-128">No corpo da solicitação, forneça uma representação JSON do objeto managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="009c2-128">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="009c2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="009c2-129">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="009c2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="009c2-130">Property</span></span>|<span data-ttu-id="009c2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="009c2-131">Type</span></span>|<span data-ttu-id="009c2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="009c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="009c2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="009c2-133">displayName</span></span>|<span data-ttu-id="009c2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="009c2-134">String</span></span>|<span data-ttu-id="009c2-135">O nome da operação.</span><span class="sxs-lookup"><span data-stu-id="009c2-135">The operation name.</span></span>|
|<span data-ttu-id="009c2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="009c2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="009c2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="009c2-137">DateTimeOffset</span></span>|<span data-ttu-id="009c2-138">Última vez em que a operação de aplicativo foi modificada.</span><span class="sxs-lookup"><span data-stu-id="009c2-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="009c2-139">state</span><span class="sxs-lookup"><span data-stu-id="009c2-139">state</span></span>|<span data-ttu-id="009c2-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="009c2-140">String</span></span>|<span data-ttu-id="009c2-141">O estado atual da operação</span><span class="sxs-lookup"><span data-stu-id="009c2-141">The current state of the operation</span></span>|
|<span data-ttu-id="009c2-142">id</span><span class="sxs-lookup"><span data-stu-id="009c2-142">id</span></span>|<span data-ttu-id="009c2-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="009c2-143">String</span></span>|<span data-ttu-id="009c2-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="009c2-144">Key of the entity.</span></span>|
|<span data-ttu-id="009c2-145">versão</span><span class="sxs-lookup"><span data-stu-id="009c2-145">version</span></span>|<span data-ttu-id="009c2-146">String</span><span class="sxs-lookup"><span data-stu-id="009c2-146">String</span></span>|<span data-ttu-id="009c2-147">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="009c2-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="009c2-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="009c2-148">Response</span></span>
<span data-ttu-id="009c2-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="009c2-149">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="009c2-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="009c2-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="009c2-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="009c2-151">Request</span></span>
<span data-ttu-id="009c2-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="009c2-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="009c2-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="009c2-153">Response</span></span>
<span data-ttu-id="009c2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="009c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




