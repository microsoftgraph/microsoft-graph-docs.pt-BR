---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f52e49c86e0e333fbf4f8c52b71c2850c73bc533
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861940"
---
# <a name="update-user"></a><span data-ttu-id="18f41-103">Atualizar usuário</span><span class="sxs-lookup"><span data-stu-id="18f41-103">Update user</span></span>

> <span data-ttu-id="18f41-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="18f41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18f41-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="18f41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18f41-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="18f41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18f41-107">Atualizar as propriedades de um objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="18f41-107">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18f41-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="18f41-108">Prerequisites</span></span>

<span data-ttu-id="18f41-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18f41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18f41-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18f41-111">Permission type</span></span>|<span data-ttu-id="18f41-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="18f41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18f41-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18f41-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="18f41-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="18f41-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="18f41-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f41-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="18f41-116">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="18f41-116">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="18f41-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f41-117">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="18f41-118">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="18f41-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="18f41-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f41-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="18f41-120">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="18f41-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="18f41-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f41-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="18f41-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18f41-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18f41-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18f41-123">Not supported.</span></span>|
|<span data-ttu-id="18f41-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18f41-124">Application</span></span>|<span data-ttu-id="18f41-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18f41-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18f41-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18f41-126">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="18f41-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18f41-127">Request headers</span></span>

|<span data-ttu-id="18f41-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18f41-128">Header</span></span>|<span data-ttu-id="18f41-129">Valor</span><span class="sxs-lookup"><span data-stu-id="18f41-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18f41-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="18f41-130">Authorization</span></span>|<span data-ttu-id="18f41-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18f41-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18f41-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="18f41-132">Accept</span></span>|<span data-ttu-id="18f41-133">application/json</span><span class="sxs-lookup"><span data-stu-id="18f41-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18f41-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18f41-134">Request body</span></span>

<span data-ttu-id="18f41-135">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="18f41-135">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="18f41-136">A tabela a seguir mostra as propriedades que são necessárias ao criar [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="18f41-136">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="18f41-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18f41-137">Property</span></span>|<span data-ttu-id="18f41-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="18f41-138">Type</span></span>|<span data-ttu-id="18f41-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="18f41-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18f41-140">id</span><span class="sxs-lookup"><span data-stu-id="18f41-140">id</span></span>|<span data-ttu-id="18f41-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18f41-141">String</span></span>|<span data-ttu-id="18f41-142">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="18f41-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="18f41-143">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="18f41-143">**Onboarding**</span></span>|
|<span data-ttu-id="18f41-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="18f41-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="18f41-145">Int32</span><span class="sxs-lookup"><span data-stu-id="18f41-145">Int32</span></span>|<span data-ttu-id="18f41-146">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="18f41-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="18f41-147">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="18f41-147">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="18f41-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="18f41-148">Response</span></span>

<span data-ttu-id="18f41-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [user](../resources/intune-shared-user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18f41-149">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18f41-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18f41-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="18f41-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18f41-151">Request</span></span>

<span data-ttu-id="18f41-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18f41-152">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="18f41-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="18f41-153">Response</span></span>

<span data-ttu-id="18f41-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18f41-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



