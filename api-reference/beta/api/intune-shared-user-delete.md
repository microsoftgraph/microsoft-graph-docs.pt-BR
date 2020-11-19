---
title: Excluir usuário
description: Exclui usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 669b35665fa0cf4449a12cb8af2e1bbc753ec6de
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49232204"
---
# <a name="delete-user"></a><span data-ttu-id="47093-103">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="47093-103">Delete user</span></span>

<span data-ttu-id="47093-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47093-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47093-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="47093-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="47093-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="47093-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47093-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47093-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47093-108">Exclui [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="47093-108">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47093-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47093-109">Prerequisites</span></span>
<span data-ttu-id="47093-110">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="47093-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="47093-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47093-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="47093-112">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="47093-112">The specific permission required depends on context.</span></span>

|<span data-ttu-id="47093-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47093-113">Permission type</span></span>|<span data-ttu-id="47093-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47093-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47093-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47093-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="47093-116">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="47093-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="47093-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47093-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="47093-118">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="47093-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="47093-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47093-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="47093-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="47093-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="47093-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47093-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="47093-122">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="47093-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="47093-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47093-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="47093-124">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47093-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47093-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47093-125">Not supported.</span></span>|
|<span data-ttu-id="47093-126">Application</span><span class="sxs-lookup"><span data-stu-id="47093-126">Application</span></span>||
| <span data-ttu-id="47093-127">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="47093-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="47093-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47093-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="47093-129">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="47093-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="47093-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47093-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="47093-131">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="47093-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="47093-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47093-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="47093-133">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="47093-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="47093-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47093-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47093-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47093-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="47093-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47093-136">Request headers</span></span>

|<span data-ttu-id="47093-137">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47093-137">Header</span></span>|<span data-ttu-id="47093-138">Valor</span><span class="sxs-lookup"><span data-stu-id="47093-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47093-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="47093-139">Authorization</span></span>|<span data-ttu-id="47093-140">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47093-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47093-141">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47093-141">Accept</span></span>|<span data-ttu-id="47093-142">application/json</span><span class="sxs-lookup"><span data-stu-id="47093-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47093-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47093-143">Request body</span></span>

<span data-ttu-id="47093-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47093-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47093-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="47093-145">Response</span></span>

<span data-ttu-id="47093-146">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="47093-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="47093-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47093-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="47093-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47093-148">Request</span></span>

<span data-ttu-id="47093-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47093-149">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="47093-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="47093-150">Response</span></span>

<span data-ttu-id="47093-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47093-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```










