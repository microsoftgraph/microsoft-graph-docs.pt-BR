---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 42959c59740332f3d330f9938ac284ac837e728f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411255"
---
# <a name="list-users"></a><span data-ttu-id="1f1af-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="1f1af-103">List users</span></span>

<span data-ttu-id="1f1af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f1af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f1af-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f1af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f1af-106">Listar propriedades e relações de objetos de [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="1f1af-106">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f1af-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1f1af-107">Prerequisites</span></span>
<span data-ttu-id="1f1af-108">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1f1af-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1f1af-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f1af-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="1f1af-110">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="1f1af-110">The specific permission depends on the context.</span></span>

|<span data-ttu-id="1f1af-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f1af-111">Permission type</span></span>|<span data-ttu-id="1f1af-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1f1af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f1af-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f1af-113">Delegated (work or school account)</span></span>| <span data-ttu-id="1f1af-114">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="1f1af-114">_varies by context_</span></span>|
| <span data-ttu-id="1f1af-115">&nbsp;&nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="1f1af-115">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="1f1af-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f1af-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="1f1af-117">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="1f1af-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="1f1af-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f1af-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="1f1af-119">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="1f1af-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="1f1af-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f1af-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="1f1af-121">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="1f1af-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="1f1af-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f1af-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="1f1af-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f1af-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f1af-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f1af-124">Not supported.</span></span>|
|<span data-ttu-id="1f1af-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f1af-125">Application</span></span>|<span data-ttu-id="1f1af-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f1af-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f1af-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f1af-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="1f1af-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f1af-128">Request headers</span></span>
|<span data-ttu-id="1f1af-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f1af-129">Header</span></span>|<span data-ttu-id="1f1af-130">Valor</span><span class="sxs-lookup"><span data-stu-id="1f1af-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f1af-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f1af-131">Authorization</span></span>|<span data-ttu-id="1f1af-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f1af-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f1af-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1f1af-133">Accept</span></span>|<span data-ttu-id="1f1af-134">application/json</span><span class="sxs-lookup"><span data-stu-id="1f1af-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f1af-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f1af-135">Request body</span></span>
<span data-ttu-id="1f1af-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f1af-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f1af-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f1af-137">Response</span></span>
<span data-ttu-id="1f1af-138">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f1af-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f1af-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f1af-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f1af-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f1af-140">Request</span></span>
<span data-ttu-id="1f1af-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f1af-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="1f1af-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f1af-142">Response</span></span>
<span data-ttu-id="1f1af-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f1af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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






