---
title: Criar usuário
description: Criar um novo objeto user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 915e043a7ed17549dd0d5a45b5bf4703dc0a6c46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458088"
---
# <a name="create-user"></a><span data-ttu-id="92097-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="92097-103">Create user</span></span>

<span data-ttu-id="92097-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="92097-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92097-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="92097-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="92097-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="92097-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92097-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92097-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92097-108">Criar um novo objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="92097-108">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92097-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92097-109">Prerequisites</span></span>

<span data-ttu-id="92097-110">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="92097-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="92097-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92097-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="92097-112">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="92097-112">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="92097-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92097-113">Permission type</span></span>|<span data-ttu-id="92097-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92097-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92097-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92097-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="92097-116">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="92097-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="92097-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92097-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="92097-118">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="92097-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="92097-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92097-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="92097-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="92097-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="92097-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92097-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="92097-122">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="92097-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="92097-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92097-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="92097-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92097-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92097-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92097-125">Not supported.</span></span>|
|<span data-ttu-id="92097-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92097-126">Application</span></span>||
| <span data-ttu-id="92097-127">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="92097-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="92097-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92097-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="92097-129">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="92097-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="92097-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92097-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="92097-131">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="92097-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="92097-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92097-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="92097-133">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="92097-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="92097-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92097-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92097-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92097-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="92097-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92097-136">Request headers</span></span>

|<span data-ttu-id="92097-137">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92097-137">Header</span></span>|<span data-ttu-id="92097-138">Valor</span><span class="sxs-lookup"><span data-stu-id="92097-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92097-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="92097-139">Authorization</span></span>|<span data-ttu-id="92097-140">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92097-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92097-141">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92097-141">Accept</span></span>|<span data-ttu-id="92097-142">application/json</span><span class="sxs-lookup"><span data-stu-id="92097-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92097-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92097-143">Request body</span></span>

<span data-ttu-id="92097-144">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="92097-144">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="92097-145">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="92097-145">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="92097-146">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92097-146">Property</span></span>|<span data-ttu-id="92097-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="92097-147">Type</span></span>|<span data-ttu-id="92097-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="92097-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92097-149">id</span><span class="sxs-lookup"><span data-stu-id="92097-149">id</span></span>|<span data-ttu-id="92097-150">String</span><span class="sxs-lookup"><span data-stu-id="92097-150">String</span></span>|<span data-ttu-id="92097-151">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="92097-151">Unique identifier of the user.</span></span>|
|<span data-ttu-id="92097-152">**Integração**</span><span class="sxs-lookup"><span data-stu-id="92097-152">**On-boarding**</span></span>||
|<span data-ttu-id="92097-153">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="92097-153">deviceEnrollmentLimit</span></span>|<span data-ttu-id="92097-154">Int32</span><span class="sxs-lookup"><span data-stu-id="92097-154">Int32</span></span>|<span data-ttu-id="92097-155">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="92097-155">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="92097-156">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="92097-156">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="92097-157">O suporte à propriedade do corpo da solicitação varia de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="92097-157">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="92097-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="92097-158">Response</span></span>

<span data-ttu-id="92097-159">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92097-159">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92097-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92097-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="92097-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92097-161">Request</span></span>

<span data-ttu-id="92097-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92097-162">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="92097-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="92097-163">Response</span></span>

<span data-ttu-id="92097-164">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92097-164">Here is an example of the response.</span></span> <span data-ttu-id="92097-165">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="92097-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="92097-166">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="92097-166">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```











