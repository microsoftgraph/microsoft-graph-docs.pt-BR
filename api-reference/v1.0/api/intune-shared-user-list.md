---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: tfitzmac
ms.openlocfilehash: 9d68b6855a80262daf359950967517a4ec8faa8c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357138"
---
# <a name="list-users"></a><span data-ttu-id="7a947-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="7a947-103">List users</span></span>

> <span data-ttu-id="7a947-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7a947-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a947-105">Listar propriedades e relações de objetos de [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="7a947-105">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7a947-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7a947-106">Prerequisites</span></span>
<span data-ttu-id="7a947-107">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="7a947-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7a947-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a947-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="7a947-109">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="7a947-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="7a947-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a947-110">Permission type</span></span>|<span data-ttu-id="7a947-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7a947-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a947-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a947-112">Delegated (work or school account)</span></span>| <span data-ttu-id="7a947-113">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="7a947-113">_varies by context_</span></span>|
| <span data-ttu-id="7a947-114">&nbsp;&nbsp; Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="7a947-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="7a947-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a947-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="7a947-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="7a947-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="7a947-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a947-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="7a947-118">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="7a947-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="7a947-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a947-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="7a947-120">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="7a947-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="7a947-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a947-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="7a947-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a947-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a947-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a947-123">Not supported.</span></span>|
|<span data-ttu-id="7a947-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a947-124">Application</span></span>|<span data-ttu-id="7a947-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a947-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a947-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a947-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="7a947-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a947-127">Request headers</span></span>
|<span data-ttu-id="7a947-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a947-128">Header</span></span>|<span data-ttu-id="7a947-129">Valor</span><span class="sxs-lookup"><span data-stu-id="7a947-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a947-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a947-130">Authorization</span></span>|<span data-ttu-id="7a947-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a947-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a947-132">Accept</span><span class="sxs-lookup"><span data-stu-id="7a947-132">Accept</span></span>|<span data-ttu-id="7a947-133">application/json</span><span class="sxs-lookup"><span data-stu-id="7a947-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a947-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a947-134">Request body</span></span>
<span data-ttu-id="7a947-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a947-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a947-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a947-136">Response</span></span>
<span data-ttu-id="7a947-137">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a947-137">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a947-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a947-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a947-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a947-139">Request</span></span>
<span data-ttu-id="7a947-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a947-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="7a947-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a947-141">Response</span></span>
<span data-ttu-id="7a947-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a947-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



