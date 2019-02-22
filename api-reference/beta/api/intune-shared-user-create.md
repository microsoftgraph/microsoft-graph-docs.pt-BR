---
title: Criar usuário
description: Criar um novo objeto user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e60d00ec008ca255459440e6d2bb888a2195f6af
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141437"
---
# <a name="create-user"></a><span data-ttu-id="be305-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="be305-103">Create user</span></span>

> <span data-ttu-id="be305-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="be305-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="be305-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="be305-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be305-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="be305-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be305-107">Criar um novo objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="be305-107">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be305-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be305-108">Prerequisites</span></span>

<span data-ttu-id="be305-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="be305-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="be305-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be305-110">To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>  <span data-ttu-id="be305-111">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="be305-111">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="be305-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be305-112">Permission type</span></span>|<span data-ttu-id="be305-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="be305-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be305-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be305-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="be305-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="be305-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="be305-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be305-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="be305-117">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="be305-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="be305-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be305-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="be305-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="be305-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="be305-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be305-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="be305-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="be305-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="be305-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be305-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="be305-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be305-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be305-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be305-124">Not supported.</span></span>|
|<span data-ttu-id="be305-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be305-125">Application</span></span>|<span data-ttu-id="be305-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be305-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be305-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be305-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="be305-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be305-128">Request headers</span></span>

|<span data-ttu-id="be305-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be305-129">Header</span></span>|<span data-ttu-id="be305-130">Valor</span><span class="sxs-lookup"><span data-stu-id="be305-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be305-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="be305-131">Authorization</span></span>|<span data-ttu-id="be305-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be305-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be305-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="be305-133">Accept</span></span>|<span data-ttu-id="be305-134">application/json</span><span class="sxs-lookup"><span data-stu-id="be305-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be305-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be305-135">Request body</span></span>

<span data-ttu-id="be305-136">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="be305-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="be305-137">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="be305-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="be305-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be305-138">Property</span></span>|<span data-ttu-id="be305-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="be305-139">Type</span></span>|<span data-ttu-id="be305-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="be305-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be305-141">id</span><span class="sxs-lookup"><span data-stu-id="be305-141">id</span></span>|<span data-ttu-id="be305-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be305-142">String</span></span>|<span data-ttu-id="be305-143">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="be305-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="be305-144">**Integração**</span><span class="sxs-lookup"><span data-stu-id="be305-144">**On-boarding**</span></span>||
|<span data-ttu-id="be305-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="be305-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="be305-146">Int32</span><span class="sxs-lookup"><span data-stu-id="be305-146">Int32</span></span>|<span data-ttu-id="be305-147">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="be305-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="be305-148">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="be305-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="be305-149">O suporte à propriedade do corpo da solicitação varia de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="be305-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="be305-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="be305-150">Response</span></span>

<span data-ttu-id="be305-151">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be305-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be305-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be305-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="be305-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be305-153">Request</span></span>

<span data-ttu-id="be305-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be305-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="be305-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="be305-155">Response</span></span>

<span data-ttu-id="be305-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be305-156">Here is an example of the response.</span></span> <span data-ttu-id="be305-157">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="be305-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="be305-158">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="be305-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



