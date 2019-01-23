---
title: Obter usuário
description: Leia as propriedades e as relações do objeto user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7e6643fa2beccf83384c454451094473e7c80ac8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419265"
---
# <a name="get-user"></a><span data-ttu-id="f6beb-103">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="f6beb-103">Get user</span></span>

> <span data-ttu-id="f6beb-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f6beb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f6beb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f6beb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6beb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f6beb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6beb-107">Leia as propriedades e as relações do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="f6beb-107">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6beb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f6beb-108">Prerequisites</span></span>

<span data-ttu-id="f6beb-109">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f6beb-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f6beb-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6beb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="f6beb-111">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="f6beb-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="f6beb-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6beb-112">Permission type</span></span>|<span data-ttu-id="f6beb-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f6beb-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6beb-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6beb-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f6beb-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f6beb-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f6beb-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6beb-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="f6beb-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="f6beb-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="f6beb-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6beb-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="f6beb-119">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="f6beb-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f6beb-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6beb-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f6beb-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="f6beb-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="f6beb-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6beb-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="f6beb-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6beb-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6beb-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6beb-124">Not supported.</span></span>|
|<span data-ttu-id="f6beb-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6beb-125">Application</span></span>|<span data-ttu-id="f6beb-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6beb-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6beb-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6beb-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6beb-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f6beb-128">Optional query parameters</span></span>

<span data-ttu-id="f6beb-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f6beb-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6beb-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6beb-130">Request headers</span></span>

|<span data-ttu-id="f6beb-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6beb-131">Header</span></span>|<span data-ttu-id="f6beb-132">Valor</span><span class="sxs-lookup"><span data-stu-id="f6beb-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6beb-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6beb-133">Authorization</span></span>|<span data-ttu-id="f6beb-134">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6beb-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6beb-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f6beb-135">Accept</span></span>|<span data-ttu-id="f6beb-136">application/json</span><span class="sxs-lookup"><span data-stu-id="f6beb-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6beb-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6beb-137">Request body</span></span>

<span data-ttu-id="f6beb-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f6beb-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6beb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6beb-139">Response</span></span>

<span data-ttu-id="f6beb-140">Se tiver êxito, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6beb-140">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6beb-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6beb-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6beb-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6beb-142">Request</span></span>

<span data-ttu-id="f6beb-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6beb-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="f6beb-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6beb-144">Response</span></span>

<span data-ttu-id="f6beb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6beb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



