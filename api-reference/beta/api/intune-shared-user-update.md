---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e2d2dde7b009e735c336ad3260cfb3064b33b6fb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053689"
---
# <a name="update-user"></a><span data-ttu-id="e962f-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="e962f-103">Update user</span></span>

<span data-ttu-id="e962f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e962f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e962f-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e962f-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e962f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e962f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e962f-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e962f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e962f-108">Atualizar as propriedades de um objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="e962f-108">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e962f-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e962f-109">Prerequisites</span></span>

<span data-ttu-id="e962f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e962f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e962f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e962f-112">Permission type</span></span>|<span data-ttu-id="e962f-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e962f-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e962f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e962f-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e962f-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="e962f-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e962f-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e962f-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="e962f-117">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="e962f-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="e962f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e962f-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="e962f-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="e962f-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e962f-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e962f-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="e962f-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="e962f-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e962f-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e962f-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e962f-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e962f-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e962f-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e962f-124">Not supported.</span></span>|
|<span data-ttu-id="e962f-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e962f-125">Application</span></span>||
| <span data-ttu-id="e962f-126">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="e962f-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e962f-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e962f-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="e962f-128">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="e962f-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="e962f-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e962f-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="e962f-130">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="e962f-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e962f-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e962f-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="e962f-132">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="e962f-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e962f-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e962f-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e962f-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e962f-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="e962f-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e962f-135">Request headers</span></span>

|<span data-ttu-id="e962f-136">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e962f-136">Header</span></span>|<span data-ttu-id="e962f-137">Valor</span><span class="sxs-lookup"><span data-stu-id="e962f-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e962f-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="e962f-138">Authorization</span></span>|<span data-ttu-id="e962f-139">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e962f-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e962f-140">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e962f-140">Accept</span></span>|<span data-ttu-id="e962f-141">application/json</span><span class="sxs-lookup"><span data-stu-id="e962f-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e962f-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e962f-142">Request body</span></span>

<span data-ttu-id="e962f-143">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="e962f-143">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="e962f-144">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="e962f-144">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="e962f-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e962f-145">Property</span></span>|<span data-ttu-id="e962f-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="e962f-146">Type</span></span>|<span data-ttu-id="e962f-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="e962f-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e962f-148">id</span><span class="sxs-lookup"><span data-stu-id="e962f-148">id</span></span>|<span data-ttu-id="e962f-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e962f-149">String</span></span>|<span data-ttu-id="e962f-150">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="e962f-150">Unique identifier of the user.</span></span>|
|<span data-ttu-id="e962f-151">**Integração**</span><span class="sxs-lookup"><span data-stu-id="e962f-151">**Onboarding**</span></span>|
|<span data-ttu-id="e962f-152">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="e962f-152">deviceEnrollmentLimit</span></span>|<span data-ttu-id="e962f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e962f-153">Int32</span></span>|<span data-ttu-id="e962f-154">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="e962f-154">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="e962f-155">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="e962f-155">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="e962f-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="e962f-156">Response</span></span>

<span data-ttu-id="e962f-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune-shared-user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e962f-157">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e962f-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e962f-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="e962f-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e962f-159">Request</span></span>

<span data-ttu-id="e962f-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e962f-160">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="e962f-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="e962f-161">Response</span></span>

<span data-ttu-id="e962f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e962f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```












