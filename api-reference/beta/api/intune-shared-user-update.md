---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3401ae8c2a33e56e69121b5704cc2e45905429be
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422695"
---
# <a name="update-user"></a><span data-ttu-id="12961-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="12961-103">Update user</span></span>

> <span data-ttu-id="12961-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="12961-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="12961-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="12961-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12961-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="12961-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12961-107">Atualizar as propriedades de um objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="12961-107">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12961-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12961-108">Prerequisites</span></span>

<span data-ttu-id="12961-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12961-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12961-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12961-111">Permission type</span></span>|<span data-ttu-id="12961-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="12961-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12961-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12961-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="12961-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="12961-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="12961-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12961-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="12961-116">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="12961-116">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="12961-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12961-117">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="12961-118">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="12961-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="12961-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12961-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="12961-120">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="12961-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="12961-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12961-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="12961-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12961-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12961-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12961-123">Not supported.</span></span>|
|<span data-ttu-id="12961-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12961-124">Application</span></span>|<span data-ttu-id="12961-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12961-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12961-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12961-126">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="12961-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12961-127">Request headers</span></span>

|<span data-ttu-id="12961-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12961-128">Header</span></span>|<span data-ttu-id="12961-129">Valor</span><span class="sxs-lookup"><span data-stu-id="12961-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12961-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="12961-130">Authorization</span></span>|<span data-ttu-id="12961-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12961-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12961-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12961-132">Accept</span></span>|<span data-ttu-id="12961-133">application/json</span><span class="sxs-lookup"><span data-stu-id="12961-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12961-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12961-134">Request body</span></span>

<span data-ttu-id="12961-135">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="12961-135">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="12961-136">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="12961-136">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="12961-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12961-137">Property</span></span>|<span data-ttu-id="12961-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="12961-138">Type</span></span>|<span data-ttu-id="12961-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="12961-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12961-140">id</span><span class="sxs-lookup"><span data-stu-id="12961-140">id</span></span>|<span data-ttu-id="12961-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12961-141">String</span></span>|<span data-ttu-id="12961-142">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="12961-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="12961-143">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="12961-143">**Onboarding**</span></span>|
|<span data-ttu-id="12961-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="12961-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="12961-145">Int32</span><span class="sxs-lookup"><span data-stu-id="12961-145">Int32</span></span>|<span data-ttu-id="12961-146">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="12961-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="12961-147">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="12961-147">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="12961-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="12961-148">Response</span></span>

<span data-ttu-id="12961-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune-shared-user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12961-149">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12961-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12961-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="12961-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12961-151">Request</span></span>

<span data-ttu-id="12961-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12961-152">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="12961-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="12961-153">Response</span></span>

<span data-ttu-id="12961-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12961-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



