---
title: Obter usuário
description: Leia as propriedades e as relações do objeto user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 66cb634de90c65bb6ca6b020c97373c57a446b21
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865660"
---
# <a name="get-user"></a><span data-ttu-id="5f8d8-103">Obter usuário</span><span class="sxs-lookup"><span data-stu-id="5f8d8-103">Get user</span></span>

<span data-ttu-id="5f8d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f8d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f8d8-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5f8d8-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5f8d8-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5f8d8-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f8d8-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f8d8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f8d8-108">Leia as propriedades e as relações do objeto [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="5f8d8-108">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f8d8-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5f8d8-109">Prerequisites</span></span>

<span data-ttu-id="5f8d8-110">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5f8d8-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5f8d8-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f8d8-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="5f8d8-112">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="5f8d8-112">The specific permission depends on the context.</span></span>

|<span data-ttu-id="5f8d8-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f8d8-113">Permission type</span></span>|<span data-ttu-id="5f8d8-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5f8d8-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f8d8-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f8d8-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5f8d8-116">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="5f8d8-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5f8d8-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f8d8-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="5f8d8-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="5f8d8-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="5f8d8-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f8d8-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="5f8d8-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="5f8d8-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5f8d8-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f8d8-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5f8d8-122">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="5f8d8-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="5f8d8-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f8d8-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="5f8d8-124">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f8d8-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f8d8-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f8d8-125">Not supported.</span></span>|
|<span data-ttu-id="5f8d8-126">Application</span><span class="sxs-lookup"><span data-stu-id="5f8d8-126">Application</span></span>||
| <span data-ttu-id="5f8d8-127">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="5f8d8-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5f8d8-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f8d8-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="5f8d8-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="5f8d8-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="5f8d8-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f8d8-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="5f8d8-131">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="5f8d8-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5f8d8-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f8d8-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="5f8d8-133">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="5f8d8-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="5f8d8-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f8d8-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f8d8-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f8d8-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f8d8-136">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5f8d8-136">Optional query parameters</span></span>

<span data-ttu-id="5f8d8-137">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5f8d8-137">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f8d8-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f8d8-138">Request headers</span></span>

|<span data-ttu-id="5f8d8-139">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f8d8-139">Header</span></span>|<span data-ttu-id="5f8d8-140">Valor</span><span class="sxs-lookup"><span data-stu-id="5f8d8-140">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f8d8-141">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f8d8-141">Authorization</span></span>|<span data-ttu-id="5f8d8-142">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f8d8-142">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f8d8-143">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5f8d8-143">Accept</span></span>|<span data-ttu-id="5f8d8-144">application/json</span><span class="sxs-lookup"><span data-stu-id="5f8d8-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f8d8-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f8d8-145">Request body</span></span>

<span data-ttu-id="5f8d8-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f8d8-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f8d8-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f8d8-147">Response</span></span>

<span data-ttu-id="5f8d8-148">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f8d8-148">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f8d8-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f8d8-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f8d8-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f8d8-150">Request</span></span>

<span data-ttu-id="5f8d8-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f8d8-151">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="5f8d8-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f8d8-152">Response</span></span>

<span data-ttu-id="5f8d8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f8d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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










