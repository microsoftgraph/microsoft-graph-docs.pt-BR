---
title: Criar usuário
description: Criar um novo objeto user.
author: tfitzmac
ms.openlocfilehash: 9d71aeca95c1a8b3efa676cca80652fb7fd124fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331637"
---
# <a name="create-user"></a><span data-ttu-id="92924-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="92924-103">Create user</span></span>

> <span data-ttu-id="92924-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="92924-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92924-105">Criar um novo objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="92924-105">Create a new [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="92924-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92924-106">Prerequisites</span></span>
<span data-ttu-id="92924-107">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="92924-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="92924-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92924-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="92924-109">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="92924-109">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="92924-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92924-110">Permission type</span></span>|<span data-ttu-id="92924-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92924-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92924-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92924-112">Delegated (work or school account)</span></span>| <span data-ttu-id="92924-113">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="92924-113">_varies by context_</span></span> |
| <span data-ttu-id="92924-114">&nbsp;&nbsp; Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="92924-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="92924-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92924-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="92924-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="92924-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="92924-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92924-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="92924-118">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="92924-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="92924-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92924-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="92924-120">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="92924-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="92924-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92924-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="92924-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92924-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92924-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92924-123">Not supported.</span></span>|
|<span data-ttu-id="92924-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92924-124">Application</span></span>|<span data-ttu-id="92924-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92924-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92924-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92924-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="92924-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92924-127">Request headers</span></span>
|<span data-ttu-id="92924-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92924-128">Header</span></span>|<span data-ttu-id="92924-129">Valor</span><span class="sxs-lookup"><span data-stu-id="92924-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92924-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="92924-130">Authorization</span></span>|<span data-ttu-id="92924-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92924-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92924-132">Accept</span><span class="sxs-lookup"><span data-stu-id="92924-132">Accept</span></span>|<span data-ttu-id="92924-133">application/json</span><span class="sxs-lookup"><span data-stu-id="92924-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92924-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92924-134">Request body</span></span>
<span data-ttu-id="92924-135">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="92924-135">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="92924-136">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="92924-136">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="92924-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92924-137">Property</span></span>|<span data-ttu-id="92924-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="92924-138">Type</span></span>|<span data-ttu-id="92924-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="92924-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92924-140">id</span><span class="sxs-lookup"><span data-stu-id="92924-140">id</span></span>|<span data-ttu-id="92924-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92924-141">String</span></span>|<span data-ttu-id="92924-142">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="92924-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="92924-143">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="92924-143">**Onboarding**</span></span>|
|<span data-ttu-id="92924-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="92924-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="92924-145">Int32</span><span class="sxs-lookup"><span data-stu-id="92924-145">Int32</span></span>|<span data-ttu-id="92924-146">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="92924-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="92924-147">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="92924-147">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="92924-148">Suporte de propriedade de corpo de solicitação varia de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="92924-148">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="92924-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="92924-149">Response</span></span>
<span data-ttu-id="92924-150">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92924-150">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92924-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92924-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="92924-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92924-152">Request</span></span>
<span data-ttu-id="92924-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92924-153">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="92924-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="92924-154">Response</span></span>
<span data-ttu-id="92924-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92924-155">Here is an example of the response.</span></span> <span data-ttu-id="92924-156">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="92924-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="92924-157">Propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="92924-157">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



