---
title: Excluir usuário
description: Exclui usuário.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0822d3e0e3e720ae1f80510dca1d904f64443978
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194373"
---
# <a name="delete-user"></a><span data-ttu-id="7e73b-103">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="7e73b-103">Delete user</span></span>

> <span data-ttu-id="7e73b-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7e73b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7e73b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7e73b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e73b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7e73b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e73b-107">Exclui [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="7e73b-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e73b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7e73b-108">Prerequisites</span></span>
<span data-ttu-id="7e73b-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7e73b-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7e73b-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e73b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="7e73b-111">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="7e73b-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="7e73b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e73b-112">Permission type</span></span>|<span data-ttu-id="7e73b-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7e73b-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e73b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e73b-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7e73b-115">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="7e73b-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="7e73b-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e73b-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="7e73b-117">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="7e73b-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="7e73b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e73b-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="7e73b-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="7e73b-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7e73b-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e73b-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="7e73b-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="7e73b-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="7e73b-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e73b-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7e73b-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e73b-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e73b-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e73b-124">Not supported.</span></span>|
|<span data-ttu-id="7e73b-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e73b-125">Application</span></span>||
| <span data-ttu-id="7e73b-126">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="7e73b-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="7e73b-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e73b-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="7e73b-128">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="7e73b-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="7e73b-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e73b-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="7e73b-130">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="7e73b-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7e73b-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e73b-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="7e73b-132">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="7e73b-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="7e73b-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e73b-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e73b-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e73b-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="7e73b-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e73b-135">Request headers</span></span>

|<span data-ttu-id="7e73b-136">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e73b-136">Header</span></span>|<span data-ttu-id="7e73b-137">Valor</span><span class="sxs-lookup"><span data-stu-id="7e73b-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e73b-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e73b-138">Authorization</span></span>|<span data-ttu-id="7e73b-139">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e73b-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e73b-140">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7e73b-140">Accept</span></span>|<span data-ttu-id="7e73b-141">application/json</span><span class="sxs-lookup"><span data-stu-id="7e73b-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e73b-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e73b-142">Request body</span></span>

<span data-ttu-id="7e73b-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e73b-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e73b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e73b-144">Response</span></span>

<span data-ttu-id="7e73b-145">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7e73b-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7e73b-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e73b-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e73b-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e73b-147">Request</span></span>

<span data-ttu-id="7e73b-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e73b-148">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="7e73b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e73b-149">Response</span></span>

<span data-ttu-id="7e73b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e73b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```







