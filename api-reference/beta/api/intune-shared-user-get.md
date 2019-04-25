---
title: Obter usuário
description: Leia as propriedades e as relações do objeto user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7e6643fa2beccf83384c454451094473e7c80ac8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526815"
---
# <a name="get-user"></a><span data-ttu-id="063aa-103">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="063aa-103">Get user</span></span>

> <span data-ttu-id="063aa-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="063aa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="063aa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="063aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="063aa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="063aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="063aa-107">Leia as propriedades e as relações do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="063aa-107">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="063aa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="063aa-108">Prerequisites</span></span>

<span data-ttu-id="063aa-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="063aa-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="063aa-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="063aa-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="063aa-111">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="063aa-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="063aa-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="063aa-112">Permission type</span></span>|<span data-ttu-id="063aa-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="063aa-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="063aa-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="063aa-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="063aa-115">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="063aa-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="063aa-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="063aa-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="063aa-117">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="063aa-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="063aa-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="063aa-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="063aa-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="063aa-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="063aa-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="063aa-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="063aa-121">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="063aa-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="063aa-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="063aa-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="063aa-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="063aa-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="063aa-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="063aa-124">Not supported.</span></span>|
|<span data-ttu-id="063aa-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="063aa-125">Application</span></span>|<span data-ttu-id="063aa-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="063aa-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="063aa-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="063aa-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="063aa-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="063aa-128">Optional query parameters</span></span>

<span data-ttu-id="063aa-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="063aa-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="063aa-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="063aa-130">Request headers</span></span>

|<span data-ttu-id="063aa-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="063aa-131">Header</span></span>|<span data-ttu-id="063aa-132">Valor</span><span class="sxs-lookup"><span data-stu-id="063aa-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="063aa-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="063aa-133">Authorization</span></span>|<span data-ttu-id="063aa-134">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="063aa-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="063aa-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="063aa-135">Accept</span></span>|<span data-ttu-id="063aa-136">application/json</span><span class="sxs-lookup"><span data-stu-id="063aa-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="063aa-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="063aa-137">Request body</span></span>

<span data-ttu-id="063aa-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="063aa-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="063aa-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="063aa-139">Response</span></span>

<span data-ttu-id="063aa-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="063aa-140">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="063aa-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="063aa-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="063aa-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="063aa-142">Request</span></span>

<span data-ttu-id="063aa-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="063aa-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="063aa-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="063aa-144">Response</span></span>

<span data-ttu-id="063aa-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="063aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



