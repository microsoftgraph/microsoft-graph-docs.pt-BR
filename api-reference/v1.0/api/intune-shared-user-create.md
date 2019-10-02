---
title: Criar usuário
description: Criar um novo objeto user.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8cbdb53286d427223d80bf8b55cef63cbf0416a4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361326"
---
# <a name="create-user"></a><span data-ttu-id="b2055-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="b2055-103">Create user</span></span>

> <span data-ttu-id="b2055-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2055-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2055-105">Criar um novo objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="b2055-105">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2055-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2055-106">Prerequisites</span></span>
<span data-ttu-id="b2055-107">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b2055-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b2055-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2055-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="b2055-109">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="b2055-109">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="b2055-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2055-110">Permission type</span></span>|<span data-ttu-id="b2055-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2055-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2055-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2055-112">Delegated (work or school account)</span></span>| <span data-ttu-id="b2055-113">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="b2055-113">_varies by context_</span></span> |
| <span data-ttu-id="b2055-114">&nbsp;&nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="b2055-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="b2055-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2055-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="b2055-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="b2055-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="b2055-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2055-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="b2055-118">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="b2055-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="b2055-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2055-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="b2055-120">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="b2055-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="b2055-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2055-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="b2055-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2055-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2055-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2055-123">Not supported.</span></span>|
|<span data-ttu-id="b2055-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2055-124">Application</span></span>|<span data-ttu-id="b2055-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2055-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2055-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2055-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="b2055-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2055-127">Request headers</span></span>
|<span data-ttu-id="b2055-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2055-128">Header</span></span>|<span data-ttu-id="b2055-129">Valor</span><span class="sxs-lookup"><span data-stu-id="b2055-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2055-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2055-130">Authorization</span></span>|<span data-ttu-id="b2055-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2055-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2055-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2055-132">Accept</span></span>|<span data-ttu-id="b2055-133">application/json</span><span class="sxs-lookup"><span data-stu-id="b2055-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2055-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2055-134">Request body</span></span>
<span data-ttu-id="b2055-135">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="b2055-135">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="b2055-136">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="b2055-136">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="b2055-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2055-137">Property</span></span>|<span data-ttu-id="b2055-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2055-138">Type</span></span>|<span data-ttu-id="b2055-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2055-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2055-140">id</span><span class="sxs-lookup"><span data-stu-id="b2055-140">id</span></span>|<span data-ttu-id="b2055-141">String</span><span class="sxs-lookup"><span data-stu-id="b2055-141">String</span></span>|<span data-ttu-id="b2055-142">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="b2055-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="b2055-143">**Integração**</span><span class="sxs-lookup"><span data-stu-id="b2055-143">**Onboarding**</span></span>|
|<span data-ttu-id="b2055-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="b2055-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="b2055-145">Int32</span><span class="sxs-lookup"><span data-stu-id="b2055-145">Int32</span></span>|<span data-ttu-id="b2055-146">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="b2055-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="b2055-147">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="b2055-147">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="b2055-148">O suporte à propriedade do corpo da solicitação varia de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="b2055-148">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="b2055-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2055-149">Response</span></span>
<span data-ttu-id="b2055-150">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2055-150">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2055-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2055-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2055-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2055-152">Request</span></span>
<span data-ttu-id="b2055-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2055-153">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="b2055-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2055-154">Response</span></span>
<span data-ttu-id="b2055-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2055-155">Here is an example of the response.</span></span> <span data-ttu-id="b2055-156">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="b2055-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b2055-157">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="b2055-157">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```




