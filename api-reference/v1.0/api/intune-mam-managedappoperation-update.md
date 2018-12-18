---
title: Atualizar managedAppOperation
description: Atualizar as propriedades de um objeto managedAppOperation.
author: tfitzmac
ms.openlocfilehash: 2bd0d326a4300bdae29484b547bbd5aa429728ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311974"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="b215a-103">Atualizar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b215a-103">Update managedAppOperation</span></span>

> <span data-ttu-id="b215a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b215a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b215a-105">Atualizar as propriedades de um objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b215a-105">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b215a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b215a-106">Prerequisites</span></span>
<span data-ttu-id="b215a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b215a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b215a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b215a-109">Permission type</span></span>|<span data-ttu-id="b215a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b215a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b215a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b215a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b215a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b215a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b215a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b215a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b215a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b215a-114">Not supported.</span></span>|
|<span data-ttu-id="b215a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b215a-115">Application</span></span>|<span data-ttu-id="b215a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b215a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b215a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b215a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="b215a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b215a-118">Request headers</span></span>
|<span data-ttu-id="b215a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b215a-119">Header</span></span>|<span data-ttu-id="b215a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b215a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b215a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b215a-121">Authorization</span></span>|<span data-ttu-id="b215a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b215a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b215a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b215a-123">Accept</span></span>|<span data-ttu-id="b215a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b215a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b215a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b215a-125">Request body</span></span>
<span data-ttu-id="b215a-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b215a-126">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="b215a-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b215a-127">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="b215a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b215a-128">Property</span></span>|<span data-ttu-id="b215a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b215a-129">Type</span></span>|<span data-ttu-id="b215a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b215a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b215a-131">displayName</span><span class="sxs-lookup"><span data-stu-id="b215a-131">displayName</span></span>|<span data-ttu-id="b215a-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b215a-132">String</span></span>|<span data-ttu-id="b215a-133">O nome da operação.</span><span class="sxs-lookup"><span data-stu-id="b215a-133">The operation name.</span></span>|
|<span data-ttu-id="b215a-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b215a-134">lastModifiedDateTime</span></span>|<span data-ttu-id="b215a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b215a-135">DateTimeOffset</span></span>|<span data-ttu-id="b215a-136">Última vez em que a operação de aplicativo foi modificada.</span><span class="sxs-lookup"><span data-stu-id="b215a-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="b215a-137">estado</span><span class="sxs-lookup"><span data-stu-id="b215a-137">state</span></span>|<span data-ttu-id="b215a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b215a-138">String</span></span>|<span data-ttu-id="b215a-139">O estado atual da operação</span><span class="sxs-lookup"><span data-stu-id="b215a-139">The current state of the operation</span></span>|
|<span data-ttu-id="b215a-140">id</span><span class="sxs-lookup"><span data-stu-id="b215a-140">id</span></span>|<span data-ttu-id="b215a-141">String</span><span class="sxs-lookup"><span data-stu-id="b215a-141">String</span></span>|<span data-ttu-id="b215a-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b215a-142">Key of the entity.</span></span>|
|<span data-ttu-id="b215a-143">version</span><span class="sxs-lookup"><span data-stu-id="b215a-143">version</span></span>|<span data-ttu-id="b215a-144">String</span><span class="sxs-lookup"><span data-stu-id="b215a-144">String</span></span>|<span data-ttu-id="b215a-145">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="b215a-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b215a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b215a-146">Response</span></span>
<span data-ttu-id="b215a-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b215a-147">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b215a-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b215a-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="b215a-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b215a-149">Request</span></span>
<span data-ttu-id="b215a-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b215a-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b215a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b215a-151">Response</span></span>
<span data-ttu-id="b215a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b215a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



