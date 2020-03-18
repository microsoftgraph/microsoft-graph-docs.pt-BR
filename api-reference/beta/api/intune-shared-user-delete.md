---
title: Excluir usuário
description: Exclui usuário.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 42bf2372deed17528b610ca719213ff2e282b9ac
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800589"
---
# <a name="delete-user"></a><span data-ttu-id="98402-103">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="98402-103">Delete user</span></span>

> <span data-ttu-id="98402-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="98402-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="98402-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="98402-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98402-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="98402-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98402-107">Exclui [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="98402-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="98402-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98402-108">Prerequisites</span></span>
<span data-ttu-id="98402-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="98402-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="98402-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98402-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="98402-111">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="98402-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="98402-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98402-112">Permission type</span></span>|<span data-ttu-id="98402-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98402-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98402-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98402-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="98402-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="98402-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="98402-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98402-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="98402-117">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="98402-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="98402-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98402-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="98402-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="98402-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="98402-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98402-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="98402-121">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="98402-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="98402-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98402-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="98402-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98402-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98402-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98402-124">Not supported.</span></span>|
|<span data-ttu-id="98402-125">Application</span><span class="sxs-lookup"><span data-stu-id="98402-125">Application</span></span>||
| <span data-ttu-id="98402-126">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="98402-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="98402-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98402-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="98402-128">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="98402-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="98402-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98402-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="98402-130">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="98402-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="98402-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98402-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="98402-132">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="98402-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="98402-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98402-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98402-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98402-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="98402-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98402-135">Request headers</span></span>

|<span data-ttu-id="98402-136">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98402-136">Header</span></span>|<span data-ttu-id="98402-137">Valor</span><span class="sxs-lookup"><span data-stu-id="98402-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98402-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="98402-138">Authorization</span></span>|<span data-ttu-id="98402-139">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98402-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98402-140">Aceitar</span><span class="sxs-lookup"><span data-stu-id="98402-140">Accept</span></span>|<span data-ttu-id="98402-141">application/json</span><span class="sxs-lookup"><span data-stu-id="98402-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98402-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98402-142">Request body</span></span>

<span data-ttu-id="98402-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="98402-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98402-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="98402-144">Response</span></span>

<span data-ttu-id="98402-145">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="98402-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="98402-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98402-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="98402-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98402-147">Request</span></span>

<span data-ttu-id="98402-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98402-148">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="98402-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="98402-149">Response</span></span>

<span data-ttu-id="98402-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98402-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```










