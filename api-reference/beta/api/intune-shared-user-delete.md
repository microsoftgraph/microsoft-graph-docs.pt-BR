---
title: Excluir usuário
description: Exclui usuário.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b4f6bc631b7a79253c8007305258fe96b821613
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939498"
---
# <a name="delete-user"></a><span data-ttu-id="14e6e-103">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="14e6e-103">Delete user</span></span>

> <span data-ttu-id="14e6e-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="14e6e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="14e6e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="14e6e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14e6e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14e6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14e6e-107">Exclui [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="14e6e-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="14e6e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14e6e-108">Prerequisites</span></span>
<span data-ttu-id="14e6e-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="14e6e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="14e6e-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14e6e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="14e6e-111">A permissão específica necessária depende do contexto.</span><span class="sxs-lookup"><span data-stu-id="14e6e-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="14e6e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14e6e-112">Permission type</span></span>|<span data-ttu-id="14e6e-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14e6e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14e6e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14e6e-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="14e6e-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="14e6e-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="14e6e-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14e6e-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="14e6e-117">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="14e6e-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="14e6e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14e6e-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="14e6e-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="14e6e-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="14e6e-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14e6e-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="14e6e-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="14e6e-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="14e6e-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14e6e-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="14e6e-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14e6e-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14e6e-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14e6e-124">Not supported.</span></span>|
|<span data-ttu-id="14e6e-125">Application</span><span class="sxs-lookup"><span data-stu-id="14e6e-125">Application</span></span>||
| <span data-ttu-id="14e6e-126">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="14e6e-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="14e6e-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14e6e-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="14e6e-128">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="14e6e-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="14e6e-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14e6e-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="14e6e-130">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="14e6e-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="14e6e-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14e6e-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="14e6e-132">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="14e6e-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="14e6e-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14e6e-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14e6e-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14e6e-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="14e6e-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14e6e-135">Request headers</span></span>

|<span data-ttu-id="14e6e-136">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14e6e-136">Header</span></span>|<span data-ttu-id="14e6e-137">Valor</span><span class="sxs-lookup"><span data-stu-id="14e6e-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14e6e-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="14e6e-138">Authorization</span></span>|<span data-ttu-id="14e6e-139">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14e6e-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14e6e-140">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14e6e-140">Accept</span></span>|<span data-ttu-id="14e6e-141">application/json</span><span class="sxs-lookup"><span data-stu-id="14e6e-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14e6e-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14e6e-142">Request body</span></span>

<span data-ttu-id="14e6e-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14e6e-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14e6e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="14e6e-144">Response</span></span>

<span data-ttu-id="14e6e-145">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="14e6e-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="14e6e-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14e6e-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="14e6e-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14e6e-147">Request</span></span>

<span data-ttu-id="14e6e-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14e6e-148">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="14e6e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="14e6e-149">Response</span></span>

<span data-ttu-id="14e6e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14e6e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```











