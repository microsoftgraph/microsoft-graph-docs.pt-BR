---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0fe1ab86e78e4bff46a6c9105048519a20c894a1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141234"
---
# <a name="list-users"></a><span data-ttu-id="06971-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="06971-103">List users</span></span>

> <span data-ttu-id="06971-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="06971-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="06971-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="06971-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06971-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06971-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06971-107">Listar propriedades e relações de objetos de [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="06971-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06971-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06971-108">Prerequisites</span></span>

<span data-ttu-id="06971-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="06971-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="06971-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06971-110">To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>  <span data-ttu-id="06971-111">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="06971-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="06971-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06971-112">Permission type</span></span>|<span data-ttu-id="06971-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06971-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06971-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06971-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="06971-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="06971-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="06971-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="06971-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="06971-117">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="06971-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="06971-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="06971-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="06971-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="06971-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="06971-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="06971-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="06971-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="06971-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="06971-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="06971-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="06971-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06971-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06971-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06971-124">Not supported.</span></span>|
|<span data-ttu-id="06971-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06971-125">Application</span></span>|<span data-ttu-id="06971-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06971-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06971-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06971-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="06971-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06971-128">Request headers</span></span>

|<span data-ttu-id="06971-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06971-129">Header</span></span>|<span data-ttu-id="06971-130">Valor</span><span class="sxs-lookup"><span data-stu-id="06971-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06971-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="06971-131">Authorization</span></span>|<span data-ttu-id="06971-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06971-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06971-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06971-133">Accept</span></span>|<span data-ttu-id="06971-134">application/json</span><span class="sxs-lookup"><span data-stu-id="06971-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06971-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06971-135">Request body</span></span>

<span data-ttu-id="06971-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06971-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06971-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="06971-137">Response</span></span>

<span data-ttu-id="06971-138">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06971-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06971-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06971-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="06971-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06971-140">Request</span></span>

<span data-ttu-id="06971-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06971-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="06971-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="06971-142">Response</span></span>

<span data-ttu-id="06971-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06971-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



