---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d8602445eab740d18b2edf7036dd4b737d5be5a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537878"
---
# <a name="list-users"></a><span data-ttu-id="fc0f7-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="fc0f7-103">List users</span></span>

> <span data-ttu-id="fc0f7-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fc0f7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc0f7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc0f7-107">Listar propriedades e relações de objetos de [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="fc0f7-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc0f7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fc0f7-108">Prerequisites</span></span>

<span data-ttu-id="fc0f7-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fc0f7-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc0f7-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="fc0f7-111">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="fc0f7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc0f7-112">Permission type</span></span>|<span data-ttu-id="fc0f7-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fc0f7-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc0f7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc0f7-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fc0f7-115">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="fc0f7-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fc0f7-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc0f7-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="fc0f7-117">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="fc0f7-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="fc0f7-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc0f7-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="fc0f7-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="fc0f7-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="fc0f7-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc0f7-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="fc0f7-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="fc0f7-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="fc0f7-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc0f7-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="fc0f7-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc0f7-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc0f7-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-124">Not supported.</span></span>|
|<span data-ttu-id="fc0f7-125">Application</span><span class="sxs-lookup"><span data-stu-id="fc0f7-125">Application</span></span>||
| <span data-ttu-id="fc0f7-126">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="fc0f7-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fc0f7-127">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc0f7-127">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="fc0f7-128">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="fc0f7-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="fc0f7-129">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc0f7-129">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="fc0f7-130">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="fc0f7-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="fc0f7-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc0f7-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="fc0f7-132">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="fc0f7-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="fc0f7-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc0f7-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc0f7-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc0f7-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="fc0f7-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc0f7-135">Request headers</span></span>

|<span data-ttu-id="fc0f7-136">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc0f7-136">Header</span></span>|<span data-ttu-id="fc0f7-137">Valor</span><span class="sxs-lookup"><span data-stu-id="fc0f7-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc0f7-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc0f7-138">Authorization</span></span>|<span data-ttu-id="fc0f7-139">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc0f7-140">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fc0f7-140">Accept</span></span>|<span data-ttu-id="fc0f7-141">application/json</span><span class="sxs-lookup"><span data-stu-id="fc0f7-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc0f7-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc0f7-142">Request body</span></span>

<span data-ttu-id="fc0f7-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc0f7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc0f7-144">Response</span></span>

<span data-ttu-id="fc0f7-145">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-145">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc0f7-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc0f7-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc0f7-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc0f7-147">Request</span></span>

<span data-ttu-id="fc0f7-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-148">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="fc0f7-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc0f7-149">Response</span></span>

<span data-ttu-id="fc0f7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc0f7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









