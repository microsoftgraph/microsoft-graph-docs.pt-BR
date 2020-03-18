---
title: Excluir androidManagedAppProtection
description: Exclui androidManagedAppProtection.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58c802968a9fed2b1f93e4be8f1cda4562e28105
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801303"
---
# <a name="delete-androidmanagedappprotection"></a><span data-ttu-id="0d473-103">Excluir androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="0d473-103">Delete androidManagedAppProtection</span></span>

> <span data-ttu-id="0d473-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0d473-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d473-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0d473-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d473-106">Exclui [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0d473-106">Deletes a [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d473-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0d473-107">Prerequisites</span></span>
<span data-ttu-id="0d473-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d473-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d473-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d473-110">Permission type</span></span>|<span data-ttu-id="0d473-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0d473-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d473-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d473-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0d473-113">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="0d473-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="0d473-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d473-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="0d473-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="0d473-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="0d473-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d473-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0d473-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d473-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d473-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d473-118">Not supported.</span></span>|
|<span data-ttu-id="0d473-119">Application</span><span class="sxs-lookup"><span data-stu-id="0d473-119">Application</span></span>||
| <span data-ttu-id="0d473-120">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="0d473-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="0d473-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d473-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="0d473-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="0d473-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="0d473-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d473-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d473-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d473-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="0d473-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d473-125">Request headers</span></span>
|<span data-ttu-id="0d473-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0d473-126">Header</span></span>|<span data-ttu-id="0d473-127">Valor</span><span class="sxs-lookup"><span data-stu-id="0d473-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d473-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d473-128">Authorization</span></span>|<span data-ttu-id="0d473-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d473-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d473-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0d473-130">Accept</span></span>|<span data-ttu-id="0d473-131">application/json</span><span class="sxs-lookup"><span data-stu-id="0d473-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d473-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d473-132">Request body</span></span>
<span data-ttu-id="0d473-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d473-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d473-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d473-134">Response</span></span>
<span data-ttu-id="0d473-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0d473-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0d473-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d473-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d473-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d473-137">Request</span></span>
<span data-ttu-id="0d473-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d473-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="0d473-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d473-139">Response</span></span>
<span data-ttu-id="0d473-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d473-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







