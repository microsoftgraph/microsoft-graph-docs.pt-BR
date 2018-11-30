---
title: Obter usuário
description: Leia as propriedades e as relações do objeto user.
ms.openlocfilehash: 619f35e5b7e8ffd75a8bcd2db32122dd69a9ac2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006025"
---
# <a name="get-user"></a><span data-ttu-id="211d7-103">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="211d7-103">Get user</span></span>

> <span data-ttu-id="211d7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="211d7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="211d7-105">Leia as propriedades e as relações do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="211d7-105">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="211d7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="211d7-106">Prerequisites</span></span>
<span data-ttu-id="211d7-107">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="211d7-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="211d7-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="211d7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="211d7-109">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="211d7-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="211d7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="211d7-110">Permission type</span></span>|<span data-ttu-id="211d7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="211d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="211d7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="211d7-112">Delegated (work or school account)</span></span>| <span data-ttu-id="211d7-113">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="211d7-113">_varies by context_</span></span>|
| <span data-ttu-id="211d7-114">&nbsp;&nbsp; Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="211d7-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="211d7-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="211d7-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="211d7-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="211d7-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="211d7-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="211d7-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="211d7-118">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="211d7-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="211d7-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="211d7-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="211d7-120">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="211d7-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="211d7-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="211d7-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="211d7-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="211d7-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="211d7-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="211d7-123">Not supported.</span></span>|
|<span data-ttu-id="211d7-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="211d7-124">Application</span></span>|<span data-ttu-id="211d7-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="211d7-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="211d7-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="211d7-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="211d7-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="211d7-127">Optional query parameters</span></span>
<span data-ttu-id="211d7-128">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="211d7-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="211d7-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="211d7-129">Request headers</span></span>
|<span data-ttu-id="211d7-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="211d7-130">Header</span></span>|<span data-ttu-id="211d7-131">Valor</span><span class="sxs-lookup"><span data-stu-id="211d7-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="211d7-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="211d7-132">Authorization</span></span>|<span data-ttu-id="211d7-133">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="211d7-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="211d7-134">Accept</span><span class="sxs-lookup"><span data-stu-id="211d7-134">Accept</span></span>|<span data-ttu-id="211d7-135">application/json</span><span class="sxs-lookup"><span data-stu-id="211d7-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="211d7-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="211d7-136">Request body</span></span>
<span data-ttu-id="211d7-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="211d7-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="211d7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="211d7-138">Response</span></span>
<span data-ttu-id="211d7-139">Se tiver êxito, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="211d7-139">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="211d7-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="211d7-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="211d7-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="211d7-141">Request</span></span>
<span data-ttu-id="211d7-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="211d7-142">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="211d7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="211d7-143">Response</span></span>
<span data-ttu-id="211d7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="211d7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



