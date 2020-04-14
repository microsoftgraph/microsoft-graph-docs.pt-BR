---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9a06eff8418c16de11578a9a2da09dd7a0b5a873
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447466"
---
# <a name="list-users"></a><span data-ttu-id="e720e-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="e720e-103">List users</span></span>

<span data-ttu-id="e720e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e720e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e720e-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e720e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e720e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e720e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e720e-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e720e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e720e-108">Listar propriedades e relações de objetos de [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="e720e-108">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e720e-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e720e-109">Prerequisites</span></span>

<span data-ttu-id="e720e-110">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e720e-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e720e-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e720e-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="e720e-112">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="e720e-112">The specific permission depends on the context.</span></span>

|<span data-ttu-id="e720e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e720e-113">Permission type</span></span>|<span data-ttu-id="e720e-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e720e-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e720e-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e720e-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e720e-116">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="e720e-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e720e-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e720e-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="e720e-118">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="e720e-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="e720e-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e720e-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="e720e-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="e720e-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e720e-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e720e-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e720e-122">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="e720e-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e720e-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e720e-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="e720e-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e720e-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e720e-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e720e-125">Not supported.</span></span>|
|<span data-ttu-id="e720e-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e720e-126">Application</span></span>||
| <span data-ttu-id="e720e-127">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="e720e-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e720e-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e720e-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="e720e-129">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="e720e-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="e720e-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e720e-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="e720e-131">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="e720e-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e720e-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e720e-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e720e-133">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="e720e-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e720e-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e720e-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e720e-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e720e-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="e720e-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e720e-136">Request headers</span></span>

|<span data-ttu-id="e720e-137">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e720e-137">Header</span></span>|<span data-ttu-id="e720e-138">Valor</span><span class="sxs-lookup"><span data-stu-id="e720e-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e720e-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="e720e-139">Authorization</span></span>|<span data-ttu-id="e720e-140">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e720e-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e720e-141">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e720e-141">Accept</span></span>|<span data-ttu-id="e720e-142">application/json</span><span class="sxs-lookup"><span data-stu-id="e720e-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e720e-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e720e-143">Request body</span></span>

<span data-ttu-id="e720e-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e720e-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e720e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e720e-145">Response</span></span>

<span data-ttu-id="e720e-146">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e720e-146">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e720e-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e720e-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="e720e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e720e-148">Request</span></span>

<span data-ttu-id="e720e-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e720e-149">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="e720e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e720e-150">Response</span></span>

<span data-ttu-id="e720e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e720e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









