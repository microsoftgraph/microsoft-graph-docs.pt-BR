---
title: Excluir usuário
description: Exclui usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7e2faa54999dbca660ce8bd3df7d4449fa4fa5d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999752"
---
# <a name="delete-user"></a><span data-ttu-id="4173a-103">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="4173a-103">Delete user</span></span>

<span data-ttu-id="4173a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4173a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4173a-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4173a-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4173a-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4173a-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4173a-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4173a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4173a-108">Exclui [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="4173a-108">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4173a-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4173a-109">Prerequisites</span></span>
<span data-ttu-id="4173a-110">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4173a-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4173a-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4173a-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="4173a-112">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="4173a-112">The specific permission required depends on context.</span></span>

|<span data-ttu-id="4173a-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4173a-113">Permission type</span></span>|<span data-ttu-id="4173a-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4173a-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4173a-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4173a-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4173a-116">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4173a-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4173a-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4173a-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="4173a-118">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="4173a-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="4173a-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4173a-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="4173a-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="4173a-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4173a-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4173a-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="4173a-122">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="4173a-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="4173a-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4173a-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4173a-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4173a-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4173a-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4173a-125">Not supported.</span></span>|
|<span data-ttu-id="4173a-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4173a-126">Application</span></span>||
| <span data-ttu-id="4173a-127">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4173a-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4173a-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4173a-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="4173a-129">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="4173a-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="4173a-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4173a-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="4173a-131">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="4173a-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4173a-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4173a-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="4173a-133">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="4173a-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="4173a-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4173a-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4173a-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4173a-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="4173a-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4173a-136">Request headers</span></span>

|<span data-ttu-id="4173a-137">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4173a-137">Header</span></span>|<span data-ttu-id="4173a-138">Valor</span><span class="sxs-lookup"><span data-stu-id="4173a-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4173a-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="4173a-139">Authorization</span></span>|<span data-ttu-id="4173a-140">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4173a-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4173a-141">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4173a-141">Accept</span></span>|<span data-ttu-id="4173a-142">application/json</span><span class="sxs-lookup"><span data-stu-id="4173a-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4173a-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4173a-143">Request body</span></span>

<span data-ttu-id="4173a-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4173a-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4173a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="4173a-145">Response</span></span>

<span data-ttu-id="4173a-146">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4173a-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4173a-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4173a-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="4173a-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4173a-148">Request</span></span>

<span data-ttu-id="4173a-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4173a-149">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="4173a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="4173a-150">Response</span></span>

<span data-ttu-id="4173a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4173a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```












