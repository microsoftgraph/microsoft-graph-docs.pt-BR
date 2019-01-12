---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 16fe6273ec71c37f0ef6408e3671f42fadcc6123
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959710"
---
# <a name="list-users"></a><span data-ttu-id="e94b8-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="e94b8-103">List users</span></span>

> <span data-ttu-id="e94b8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e94b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e94b8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e94b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e94b8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e94b8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e94b8-107">Listar propriedades e relações de objetos de [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="e94b8-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e94b8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e94b8-108">Prerequisites</span></span>

<span data-ttu-id="e94b8-109">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e94b8-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e94b8-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e94b8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="e94b8-111">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="e94b8-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="e94b8-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e94b8-112">Permission type</span></span>|<span data-ttu-id="e94b8-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e94b8-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e94b8-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e94b8-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e94b8-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="e94b8-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e94b8-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e94b8-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="e94b8-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="e94b8-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="e94b8-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e94b8-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="e94b8-119">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="e94b8-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e94b8-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e94b8-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e94b8-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="e94b8-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e94b8-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e94b8-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="e94b8-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e94b8-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e94b8-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e94b8-124">Not supported.</span></span>|
|<span data-ttu-id="e94b8-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e94b8-125">Application</span></span>|<span data-ttu-id="e94b8-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e94b8-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e94b8-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e94b8-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="e94b8-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e94b8-128">Request headers</span></span>

|<span data-ttu-id="e94b8-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e94b8-129">Header</span></span>|<span data-ttu-id="e94b8-130">Valor</span><span class="sxs-lookup"><span data-stu-id="e94b8-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e94b8-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="e94b8-131">Authorization</span></span>|<span data-ttu-id="e94b8-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e94b8-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e94b8-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e94b8-133">Accept</span></span>|<span data-ttu-id="e94b8-134">application/json</span><span class="sxs-lookup"><span data-stu-id="e94b8-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e94b8-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e94b8-135">Request body</span></span>

<span data-ttu-id="e94b8-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e94b8-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e94b8-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e94b8-137">Response</span></span>

<span data-ttu-id="e94b8-138">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e94b8-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e94b8-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e94b8-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="e94b8-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e94b8-140">Request</span></span>

<span data-ttu-id="e94b8-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e94b8-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="e94b8-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e94b8-142">Response</span></span>

<span data-ttu-id="e94b8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e94b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```



