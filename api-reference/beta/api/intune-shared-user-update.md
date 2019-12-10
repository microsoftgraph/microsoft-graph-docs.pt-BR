---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d394a3c357a53d8fce36b605ecaca7c7595564b5
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939427"
---
# <a name="update-user"></a><span data-ttu-id="540ee-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="540ee-103">Update user</span></span>

> <span data-ttu-id="540ee-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="540ee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="540ee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="540ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="540ee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="540ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="540ee-107">Atualizar as propriedades de um objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="540ee-107">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="540ee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="540ee-108">Prerequisites</span></span>

<span data-ttu-id="540ee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="540ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="540ee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="540ee-111">Permission type</span></span>|<span data-ttu-id="540ee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="540ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="540ee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="540ee-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="540ee-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="540ee-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="540ee-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="540ee-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="540ee-116">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="540ee-116">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="540ee-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="540ee-117">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="540ee-118">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="540ee-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="540ee-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="540ee-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="540ee-120">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="540ee-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="540ee-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="540ee-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="540ee-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="540ee-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="540ee-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="540ee-123">Not supported.</span></span>|
|<span data-ttu-id="540ee-124">Application</span><span class="sxs-lookup"><span data-stu-id="540ee-124">Application</span></span>||
| <span data-ttu-id="540ee-125">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="540ee-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="540ee-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="540ee-126">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="540ee-127">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="540ee-127">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="540ee-128">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="540ee-128">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="540ee-129">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="540ee-129">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="540ee-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="540ee-130">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="540ee-131">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="540ee-131">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="540ee-132">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="540ee-132">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="540ee-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="540ee-133">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="540ee-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="540ee-134">Request headers</span></span>

|<span data-ttu-id="540ee-135">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="540ee-135">Header</span></span>|<span data-ttu-id="540ee-136">Valor</span><span class="sxs-lookup"><span data-stu-id="540ee-136">Value</span></span>|
|:---|:---|
|<span data-ttu-id="540ee-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="540ee-137">Authorization</span></span>|<span data-ttu-id="540ee-138">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="540ee-138">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="540ee-139">Aceitar</span><span class="sxs-lookup"><span data-stu-id="540ee-139">Accept</span></span>|<span data-ttu-id="540ee-140">application/json</span><span class="sxs-lookup"><span data-stu-id="540ee-140">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="540ee-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="540ee-141">Request body</span></span>

<span data-ttu-id="540ee-142">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="540ee-142">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="540ee-143">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="540ee-143">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="540ee-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="540ee-144">Property</span></span>|<span data-ttu-id="540ee-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="540ee-145">Type</span></span>|<span data-ttu-id="540ee-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="540ee-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="540ee-147">id</span><span class="sxs-lookup"><span data-stu-id="540ee-147">id</span></span>|<span data-ttu-id="540ee-148">String</span><span class="sxs-lookup"><span data-stu-id="540ee-148">String</span></span>|<span data-ttu-id="540ee-149">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="540ee-149">Unique identifier of the user.</span></span>|
|<span data-ttu-id="540ee-150">**Integração**</span><span class="sxs-lookup"><span data-stu-id="540ee-150">**Onboarding**</span></span>|
|<span data-ttu-id="540ee-151">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="540ee-151">deviceEnrollmentLimit</span></span>|<span data-ttu-id="540ee-152">Int32</span><span class="sxs-lookup"><span data-stu-id="540ee-152">Int32</span></span>|<span data-ttu-id="540ee-153">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="540ee-153">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="540ee-154">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="540ee-154">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="540ee-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="540ee-155">Response</span></span>

<span data-ttu-id="540ee-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune-shared-user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="540ee-156">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="540ee-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="540ee-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="540ee-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="540ee-158">Request</span></span>

<span data-ttu-id="540ee-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="540ee-159">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="540ee-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="540ee-160">Response</span></span>

<span data-ttu-id="540ee-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="540ee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```











