---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 60bf52574564815f2b60f1c4d81201ea3eef5e28
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537871"
---
# <a name="update-user"></a><span data-ttu-id="d6769-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="d6769-103">Update user</span></span>

> <span data-ttu-id="d6769-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d6769-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d6769-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d6769-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6769-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6769-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6769-107">Atualizar as propriedades de um objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="d6769-107">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6769-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6769-108">Prerequisites</span></span>

<span data-ttu-id="d6769-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6769-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6769-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6769-111">Permission type</span></span>|<span data-ttu-id="d6769-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6769-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6769-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6769-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d6769-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="d6769-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d6769-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6769-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d6769-116">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="d6769-116">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="d6769-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6769-117">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d6769-118">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="d6769-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d6769-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6769-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="d6769-120">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="d6769-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d6769-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6769-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d6769-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6769-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6769-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6769-123">Not supported.</span></span>|
|<span data-ttu-id="d6769-124">Application</span><span class="sxs-lookup"><span data-stu-id="d6769-124">Application</span></span>||
| <span data-ttu-id="d6769-125">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="d6769-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d6769-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6769-126">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d6769-127">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="d6769-127">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="d6769-128">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6769-128">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d6769-129">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="d6769-129">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d6769-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6769-130">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="d6769-131">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="d6769-131">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d6769-132">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6769-132">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6769-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6769-133">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="d6769-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6769-134">Request headers</span></span>

|<span data-ttu-id="d6769-135">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6769-135">Header</span></span>|<span data-ttu-id="d6769-136">Valor</span><span class="sxs-lookup"><span data-stu-id="d6769-136">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6769-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6769-137">Authorization</span></span>|<span data-ttu-id="d6769-138">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6769-138">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6769-139">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6769-139">Accept</span></span>|<span data-ttu-id="d6769-140">application/json</span><span class="sxs-lookup"><span data-stu-id="d6769-140">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6769-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6769-141">Request body</span></span>

<span data-ttu-id="d6769-142">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="d6769-142">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="d6769-143">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="d6769-143">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="d6769-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6769-144">Property</span></span>|<span data-ttu-id="d6769-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6769-145">Type</span></span>|<span data-ttu-id="d6769-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6769-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6769-147">id</span><span class="sxs-lookup"><span data-stu-id="d6769-147">id</span></span>|<span data-ttu-id="d6769-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6769-148">String</span></span>|<span data-ttu-id="d6769-149">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="d6769-149">Unique identifier of the user.</span></span>|
|<span data-ttu-id="d6769-150">**Integração**</span><span class="sxs-lookup"><span data-stu-id="d6769-150">**Onboarding**</span></span>|
|<span data-ttu-id="d6769-151">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="d6769-151">deviceEnrollmentLimit</span></span>|<span data-ttu-id="d6769-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d6769-152">Int32</span></span>|<span data-ttu-id="d6769-153">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="d6769-153">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="d6769-154">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="d6769-154">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="d6769-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6769-155">Response</span></span>

<span data-ttu-id="d6769-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune-shared-user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6769-156">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6769-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6769-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6769-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6769-158">Request</span></span>

<span data-ttu-id="d6769-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6769-159">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="d6769-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6769-160">Response</span></span>

<span data-ttu-id="d6769-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6769-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```









