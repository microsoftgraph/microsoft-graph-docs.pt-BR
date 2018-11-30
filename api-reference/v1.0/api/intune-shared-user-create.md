---
title: Criar usuário
description: Criar um novo objeto user.
ms.openlocfilehash: e79fc06543b2f5d6c827b4f0900c4ba972bf6e74
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006448"
---
# <a name="create-user"></a><span data-ttu-id="b8713-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="b8713-103">Create user</span></span>

> <span data-ttu-id="b8713-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b8713-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8713-105">Criar um novo objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="b8713-105">Create a new [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8713-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8713-106">Prerequisites</span></span>
<span data-ttu-id="b8713-107">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b8713-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b8713-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8713-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="b8713-109">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="b8713-109">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="b8713-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8713-110">Permission type</span></span>|<span data-ttu-id="b8713-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8713-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8713-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8713-112">Delegated (work or school account)</span></span>| <span data-ttu-id="b8713-113">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="b8713-113">_varies by context_</span></span> |
| <span data-ttu-id="b8713-114">&nbsp;&nbsp; Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b8713-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="b8713-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8713-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="b8713-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="b8713-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="b8713-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8713-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="b8713-118">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="b8713-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="b8713-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8713-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="b8713-120">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="b8713-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="b8713-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8713-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="b8713-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8713-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8713-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8713-123">Not supported.</span></span>|
|<span data-ttu-id="b8713-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8713-124">Application</span></span>|<span data-ttu-id="b8713-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8713-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8713-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8713-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="b8713-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8713-127">Request headers</span></span>
|<span data-ttu-id="b8713-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8713-128">Header</span></span>|<span data-ttu-id="b8713-129">Valor</span><span class="sxs-lookup"><span data-stu-id="b8713-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8713-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8713-130">Authorization</span></span>|<span data-ttu-id="b8713-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8713-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8713-132">Accept</span><span class="sxs-lookup"><span data-stu-id="b8713-132">Accept</span></span>|<span data-ttu-id="b8713-133">application/json</span><span class="sxs-lookup"><span data-stu-id="b8713-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8713-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8713-134">Request body</span></span>
<span data-ttu-id="b8713-135">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="b8713-135">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="b8713-136">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="b8713-136">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="b8713-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8713-137">Property</span></span>|<span data-ttu-id="b8713-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8713-138">Type</span></span>|<span data-ttu-id="b8713-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8713-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8713-140">id</span><span class="sxs-lookup"><span data-stu-id="b8713-140">id</span></span>|<span data-ttu-id="b8713-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8713-141">String</span></span>|<span data-ttu-id="b8713-142">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8713-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="b8713-143">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="b8713-143">**Onboarding**</span></span>|
|<span data-ttu-id="b8713-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="b8713-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="b8713-145">Int32</span><span class="sxs-lookup"><span data-stu-id="b8713-145">Int32</span></span>|<span data-ttu-id="b8713-146">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="b8713-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="b8713-147">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="b8713-147">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="b8713-148">Suporte de propriedade de corpo de solicitação varia de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="b8713-148">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="b8713-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8713-149">Response</span></span>
<span data-ttu-id="b8713-150">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8713-150">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8713-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8713-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8713-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8713-152">Request</span></span>
<span data-ttu-id="b8713-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8713-153">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="b8713-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8713-154">Response</span></span>
<span data-ttu-id="b8713-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8713-155">Here is an example of the response.</span></span> <span data-ttu-id="b8713-156">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="b8713-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b8713-157">Propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="b8713-157">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



