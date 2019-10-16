---
title: Criar usuário
description: Criar um novo objeto user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d4297fbb4e6693d422a3c65a81890c9f84b8aeac
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536921"
---
# <a name="create-user"></a><span data-ttu-id="99dbe-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="99dbe-103">Create user</span></span>

> <span data-ttu-id="99dbe-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="99dbe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="99dbe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99dbe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99dbe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99dbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99dbe-107">Criar um novo objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="99dbe-107">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99dbe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99dbe-108">Prerequisites</span></span>

<span data-ttu-id="99dbe-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="99dbe-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="99dbe-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99dbe-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="99dbe-111">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="99dbe-111">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="99dbe-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99dbe-112">Permission type</span></span>|<span data-ttu-id="99dbe-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99dbe-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99dbe-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99dbe-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="99dbe-115">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="99dbe-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="99dbe-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99dbe-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="99dbe-117">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="99dbe-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="99dbe-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99dbe-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="99dbe-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="99dbe-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="99dbe-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99dbe-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="99dbe-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="99dbe-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="99dbe-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99dbe-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="99dbe-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99dbe-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99dbe-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99dbe-124">Not supported.</span></span>|
|<span data-ttu-id="99dbe-125">Application</span><span class="sxs-lookup"><span data-stu-id="99dbe-125">Application</span></span>||
| <span data-ttu-id="99dbe-126">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="99dbe-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="99dbe-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99dbe-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="99dbe-128">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="99dbe-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="99dbe-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99dbe-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="99dbe-130">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="99dbe-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="99dbe-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99dbe-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="99dbe-132">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="99dbe-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="99dbe-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99dbe-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99dbe-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99dbe-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="99dbe-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99dbe-135">Request headers</span></span>

|<span data-ttu-id="99dbe-136">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99dbe-136">Header</span></span>|<span data-ttu-id="99dbe-137">Valor</span><span class="sxs-lookup"><span data-stu-id="99dbe-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99dbe-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="99dbe-138">Authorization</span></span>|<span data-ttu-id="99dbe-139">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99dbe-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99dbe-140">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99dbe-140">Accept</span></span>|<span data-ttu-id="99dbe-141">application/json</span><span class="sxs-lookup"><span data-stu-id="99dbe-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99dbe-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99dbe-142">Request body</span></span>

<span data-ttu-id="99dbe-143">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="99dbe-143">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="99dbe-144">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="99dbe-144">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="99dbe-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99dbe-145">Property</span></span>|<span data-ttu-id="99dbe-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="99dbe-146">Type</span></span>|<span data-ttu-id="99dbe-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="99dbe-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99dbe-148">id</span><span class="sxs-lookup"><span data-stu-id="99dbe-148">id</span></span>|<span data-ttu-id="99dbe-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99dbe-149">String</span></span>|<span data-ttu-id="99dbe-150">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="99dbe-150">Unique identifier of the user.</span></span>|
|<span data-ttu-id="99dbe-151">**Integração**</span><span class="sxs-lookup"><span data-stu-id="99dbe-151">**On-boarding**</span></span>||
|<span data-ttu-id="99dbe-152">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="99dbe-152">deviceEnrollmentLimit</span></span>|<span data-ttu-id="99dbe-153">Int32</span><span class="sxs-lookup"><span data-stu-id="99dbe-153">Int32</span></span>|<span data-ttu-id="99dbe-154">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="99dbe-154">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="99dbe-155">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="99dbe-155">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="99dbe-156">O suporte à propriedade do corpo da solicitação varia de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="99dbe-156">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="99dbe-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="99dbe-157">Response</span></span>

<span data-ttu-id="99dbe-158">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99dbe-158">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99dbe-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99dbe-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="99dbe-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99dbe-160">Request</span></span>

<span data-ttu-id="99dbe-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99dbe-161">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="99dbe-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="99dbe-162">Response</span></span>

<span data-ttu-id="99dbe-163">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99dbe-163">Here is an example of the response.</span></span> <span data-ttu-id="99dbe-164">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="99dbe-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="99dbe-165">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="99dbe-165">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```









