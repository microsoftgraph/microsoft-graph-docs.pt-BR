---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d06b458b96598c892dc068a13d8aadc728d28505
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732274"
---
# <a name="list-users"></a><span data-ttu-id="02b08-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="02b08-103">List users</span></span>

<span data-ttu-id="02b08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02b08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02b08-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02b08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02b08-106">Listar propriedades e relações de objetos de [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="02b08-106">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02b08-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02b08-107">Prerequisites</span></span>
<span data-ttu-id="02b08-108">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="02b08-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="02b08-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02b08-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="02b08-110">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="02b08-110">The specific permission depends on the context.</span></span>

|<span data-ttu-id="02b08-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02b08-111">Permission type</span></span>|<span data-ttu-id="02b08-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02b08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02b08-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02b08-113">Delegated (work or school account)</span></span>| <span data-ttu-id="02b08-114">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="02b08-114">_varies by context_</span></span>|
| <span data-ttu-id="02b08-115">&nbsp;&nbsp;Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="02b08-115">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="02b08-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="02b08-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="02b08-117">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="02b08-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="02b08-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="02b08-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="02b08-119">&nbsp;&nbsp;Integração</span><span class="sxs-lookup"><span data-stu-id="02b08-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="02b08-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="02b08-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="02b08-121">&nbsp;&nbsp;Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="02b08-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="02b08-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="02b08-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="02b08-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02b08-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02b08-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02b08-124">Not supported.</span></span>|
|<span data-ttu-id="02b08-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02b08-125">Application</span></span>|<span data-ttu-id="02b08-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02b08-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02b08-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02b08-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="02b08-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02b08-128">Request headers</span></span>
|<span data-ttu-id="02b08-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02b08-129">Header</span></span>|<span data-ttu-id="02b08-130">Valor</span><span class="sxs-lookup"><span data-stu-id="02b08-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02b08-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="02b08-131">Authorization</span></span>|<span data-ttu-id="02b08-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02b08-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02b08-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02b08-133">Accept</span></span>|<span data-ttu-id="02b08-134">application/json</span><span class="sxs-lookup"><span data-stu-id="02b08-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02b08-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02b08-135">Request body</span></span>
<span data-ttu-id="02b08-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02b08-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02b08-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="02b08-137">Response</span></span>
<span data-ttu-id="02b08-138">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02b08-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02b08-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02b08-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="02b08-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02b08-140">Request</span></span>
<span data-ttu-id="02b08-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02b08-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="02b08-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="02b08-142">Response</span></span>
<span data-ttu-id="02b08-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02b08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









