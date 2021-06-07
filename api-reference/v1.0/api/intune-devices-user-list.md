---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e160dcf921b76eeedc51999c65e03ab590fd73b5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752913"
---
# <a name="list-users"></a><span data-ttu-id="df3f6-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="df3f6-103">List users</span></span>

<span data-ttu-id="df3f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df3f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df3f6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df3f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df3f6-106">Listar propriedades e relações de objetos de [usuário](../resources/intune-devices-user.md).</span><span class="sxs-lookup"><span data-stu-id="df3f6-106">List properties and relationships of the [user](../resources/intune-devices-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df3f6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df3f6-107">Prerequisites</span></span>
<span data-ttu-id="df3f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df3f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df3f6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df3f6-110">Permission type</span></span>|<span data-ttu-id="df3f6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df3f6-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df3f6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df3f6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df3f6-113">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df3f6-113">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="df3f6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df3f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df3f6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df3f6-115">Not supported.</span></span>|
|<span data-ttu-id="df3f6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df3f6-116">Application</span></span>|<span data-ttu-id="df3f6-117">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df3f6-117">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df3f6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df3f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="df3f6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df3f6-119">Request headers</span></span>
|<span data-ttu-id="df3f6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df3f6-120">Header</span></span>|<span data-ttu-id="df3f6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="df3f6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df3f6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="df3f6-122">Authorization</span></span>|<span data-ttu-id="df3f6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df3f6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df3f6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df3f6-124">Accept</span></span>|<span data-ttu-id="df3f6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df3f6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df3f6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df3f6-126">Request body</span></span>
<span data-ttu-id="df3f6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df3f6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df3f6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="df3f6-128">Response</span></span>
<span data-ttu-id="df3f6-129">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-devices-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df3f6-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-devices-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df3f6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df3f6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="df3f6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df3f6-131">Request</span></span>
<span data-ttu-id="df3f6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df3f6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="df3f6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="df3f6-133">Response</span></span>
<span data-ttu-id="df3f6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df3f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




