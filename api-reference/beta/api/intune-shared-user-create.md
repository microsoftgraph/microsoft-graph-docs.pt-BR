---
title: Criar usuário
description: Criar um novo objeto user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a78060243259ace0efed84f964cdd9ab7bd29cd0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939505"
---
# <a name="create-user"></a><span data-ttu-id="56911-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="56911-103">Create user</span></span>

> <span data-ttu-id="56911-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="56911-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="56911-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="56911-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56911-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56911-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56911-107">Criar um novo objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="56911-107">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56911-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56911-108">Prerequisites</span></span>

<span data-ttu-id="56911-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="56911-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="56911-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56911-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="56911-111">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="56911-111">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="56911-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56911-112">Permission type</span></span>|<span data-ttu-id="56911-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56911-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56911-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56911-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="56911-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="56911-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="56911-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56911-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="56911-117">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="56911-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="56911-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56911-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="56911-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="56911-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="56911-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56911-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="56911-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="56911-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="56911-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56911-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="56911-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56911-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56911-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56911-124">Not supported.</span></span>|
|<span data-ttu-id="56911-125">Application</span><span class="sxs-lookup"><span data-stu-id="56911-125">Application</span></span>||
| <span data-ttu-id="56911-126">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="56911-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="56911-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56911-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="56911-128">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="56911-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="56911-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56911-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="56911-130">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="56911-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="56911-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56911-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="56911-132">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="56911-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="56911-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56911-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56911-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56911-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="56911-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56911-135">Request headers</span></span>

|<span data-ttu-id="56911-136">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56911-136">Header</span></span>|<span data-ttu-id="56911-137">Valor</span><span class="sxs-lookup"><span data-stu-id="56911-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56911-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="56911-138">Authorization</span></span>|<span data-ttu-id="56911-139">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56911-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56911-140">Aceitar</span><span class="sxs-lookup"><span data-stu-id="56911-140">Accept</span></span>|<span data-ttu-id="56911-141">application/json</span><span class="sxs-lookup"><span data-stu-id="56911-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56911-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56911-142">Request body</span></span>

<span data-ttu-id="56911-143">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="56911-143">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="56911-144">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="56911-144">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="56911-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56911-145">Property</span></span>|<span data-ttu-id="56911-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="56911-146">Type</span></span>|<span data-ttu-id="56911-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="56911-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56911-148">id</span><span class="sxs-lookup"><span data-stu-id="56911-148">id</span></span>|<span data-ttu-id="56911-149">String</span><span class="sxs-lookup"><span data-stu-id="56911-149">String</span></span>|<span data-ttu-id="56911-150">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="56911-150">Unique identifier of the user.</span></span>|
|<span data-ttu-id="56911-151">**Integração**</span><span class="sxs-lookup"><span data-stu-id="56911-151">**On-boarding**</span></span>||
|<span data-ttu-id="56911-152">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="56911-152">deviceEnrollmentLimit</span></span>|<span data-ttu-id="56911-153">Int32</span><span class="sxs-lookup"><span data-stu-id="56911-153">Int32</span></span>|<span data-ttu-id="56911-154">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="56911-154">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="56911-155">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="56911-155">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="56911-156">O suporte à propriedade do corpo da solicitação varia de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="56911-156">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="56911-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="56911-157">Response</span></span>

<span data-ttu-id="56911-158">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56911-158">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56911-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56911-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="56911-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56911-160">Request</span></span>

<span data-ttu-id="56911-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56911-161">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="56911-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="56911-162">Response</span></span>

<span data-ttu-id="56911-163">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56911-163">Here is an example of the response.</span></span> <span data-ttu-id="56911-164">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="56911-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="56911-165">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="56911-165">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```











