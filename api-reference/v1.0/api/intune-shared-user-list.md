---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b3981047311673be8c640a35dbc862416427fa31
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576630"
---
# <a name="list-users"></a><span data-ttu-id="c88ae-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="c88ae-103">List users</span></span>

> <span data-ttu-id="c88ae-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c88ae-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c88ae-105">Listar propriedades e relações de objetos de [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="c88ae-105">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c88ae-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c88ae-106">Prerequisites</span></span>
<span data-ttu-id="c88ae-107">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c88ae-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c88ae-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c88ae-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="c88ae-109">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="c88ae-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="c88ae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c88ae-110">Permission type</span></span>|<span data-ttu-id="c88ae-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c88ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c88ae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c88ae-112">Delegated (work or school account)</span></span>| <span data-ttu-id="c88ae-113">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="c88ae-113">_varies by context_</span></span>|
| <span data-ttu-id="c88ae-114">&nbsp;&nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="c88ae-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="c88ae-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c88ae-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="c88ae-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="c88ae-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="c88ae-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c88ae-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="c88ae-118">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="c88ae-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="c88ae-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c88ae-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c88ae-120">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="c88ae-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="c88ae-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c88ae-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="c88ae-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c88ae-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c88ae-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c88ae-123">Not supported.</span></span>|
|<span data-ttu-id="c88ae-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c88ae-124">Application</span></span>|<span data-ttu-id="c88ae-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c88ae-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c88ae-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c88ae-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="c88ae-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c88ae-127">Request headers</span></span>
|<span data-ttu-id="c88ae-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c88ae-128">Header</span></span>|<span data-ttu-id="c88ae-129">Valor</span><span class="sxs-lookup"><span data-stu-id="c88ae-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c88ae-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="c88ae-130">Authorization</span></span>|<span data-ttu-id="c88ae-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c88ae-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c88ae-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c88ae-132">Accept</span></span>|<span data-ttu-id="c88ae-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c88ae-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c88ae-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c88ae-134">Request body</span></span>
<span data-ttu-id="c88ae-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c88ae-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c88ae-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c88ae-136">Response</span></span>
<span data-ttu-id="c88ae-137">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c88ae-137">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c88ae-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c88ae-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c88ae-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c88ae-139">Request</span></span>
<span data-ttu-id="c88ae-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c88ae-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="c88ae-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c88ae-141">Response</span></span>
<span data-ttu-id="c88ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c88ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



