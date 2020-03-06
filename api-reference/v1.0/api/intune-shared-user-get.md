---
title: Obter usuário
description: Leia as propriedades e as relações do objeto user.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e259b1de5dc72b0f8b312e70c0496a9a09d00406
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511989"
---
# <a name="get-user"></a><span data-ttu-id="42932-103">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="42932-103">Get user</span></span>

<span data-ttu-id="42932-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42932-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42932-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42932-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42932-106">Leia as propriedades e as relações do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="42932-106">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42932-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42932-107">Prerequisites</span></span>
<span data-ttu-id="42932-108">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="42932-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="42932-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42932-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="42932-110">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="42932-110">The specific permission depends on the context.</span></span>

|<span data-ttu-id="42932-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42932-111">Permission type</span></span>|<span data-ttu-id="42932-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42932-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42932-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42932-113">Delegated (work or school account)</span></span>| <span data-ttu-id="42932-114">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="42932-114">_varies by context_</span></span>|
| <span data-ttu-id="42932-115">&nbsp;&nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="42932-115">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="42932-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="42932-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="42932-117">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="42932-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="42932-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="42932-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="42932-119">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="42932-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="42932-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="42932-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="42932-121">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="42932-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="42932-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="42932-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="42932-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42932-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42932-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42932-124">Not supported.</span></span>|
|<span data-ttu-id="42932-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42932-125">Application</span></span>|<span data-ttu-id="42932-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42932-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42932-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42932-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42932-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="42932-128">Optional query parameters</span></span>
<span data-ttu-id="42932-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="42932-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="42932-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42932-130">Request headers</span></span>
|<span data-ttu-id="42932-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42932-131">Header</span></span>|<span data-ttu-id="42932-132">Valor</span><span class="sxs-lookup"><span data-stu-id="42932-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42932-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="42932-133">Authorization</span></span>|<span data-ttu-id="42932-134">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42932-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42932-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42932-135">Accept</span></span>|<span data-ttu-id="42932-136">application/json</span><span class="sxs-lookup"><span data-stu-id="42932-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42932-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42932-137">Request body</span></span>
<span data-ttu-id="42932-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42932-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42932-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="42932-139">Response</span></span>
<span data-ttu-id="42932-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42932-140">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42932-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42932-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="42932-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42932-142">Request</span></span>
<span data-ttu-id="42932-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42932-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="42932-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="42932-144">Response</span></span>
<span data-ttu-id="42932-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42932-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```




