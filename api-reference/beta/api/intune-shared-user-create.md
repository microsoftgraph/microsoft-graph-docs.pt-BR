---
title: Criar usuário
description: Criar um novo objeto user.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9146f7292e003bb64c958e91d1305544b3980442
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821704"
---
# <a name="create-user"></a><span data-ttu-id="ee3cd-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="ee3cd-103">Create user</span></span>

> <span data-ttu-id="ee3cd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee3cd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee3cd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee3cd-107">Criar um novo objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="ee3cd-107">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee3cd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ee3cd-108">Prerequisites</span></span>

<span data-ttu-id="ee3cd-109">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ee3cd-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee3cd-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="ee3cd-111">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-111">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="ee3cd-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee3cd-112">Permission type</span></span>|<span data-ttu-id="ee3cd-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ee3cd-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee3cd-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee3cd-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ee3cd-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ee3cd-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ee3cd-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee3cd-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="ee3cd-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="ee3cd-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="ee3cd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee3cd-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="ee3cd-119">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="ee3cd-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ee3cd-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee3cd-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="ee3cd-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="ee3cd-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ee3cd-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee3cd-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ee3cd-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee3cd-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee3cd-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-124">Not supported.</span></span>|
|<span data-ttu-id="ee3cd-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee3cd-125">Application</span></span>|<span data-ttu-id="ee3cd-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee3cd-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee3cd-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="ee3cd-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee3cd-128">Request headers</span></span>

|<span data-ttu-id="ee3cd-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee3cd-129">Header</span></span>|<span data-ttu-id="ee3cd-130">Valor</span><span class="sxs-lookup"><span data-stu-id="ee3cd-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee3cd-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee3cd-131">Authorization</span></span>|<span data-ttu-id="ee3cd-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee3cd-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ee3cd-133">Accept</span></span>|<span data-ttu-id="ee3cd-134">application/json</span><span class="sxs-lookup"><span data-stu-id="ee3cd-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee3cd-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee3cd-135">Request body</span></span>

<span data-ttu-id="ee3cd-136">No corpo da solicitação, forneça uma representação JSON do objeto user.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="ee3cd-137">A tabela a seguir mostra as propriedades que são necessárias ao criar user.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="ee3cd-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee3cd-138">Property</span></span>|<span data-ttu-id="ee3cd-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee3cd-139">Type</span></span>|<span data-ttu-id="ee3cd-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee3cd-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee3cd-141">id</span><span class="sxs-lookup"><span data-stu-id="ee3cd-141">id</span></span>|<span data-ttu-id="ee3cd-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee3cd-142">String</span></span>|<span data-ttu-id="ee3cd-143">Identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="ee3cd-144">**Nível de contratação**</span><span class="sxs-lookup"><span data-stu-id="ee3cd-144">**On-boarding**</span></span>||
|<span data-ttu-id="ee3cd-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="ee3cd-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="ee3cd-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ee3cd-146">Int32</span></span>|<span data-ttu-id="ee3cd-147">O limite do número máximo de dispositivos que o usuário tem permissão para inscrever.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="ee3cd-148">Os valores permitidos vão de 5 a 1000.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="ee3cd-149">Suporte de propriedade de corpo de solicitação varia de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="ee3cd-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee3cd-150">Response</span></span>

<span data-ttu-id="ee3cd-151">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee3cd-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee3cd-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee3cd-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee3cd-153">Request</span></span>

<span data-ttu-id="ee3cd-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="ee3cd-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee3cd-155">Response</span></span>

<span data-ttu-id="ee3cd-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-156">Here is an example of the response.</span></span> <span data-ttu-id="ee3cd-157">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ee3cd-158">Propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="ee3cd-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



