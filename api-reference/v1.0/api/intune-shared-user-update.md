---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8fb82586ea0fda24297179963b730a097b2d81fa
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251346"
---
# <a name="update-user"></a><span data-ttu-id="902ea-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="902ea-103">Update user</span></span>

> <span data-ttu-id="902ea-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="902ea-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="902ea-105">Atualizar as propriedades de um objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="902ea-105">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="902ea-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="902ea-106">Prerequisites</span></span>
<span data-ttu-id="902ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="902ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="902ea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="902ea-109">Permission type</span></span>|<span data-ttu-id="902ea-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="902ea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="902ea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="902ea-111">Delegated (work or school account)</span></span>| <span data-ttu-id="902ea-112">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="902ea-112">_varies by context_</span></span>|
| <span data-ttu-id="902ea-113">&nbsp;&nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="902ea-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="902ea-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="902ea-114">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="902ea-115">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="902ea-115">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="902ea-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="902ea-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="902ea-117">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="902ea-117">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="902ea-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="902ea-118">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="902ea-119">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="902ea-119">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="902ea-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="902ea-120">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="902ea-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="902ea-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="902ea-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="902ea-122">Not supported.</span></span>|
|<span data-ttu-id="902ea-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="902ea-123">Application</span></span>|<span data-ttu-id="902ea-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="902ea-124">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="902ea-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="902ea-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="902ea-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="902ea-126">Request headers</span></span>
|<span data-ttu-id="902ea-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="902ea-127">Header</span></span>|<span data-ttu-id="902ea-128">Valor</span><span class="sxs-lookup"><span data-stu-id="902ea-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="902ea-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="902ea-129">Authorization</span></span>|<span data-ttu-id="902ea-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="902ea-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="902ea-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="902ea-131">Accept</span></span>|<span data-ttu-id="902ea-132">application/json</span><span class="sxs-lookup"><span data-stu-id="902ea-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="902ea-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="902ea-133">Request body</span></span>
<span data-ttu-id="902ea-134">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="902ea-134">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="902ea-135">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="902ea-135">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="902ea-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="902ea-136">Property</span></span>|<span data-ttu-id="902ea-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="902ea-137">Type</span></span>|<span data-ttu-id="902ea-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="902ea-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="902ea-139">id</span><span class="sxs-lookup"><span data-stu-id="902ea-139">id</span></span>|<span data-ttu-id="902ea-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="902ea-140">String</span></span>|<span data-ttu-id="902ea-141">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="902ea-141">Unique identifier of the user.</span></span>|
|<span data-ttu-id="902ea-142">**Integração**</span><span class="sxs-lookup"><span data-stu-id="902ea-142">**Onboarding**</span></span>|
|<span data-ttu-id="902ea-143">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="902ea-143">deviceEnrollmentLimit</span></span>|<span data-ttu-id="902ea-144">Int32</span><span class="sxs-lookup"><span data-stu-id="902ea-144">Int32</span></span>|<span data-ttu-id="902ea-145">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="902ea-145">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="902ea-146">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="902ea-146">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="902ea-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="902ea-147">Response</span></span>
<span data-ttu-id="902ea-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune-shared-user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="902ea-148">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="902ea-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="902ea-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="902ea-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="902ea-150">Request</span></span>
<span data-ttu-id="902ea-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="902ea-151">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="902ea-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="902ea-152">Response</span></span>
<span data-ttu-id="902ea-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="902ea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



