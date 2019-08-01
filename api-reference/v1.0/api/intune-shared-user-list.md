---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97575c3d323641fa0a4f86f92bb8290ad0d7c815
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025782"
---
# <a name="list-users"></a><span data-ttu-id="3b058-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="3b058-103">List users</span></span>

> <span data-ttu-id="3b058-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b058-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b058-105">Listar propriedades e relações de objetos de [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="3b058-105">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b058-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b058-106">Prerequisites</span></span>
<span data-ttu-id="3b058-107">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3b058-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3b058-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b058-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="3b058-109">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="3b058-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="3b058-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b058-110">Permission type</span></span>|<span data-ttu-id="3b058-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b058-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b058-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b058-112">Delegated (work or school account)</span></span>| <span data-ttu-id="3b058-113">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="3b058-113">_varies by context_</span></span>|
| <span data-ttu-id="3b058-114">&nbsp;&nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="3b058-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="3b058-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b058-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="3b058-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="3b058-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="3b058-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b058-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="3b058-118">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="3b058-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="3b058-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b058-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="3b058-120">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="3b058-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="3b058-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b058-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="3b058-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b058-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b058-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b058-123">Not supported.</span></span>|
|<span data-ttu-id="3b058-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b058-124">Application</span></span>|<span data-ttu-id="3b058-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b058-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b058-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b058-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="3b058-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b058-127">Request headers</span></span>
|<span data-ttu-id="3b058-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b058-128">Header</span></span>|<span data-ttu-id="3b058-129">Valor</span><span class="sxs-lookup"><span data-stu-id="3b058-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b058-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b058-130">Authorization</span></span>|<span data-ttu-id="3b058-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b058-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b058-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b058-132">Accept</span></span>|<span data-ttu-id="3b058-133">application/json</span><span class="sxs-lookup"><span data-stu-id="3b058-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b058-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b058-134">Request body</span></span>
<span data-ttu-id="3b058-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b058-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b058-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b058-136">Response</span></span>
<span data-ttu-id="3b058-137">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b058-137">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b058-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b058-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b058-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b058-139">Request</span></span>
<span data-ttu-id="3b058-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b058-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="3b058-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b058-141">Response</span></span>
<span data-ttu-id="3b058-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b058-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



