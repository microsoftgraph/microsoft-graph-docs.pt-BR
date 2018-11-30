---
title: Criar managedAppOperation
description: Criar um novo objeto managedAppOperation.
ms.openlocfilehash: ac6a6933a7cceac298e2cbd1c59d3cb1ec4aaade
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036708"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="4e248-103">Criar managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="4e248-103">Create managedAppOperation</span></span>

> <span data-ttu-id="4e248-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4e248-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e248-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4e248-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e248-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4e248-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e248-107">Criar um novo objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="4e248-107">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e248-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4e248-108">Prerequisites</span></span>
<span data-ttu-id="4e248-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e248-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e248-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e248-111">Permission type</span></span>|<span data-ttu-id="4e248-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e248-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e248-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e248-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e248-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e248-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e248-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e248-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e248-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e248-116">Not supported.</span></span>|
|<span data-ttu-id="4e248-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e248-117">Application</span></span>|<span data-ttu-id="4e248-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e248-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e248-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e248-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="4e248-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e248-120">Request headers</span></span>
|<span data-ttu-id="4e248-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e248-121">Header</span></span>|<span data-ttu-id="4e248-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4e248-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e248-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e248-123">Authorization</span></span>|<span data-ttu-id="4e248-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e248-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e248-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e248-125">Accept</span></span>|<span data-ttu-id="4e248-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e248-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e248-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e248-127">Request body</span></span>
<span data-ttu-id="4e248-128">No corpo da solicitação, forneça uma representação JSON do objeto managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="4e248-128">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="4e248-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="4e248-129">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="4e248-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e248-130">Property</span></span>|<span data-ttu-id="4e248-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e248-131">Type</span></span>|<span data-ttu-id="4e248-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e248-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e248-133">displayName</span><span class="sxs-lookup"><span data-stu-id="4e248-133">displayName</span></span>|<span data-ttu-id="4e248-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e248-134">String</span></span>|<span data-ttu-id="4e248-135">O nome da operação.</span><span class="sxs-lookup"><span data-stu-id="4e248-135">The operation name.</span></span>|
|<span data-ttu-id="4e248-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e248-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4e248-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e248-137">DateTimeOffset</span></span>|<span data-ttu-id="4e248-138">Última vez em que a operação de aplicativo foi modificada.</span><span class="sxs-lookup"><span data-stu-id="4e248-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="4e248-139">state</span><span class="sxs-lookup"><span data-stu-id="4e248-139">state</span></span>|<span data-ttu-id="4e248-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e248-140">String</span></span>|<span data-ttu-id="4e248-141">O estado atual da operação</span><span class="sxs-lookup"><span data-stu-id="4e248-141">The current state of the operation</span></span>|
|<span data-ttu-id="4e248-142">id</span><span class="sxs-lookup"><span data-stu-id="4e248-142">id</span></span>|<span data-ttu-id="4e248-143">String</span><span class="sxs-lookup"><span data-stu-id="4e248-143">String</span></span>|<span data-ttu-id="4e248-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4e248-144">Key of the entity.</span></span>|
|<span data-ttu-id="4e248-145">version</span><span class="sxs-lookup"><span data-stu-id="4e248-145">version</span></span>|<span data-ttu-id="4e248-146">String</span><span class="sxs-lookup"><span data-stu-id="4e248-146">String</span></span>|<span data-ttu-id="4e248-147">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="4e248-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="4e248-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e248-148">Response</span></span>
<span data-ttu-id="4e248-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedAppOperation](../resources/intune-mam-managedappoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e248-149">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e248-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e248-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e248-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e248-151">Request</span></span>
<span data-ttu-id="4e248-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e248-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 223

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="4e248-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e248-153">Response</span></span>
<span data-ttu-id="4e248-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e248-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





