---
title: Criar usuário
description: Criar um novo objeto user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 19e8bb3d1074c8413ad0ad636d1eea22d45bd15d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457710"
---
# <a name="create-user"></a><span data-ttu-id="11dfe-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="11dfe-103">Create user</span></span>

<span data-ttu-id="11dfe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11dfe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11dfe-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="11dfe-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="11dfe-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="11dfe-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11dfe-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11dfe-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11dfe-108">Criar um novo objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="11dfe-108">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11dfe-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="11dfe-109">Prerequisites</span></span>

<span data-ttu-id="11dfe-110">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="11dfe-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="11dfe-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11dfe-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="11dfe-112">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="11dfe-112">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="11dfe-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11dfe-113">Permission type</span></span>|<span data-ttu-id="11dfe-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="11dfe-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11dfe-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11dfe-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="11dfe-116">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="11dfe-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="11dfe-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11dfe-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="11dfe-118">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="11dfe-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="11dfe-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11dfe-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="11dfe-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="11dfe-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="11dfe-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11dfe-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="11dfe-122">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="11dfe-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="11dfe-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11dfe-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="11dfe-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11dfe-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11dfe-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11dfe-125">Not supported.</span></span>|
|<span data-ttu-id="11dfe-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11dfe-126">Application</span></span>||
| <span data-ttu-id="11dfe-127">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="11dfe-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="11dfe-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11dfe-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="11dfe-129">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="11dfe-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="11dfe-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11dfe-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="11dfe-131">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="11dfe-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="11dfe-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11dfe-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="11dfe-133">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="11dfe-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="11dfe-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11dfe-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="11dfe-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11dfe-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="11dfe-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11dfe-136">Request headers</span></span>

|<span data-ttu-id="11dfe-137">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11dfe-137">Header</span></span>|<span data-ttu-id="11dfe-138">Valor</span><span class="sxs-lookup"><span data-stu-id="11dfe-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11dfe-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="11dfe-139">Authorization</span></span>|<span data-ttu-id="11dfe-140">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11dfe-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11dfe-141">Aceitar</span><span class="sxs-lookup"><span data-stu-id="11dfe-141">Accept</span></span>|<span data-ttu-id="11dfe-142">application/json</span><span class="sxs-lookup"><span data-stu-id="11dfe-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11dfe-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11dfe-143">Request body</span></span>

<span data-ttu-id="11dfe-144">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="11dfe-144">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="11dfe-145">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="11dfe-145">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="11dfe-146">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11dfe-146">Property</span></span>|<span data-ttu-id="11dfe-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="11dfe-147">Type</span></span>|<span data-ttu-id="11dfe-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="11dfe-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11dfe-149">id</span><span class="sxs-lookup"><span data-stu-id="11dfe-149">id</span></span>|<span data-ttu-id="11dfe-150">String</span><span class="sxs-lookup"><span data-stu-id="11dfe-150">String</span></span>|<span data-ttu-id="11dfe-151">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="11dfe-151">Unique identifier of the user.</span></span>|
|<span data-ttu-id="11dfe-152">**Integração**</span><span class="sxs-lookup"><span data-stu-id="11dfe-152">**On-boarding**</span></span>||
|<span data-ttu-id="11dfe-153">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="11dfe-153">deviceEnrollmentLimit</span></span>|<span data-ttu-id="11dfe-154">Int32</span><span class="sxs-lookup"><span data-stu-id="11dfe-154">Int32</span></span>|<span data-ttu-id="11dfe-155">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="11dfe-155">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="11dfe-156">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="11dfe-156">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="11dfe-157">O suporte à propriedade do corpo da solicitação varia de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="11dfe-157">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="11dfe-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="11dfe-158">Response</span></span>

<span data-ttu-id="11dfe-159">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11dfe-159">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11dfe-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11dfe-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="11dfe-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11dfe-161">Request</span></span>

<span data-ttu-id="11dfe-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11dfe-162">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="11dfe-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="11dfe-163">Response</span></span>

<span data-ttu-id="11dfe-164">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11dfe-164">Here is an example of the response.</span></span> <span data-ttu-id="11dfe-165">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="11dfe-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="11dfe-166">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="11dfe-166">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```









