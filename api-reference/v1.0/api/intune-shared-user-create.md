---
title: Criar usuário
description: Criar um novo objeto user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d5e3fe1d4b1b2dcf27de3915ffd49cd38ccb91d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028788"
---
# <a name="create-user"></a><span data-ttu-id="6cb5e-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="6cb5e-103">Create user</span></span>

<span data-ttu-id="6cb5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cb5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cb5e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cb5e-106">Criar um novo objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="6cb5e-106">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cb5e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6cb5e-107">Prerequisites</span></span>
<span data-ttu-id="6cb5e-108">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6cb5e-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cb5e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="6cb5e-110">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-110">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="6cb5e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cb5e-111">Permission type</span></span>|<span data-ttu-id="6cb5e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6cb5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cb5e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cb5e-113">Delegated (work or school account)</span></span>| <span data-ttu-id="6cb5e-114">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="6cb5e-114">_varies by context_</span></span> |
| <span data-ttu-id="6cb5e-115">&nbsp;&nbsp;Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="6cb5e-115">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="6cb5e-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cb5e-116">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="6cb5e-117">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="6cb5e-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="6cb5e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cb5e-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="6cb5e-119">&nbsp;&nbsp;Integração</span><span class="sxs-lookup"><span data-stu-id="6cb5e-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="6cb5e-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cb5e-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="6cb5e-121">&nbsp;&nbsp;Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="6cb5e-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="6cb5e-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cb5e-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="6cb5e-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cb5e-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cb5e-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-124">Not supported.</span></span>|
|<span data-ttu-id="6cb5e-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cb5e-125">Application</span></span>|<span data-ttu-id="6cb5e-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cb5e-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cb5e-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="6cb5e-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb5e-128">Request headers</span></span>
|<span data-ttu-id="6cb5e-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6cb5e-129">Header</span></span>|<span data-ttu-id="6cb5e-130">Valor</span><span class="sxs-lookup"><span data-stu-id="6cb5e-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cb5e-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cb5e-131">Authorization</span></span>|<span data-ttu-id="6cb5e-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cb5e-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6cb5e-133">Accept</span></span>|<span data-ttu-id="6cb5e-134">application/json</span><span class="sxs-lookup"><span data-stu-id="6cb5e-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cb5e-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb5e-135">Request body</span></span>
<span data-ttu-id="6cb5e-136">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="6cb5e-137">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="6cb5e-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cb5e-138">Property</span></span>|<span data-ttu-id="6cb5e-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cb5e-139">Type</span></span>|<span data-ttu-id="6cb5e-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cb5e-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cb5e-141">id</span><span class="sxs-lookup"><span data-stu-id="6cb5e-141">id</span></span>|<span data-ttu-id="6cb5e-142">String</span><span class="sxs-lookup"><span data-stu-id="6cb5e-142">String</span></span>|<span data-ttu-id="6cb5e-143">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="6cb5e-144">**Integração**</span><span class="sxs-lookup"><span data-stu-id="6cb5e-144">**Onboarding**</span></span>|
|<span data-ttu-id="6cb5e-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="6cb5e-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="6cb5e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6cb5e-146">Int32</span></span>|<span data-ttu-id="6cb5e-147">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="6cb5e-148">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="6cb5e-149">O suporte à propriedade do corpo da solicitação varia de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="6cb5e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cb5e-150">Response</span></span>
<span data-ttu-id="6cb5e-151">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cb5e-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cb5e-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cb5e-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb5e-153">Request</span></span>
<span data-ttu-id="6cb5e-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="6cb5e-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cb5e-155">Response</span></span>
<span data-ttu-id="6cb5e-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-156">Here is an example of the response.</span></span> <span data-ttu-id="6cb5e-157">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6cb5e-158">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="6cb5e-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```









