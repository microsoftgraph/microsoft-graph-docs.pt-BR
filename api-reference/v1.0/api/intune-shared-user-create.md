---
title: Criar usuário
description: Criar um novo objeto user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 95b01b4b00328c230d55b530cbdef2cb32dfe607
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576822"
---
# <a name="create-user"></a><span data-ttu-id="12e8a-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="12e8a-103">Create user</span></span>

> <span data-ttu-id="12e8a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12e8a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12e8a-105">Criar um novo objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="12e8a-105">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12e8a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12e8a-106">Prerequisites</span></span>
<span data-ttu-id="12e8a-107">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="12e8a-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="12e8a-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12e8a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="12e8a-109">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="12e8a-109">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="12e8a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12e8a-110">Permission type</span></span>|<span data-ttu-id="12e8a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="12e8a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12e8a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12e8a-112">Delegated (work or school account)</span></span>| <span data-ttu-id="12e8a-113">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="12e8a-113">_varies by context_</span></span> |
| <span data-ttu-id="12e8a-114">&nbsp;&nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="12e8a-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="12e8a-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12e8a-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="12e8a-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="12e8a-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="12e8a-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12e8a-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="12e8a-118">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="12e8a-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="12e8a-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12e8a-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="12e8a-120">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="12e8a-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="12e8a-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12e8a-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="12e8a-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12e8a-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12e8a-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12e8a-123">Not supported.</span></span>|
|<span data-ttu-id="12e8a-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12e8a-124">Application</span></span>|<span data-ttu-id="12e8a-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12e8a-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12e8a-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12e8a-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="12e8a-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12e8a-127">Request headers</span></span>
|<span data-ttu-id="12e8a-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12e8a-128">Header</span></span>|<span data-ttu-id="12e8a-129">Valor</span><span class="sxs-lookup"><span data-stu-id="12e8a-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12e8a-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="12e8a-130">Authorization</span></span>|<span data-ttu-id="12e8a-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12e8a-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12e8a-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12e8a-132">Accept</span></span>|<span data-ttu-id="12e8a-133">application/json</span><span class="sxs-lookup"><span data-stu-id="12e8a-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12e8a-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12e8a-134">Request body</span></span>
<span data-ttu-id="12e8a-135">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="12e8a-135">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="12e8a-136">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="12e8a-136">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="12e8a-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12e8a-137">Property</span></span>|<span data-ttu-id="12e8a-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="12e8a-138">Type</span></span>|<span data-ttu-id="12e8a-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="12e8a-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12e8a-140">id</span><span class="sxs-lookup"><span data-stu-id="12e8a-140">id</span></span>|<span data-ttu-id="12e8a-141">String</span><span class="sxs-lookup"><span data-stu-id="12e8a-141">String</span></span>|<span data-ttu-id="12e8a-142">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="12e8a-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="12e8a-143">**Integração**</span><span class="sxs-lookup"><span data-stu-id="12e8a-143">**Onboarding**</span></span>|
|<span data-ttu-id="12e8a-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="12e8a-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="12e8a-145">Int32</span><span class="sxs-lookup"><span data-stu-id="12e8a-145">Int32</span></span>|<span data-ttu-id="12e8a-146">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="12e8a-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="12e8a-147">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="12e8a-147">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="12e8a-148">O suporte à propriedade do corpo da solicitação varia de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="12e8a-148">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="12e8a-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="12e8a-149">Response</span></span>
<span data-ttu-id="12e8a-150">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12e8a-150">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12e8a-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12e8a-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="12e8a-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12e8a-152">Request</span></span>
<span data-ttu-id="12e8a-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12e8a-153">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="12e8a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="12e8a-154">Response</span></span>
<span data-ttu-id="12e8a-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12e8a-155">Here is an example of the response.</span></span> <span data-ttu-id="12e8a-156">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="12e8a-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="12e8a-157">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="12e8a-157">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



