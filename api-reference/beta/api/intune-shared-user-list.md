---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e72ab04776bdf56c7e4896c5f94d8f97481ff446
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702907"
---
# <a name="list-users"></a><span data-ttu-id="e8072-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="e8072-103">List users</span></span>

<span data-ttu-id="e8072-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8072-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8072-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e8072-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e8072-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e8072-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8072-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8072-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8072-108">Listar propriedades e relações de objetos de [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="e8072-108">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8072-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8072-109">Prerequisites</span></span>

<span data-ttu-id="e8072-110">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e8072-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e8072-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8072-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="e8072-112">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="e8072-112">The specific permission depends on the context.</span></span>

|<span data-ttu-id="e8072-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8072-113">Permission type</span></span>|<span data-ttu-id="e8072-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8072-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8072-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8072-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e8072-116">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="e8072-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e8072-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8072-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="e8072-118">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="e8072-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="e8072-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8072-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="e8072-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="e8072-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e8072-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8072-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e8072-122">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="e8072-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e8072-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8072-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="e8072-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8072-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8072-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8072-125">Not supported.</span></span>|
|<span data-ttu-id="e8072-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8072-126">Application</span></span>||
| <span data-ttu-id="e8072-127">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="e8072-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e8072-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8072-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="e8072-129">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="e8072-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="e8072-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8072-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="e8072-131">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="e8072-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e8072-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8072-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e8072-133">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="e8072-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e8072-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8072-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8072-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8072-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="e8072-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8072-136">Request headers</span></span>

|<span data-ttu-id="e8072-137">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8072-137">Header</span></span>|<span data-ttu-id="e8072-138">Valor</span><span class="sxs-lookup"><span data-stu-id="e8072-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8072-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8072-139">Authorization</span></span>|<span data-ttu-id="e8072-140">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8072-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8072-141">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8072-141">Accept</span></span>|<span data-ttu-id="e8072-142">application/json</span><span class="sxs-lookup"><span data-stu-id="e8072-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8072-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8072-143">Request body</span></span>

<span data-ttu-id="e8072-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8072-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8072-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8072-145">Response</span></span>

<span data-ttu-id="e8072-146">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8072-146">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8072-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8072-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8072-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8072-148">Request</span></span>

<span data-ttu-id="e8072-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8072-149">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="e8072-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8072-150">Response</span></span>

<span data-ttu-id="e8072-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8072-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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











