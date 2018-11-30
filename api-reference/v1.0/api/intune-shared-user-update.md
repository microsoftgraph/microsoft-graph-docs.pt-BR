---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
ms.openlocfilehash: cfb8a7d46d8383cdaae4f012cff4ed0a0ad93594
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005913"
---
# <a name="update-user"></a><span data-ttu-id="d3d8a-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="d3d8a-103">Update user</span></span>

> <span data-ttu-id="d3d8a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d3d8a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3d8a-105">Atualizar as propriedades de um objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="d3d8a-105">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3d8a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3d8a-106">Prerequisites</span></span>
<span data-ttu-id="d3d8a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3d8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3d8a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3d8a-109">Permission type</span></span>|<span data-ttu-id="d3d8a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3d8a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3d8a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3d8a-111">Delegated (work or school account)</span></span>| <span data-ttu-id="d3d8a-112">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="d3d8a-112">_varies by context_</span></span>|
| <span data-ttu-id="d3d8a-113">&nbsp;&nbsp; Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="d3d8a-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="d3d8a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3d8a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="d3d8a-115">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="d3d8a-115">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="d3d8a-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3d8a-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="d3d8a-117">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="d3d8a-117">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="d3d8a-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3d8a-118">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d3d8a-119">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="d3d8a-119">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="d3d8a-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3d8a-120">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="d3d8a-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3d8a-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3d8a-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3d8a-122">Not supported.</span></span>|
|<span data-ttu-id="d3d8a-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3d8a-123">Application</span></span>|<span data-ttu-id="d3d8a-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3d8a-124">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3d8a-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3d8a-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="d3d8a-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3d8a-126">Request headers</span></span>
|<span data-ttu-id="d3d8a-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3d8a-127">Header</span></span>|<span data-ttu-id="d3d8a-128">Valor</span><span class="sxs-lookup"><span data-stu-id="d3d8a-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3d8a-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3d8a-129">Authorization</span></span>|<span data-ttu-id="d3d8a-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3d8a-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3d8a-131">Accept</span><span class="sxs-lookup"><span data-stu-id="d3d8a-131">Accept</span></span>|<span data-ttu-id="d3d8a-132">application/json</span><span class="sxs-lookup"><span data-stu-id="d3d8a-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3d8a-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3d8a-133">Request body</span></span>
<span data-ttu-id="d3d8a-134">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="d3d8a-134">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="d3d8a-135">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="d3d8a-135">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="d3d8a-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3d8a-136">Property</span></span>|<span data-ttu-id="d3d8a-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3d8a-137">Type</span></span>|<span data-ttu-id="d3d8a-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3d8a-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3d8a-139">id</span><span class="sxs-lookup"><span data-stu-id="d3d8a-139">id</span></span>|<span data-ttu-id="d3d8a-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3d8a-140">String</span></span>|<span data-ttu-id="d3d8a-141">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="d3d8a-141">Unique identifier of the user.</span></span>|
|<span data-ttu-id="d3d8a-142">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="d3d8a-142">**Onboarding**</span></span>|
|<span data-ttu-id="d3d8a-143">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="d3d8a-143">deviceEnrollmentLimit</span></span>|<span data-ttu-id="d3d8a-144">Int32</span><span class="sxs-lookup"><span data-stu-id="d3d8a-144">Int32</span></span>|<span data-ttu-id="d3d8a-145">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="d3d8a-145">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="d3d8a-146">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="d3d8a-146">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="d3d8a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3d8a-147">Response</span></span>
<span data-ttu-id="d3d8a-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune-shared-user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3d8a-148">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3d8a-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3d8a-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3d8a-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3d8a-150">Request</span></span>
<span data-ttu-id="d3d8a-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3d8a-151">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="d3d8a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3d8a-152">Response</span></span>
<span data-ttu-id="d3d8a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3d8a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



