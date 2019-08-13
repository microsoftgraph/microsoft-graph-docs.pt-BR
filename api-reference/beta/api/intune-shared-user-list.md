---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bfa97f3dece44fd017e960f88cd778eb562d1bb0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350626"
---
# <a name="list-users"></a><span data-ttu-id="8840a-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="8840a-103">List users</span></span>

> <span data-ttu-id="8840a-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8840a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8840a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8840a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8840a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8840a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8840a-107">Listar propriedades e relações de objetos de [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="8840a-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8840a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8840a-108">Prerequisites</span></span>

<span data-ttu-id="8840a-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8840a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8840a-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8840a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="8840a-111">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="8840a-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="8840a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8840a-112">Permission type</span></span>|<span data-ttu-id="8840a-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8840a-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8840a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8840a-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8840a-115">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="8840a-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8840a-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8840a-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="8840a-117">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="8840a-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="8840a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8840a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="8840a-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="8840a-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="8840a-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8840a-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="8840a-121">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="8840a-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="8840a-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8840a-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="8840a-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8840a-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8840a-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8840a-124">Not supported.</span></span>|
|<span data-ttu-id="8840a-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8840a-125">Application</span></span>|<span data-ttu-id="8840a-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8840a-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8840a-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8840a-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="8840a-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8840a-128">Request headers</span></span>

|<span data-ttu-id="8840a-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8840a-129">Header</span></span>|<span data-ttu-id="8840a-130">Valor</span><span class="sxs-lookup"><span data-stu-id="8840a-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8840a-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="8840a-131">Authorization</span></span>|<span data-ttu-id="8840a-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8840a-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8840a-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8840a-133">Accept</span></span>|<span data-ttu-id="8840a-134">application/json</span><span class="sxs-lookup"><span data-stu-id="8840a-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8840a-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8840a-135">Request body</span></span>

<span data-ttu-id="8840a-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8840a-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8840a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8840a-137">Response</span></span>

<span data-ttu-id="8840a-138">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8840a-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8840a-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8840a-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="8840a-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8840a-140">Request</span></span>

<span data-ttu-id="8840a-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8840a-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="8840a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8840a-142">Response</span></span>

<span data-ttu-id="8840a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8840a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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






