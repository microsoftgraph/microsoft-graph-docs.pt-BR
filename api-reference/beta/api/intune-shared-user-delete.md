---
title: Excluir usuário
description: Exclui usuário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6d0afb6c816241acf15319c3fb4082d3cc7935dd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165489"
---
# <a name="delete-user"></a><span data-ttu-id="3e41b-103">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="3e41b-103">Delete user</span></span>

> <span data-ttu-id="3e41b-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3e41b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3e41b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3e41b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e41b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e41b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e41b-107">Exclui [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="3e41b-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e41b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3e41b-108">Prerequisites</span></span>
<span data-ttu-id="3e41b-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3e41b-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3e41b-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e41b-110">To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>  <span data-ttu-id="3e41b-111">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="3e41b-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="3e41b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e41b-112">Permission type</span></span>|<span data-ttu-id="3e41b-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3e41b-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e41b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e41b-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3e41b-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="3e41b-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="3e41b-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e41b-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="3e41b-117">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="3e41b-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3e41b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e41b-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="3e41b-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="3e41b-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="3e41b-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e41b-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="3e41b-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="3e41b-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="3e41b-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e41b-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3e41b-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e41b-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e41b-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e41b-124">Not supported.</span></span>|
|<span data-ttu-id="3e41b-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e41b-125">Application</span></span>|<span data-ttu-id="3e41b-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e41b-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e41b-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e41b-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="3e41b-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e41b-128">Request headers</span></span>

|<span data-ttu-id="3e41b-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3e41b-129">Header</span></span>|<span data-ttu-id="3e41b-130">Valor</span><span class="sxs-lookup"><span data-stu-id="3e41b-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e41b-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e41b-131">Authorization</span></span>|<span data-ttu-id="3e41b-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e41b-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e41b-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3e41b-133">Accept</span></span>|<span data-ttu-id="3e41b-134">application/json</span><span class="sxs-lookup"><span data-stu-id="3e41b-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e41b-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e41b-135">Request body</span></span>

<span data-ttu-id="3e41b-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e41b-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e41b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e41b-137">Response</span></span>

<span data-ttu-id="3e41b-138">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3e41b-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3e41b-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e41b-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e41b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e41b-140">Request</span></span>

<span data-ttu-id="3e41b-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e41b-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="3e41b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e41b-142">Response</span></span>

<span data-ttu-id="3e41b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e41b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



