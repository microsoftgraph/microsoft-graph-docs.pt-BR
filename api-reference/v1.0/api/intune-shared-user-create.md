---
title: Criar usuário
description: Criar um novo objeto user.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 47464435a2b38e5fb6a6649ab4b1f932bd970a89
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512003"
---
# <a name="create-user"></a><span data-ttu-id="cad81-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="cad81-103">Create user</span></span>

<span data-ttu-id="cad81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cad81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cad81-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cad81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cad81-106">Criar um novo objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="cad81-106">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cad81-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cad81-107">Prerequisites</span></span>
<span data-ttu-id="cad81-108">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="cad81-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="cad81-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cad81-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="cad81-110">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="cad81-110">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="cad81-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cad81-111">Permission type</span></span>|<span data-ttu-id="cad81-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cad81-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cad81-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cad81-113">Delegated (work or school account)</span></span>| <span data-ttu-id="cad81-114">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="cad81-114">_varies by context_</span></span> |
| <span data-ttu-id="cad81-115">&nbsp;&nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="cad81-115">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="cad81-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cad81-116">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="cad81-117">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="cad81-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="cad81-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cad81-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="cad81-119">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="cad81-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="cad81-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cad81-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cad81-121">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="cad81-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="cad81-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cad81-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="cad81-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cad81-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cad81-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cad81-124">Not supported.</span></span>|
|<span data-ttu-id="cad81-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cad81-125">Application</span></span>|<span data-ttu-id="cad81-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cad81-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cad81-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cad81-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="cad81-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cad81-128">Request headers</span></span>
|<span data-ttu-id="cad81-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cad81-129">Header</span></span>|<span data-ttu-id="cad81-130">Valor</span><span class="sxs-lookup"><span data-stu-id="cad81-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cad81-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="cad81-131">Authorization</span></span>|<span data-ttu-id="cad81-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cad81-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cad81-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cad81-133">Accept</span></span>|<span data-ttu-id="cad81-134">application/json</span><span class="sxs-lookup"><span data-stu-id="cad81-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cad81-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cad81-135">Request body</span></span>
<span data-ttu-id="cad81-136">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="cad81-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="cad81-137">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="cad81-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="cad81-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cad81-138">Property</span></span>|<span data-ttu-id="cad81-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="cad81-139">Type</span></span>|<span data-ttu-id="cad81-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="cad81-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cad81-141">id</span><span class="sxs-lookup"><span data-stu-id="cad81-141">id</span></span>|<span data-ttu-id="cad81-142">String</span><span class="sxs-lookup"><span data-stu-id="cad81-142">String</span></span>|<span data-ttu-id="cad81-143">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="cad81-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="cad81-144">**Integração**</span><span class="sxs-lookup"><span data-stu-id="cad81-144">**Onboarding**</span></span>|
|<span data-ttu-id="cad81-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="cad81-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="cad81-146">Int32</span><span class="sxs-lookup"><span data-stu-id="cad81-146">Int32</span></span>|<span data-ttu-id="cad81-147">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="cad81-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="cad81-148">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="cad81-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="cad81-149">O suporte à propriedade do corpo da solicitação varia de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="cad81-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="cad81-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="cad81-150">Response</span></span>
<span data-ttu-id="cad81-151">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cad81-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cad81-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cad81-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="cad81-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cad81-153">Request</span></span>
<span data-ttu-id="cad81-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cad81-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="cad81-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="cad81-155">Response</span></span>
<span data-ttu-id="cad81-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cad81-156">Here is an example of the response.</span></span> <span data-ttu-id="cad81-157">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="cad81-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cad81-158">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="cad81-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```




