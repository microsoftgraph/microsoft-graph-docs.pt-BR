---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2ebdc1842eb3530a0327326b2c06fa87eb92563a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401856"
---
# <a name="list-users"></a><span data-ttu-id="ac817-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="ac817-103">List users</span></span>

> <span data-ttu-id="ac817-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ac817-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ac817-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ac817-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac817-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ac817-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac817-107">Listar propriedades e relações de objetos de [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="ac817-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac817-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ac817-108">Prerequisites</span></span>

<span data-ttu-id="ac817-109">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="ac817-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ac817-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac817-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="ac817-111">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="ac817-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="ac817-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac817-112">Permission type</span></span>|<span data-ttu-id="ac817-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ac817-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac817-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac817-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ac817-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ac817-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ac817-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac817-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="ac817-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="ac817-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="ac817-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac817-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="ac817-119">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="ac817-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ac817-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac817-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ac817-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="ac817-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ac817-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac817-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="ac817-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac817-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac817-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac817-124">Not supported.</span></span>|
|<span data-ttu-id="ac817-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac817-125">Application</span></span>|<span data-ttu-id="ac817-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac817-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac817-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac817-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="ac817-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac817-128">Request headers</span></span>

|<span data-ttu-id="ac817-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac817-129">Header</span></span>|<span data-ttu-id="ac817-130">Valor</span><span class="sxs-lookup"><span data-stu-id="ac817-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac817-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac817-131">Authorization</span></span>|<span data-ttu-id="ac817-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac817-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac817-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ac817-133">Accept</span></span>|<span data-ttu-id="ac817-134">application/json</span><span class="sxs-lookup"><span data-stu-id="ac817-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac817-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac817-135">Request body</span></span>

<span data-ttu-id="ac817-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac817-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac817-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac817-137">Response</span></span>

<span data-ttu-id="ac817-138">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac817-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac817-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac817-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac817-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac817-140">Request</span></span>

<span data-ttu-id="ac817-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac817-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="ac817-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac817-142">Response</span></span>

<span data-ttu-id="ac817-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac817-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



