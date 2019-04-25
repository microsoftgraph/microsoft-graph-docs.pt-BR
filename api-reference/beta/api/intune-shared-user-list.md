---
title: Listar usuários
description: Listar propriedades e relações de objetos de usuário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2ebdc1842eb3530a0327326b2c06fa87eb92563a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526906"
---
# <a name="list-users"></a><span data-ttu-id="2b00b-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="2b00b-103">List users</span></span>

> <span data-ttu-id="2b00b-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2b00b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2b00b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2b00b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b00b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b00b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b00b-107">Listar propriedades e relações de objetos de [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="2b00b-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b00b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b00b-108">Prerequisites</span></span>

<span data-ttu-id="2b00b-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2b00b-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2b00b-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b00b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="2b00b-111">A permissão específica depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="2b00b-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="2b00b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b00b-112">Permission type</span></span>|<span data-ttu-id="2b00b-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2b00b-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b00b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b00b-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2b00b-115">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="2b00b-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2b00b-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b00b-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="2b00b-117">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="2b00b-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="2b00b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b00b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="2b00b-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="2b00b-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2b00b-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b00b-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="2b00b-121">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="2b00b-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="2b00b-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b00b-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="2b00b-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b00b-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b00b-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b00b-124">Not supported.</span></span>|
|<span data-ttu-id="2b00b-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b00b-125">Application</span></span>|<span data-ttu-id="2b00b-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b00b-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b00b-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b00b-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="2b00b-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b00b-128">Request headers</span></span>

|<span data-ttu-id="2b00b-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b00b-129">Header</span></span>|<span data-ttu-id="2b00b-130">Valor</span><span class="sxs-lookup"><span data-stu-id="2b00b-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b00b-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b00b-131">Authorization</span></span>|<span data-ttu-id="2b00b-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b00b-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b00b-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2b00b-133">Accept</span></span>|<span data-ttu-id="2b00b-134">application/json</span><span class="sxs-lookup"><span data-stu-id="2b00b-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b00b-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b00b-135">Request body</span></span>

<span data-ttu-id="2b00b-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b00b-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b00b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b00b-137">Response</span></span>

<span data-ttu-id="2b00b-138">Se tiver êxito, este método retornará o código de resposta `200 OK` e a coleção de objetos [user](../resources/intune-shared-user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b00b-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b00b-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b00b-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b00b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b00b-140">Request</span></span>

<span data-ttu-id="2b00b-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b00b-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="2b00b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b00b-142">Response</span></span>

<span data-ttu-id="2b00b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b00b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



