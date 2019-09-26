---
title: Excluir androidManagedAppProtection
description: Exclui androidManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f218e4d93cadeff484ff46ef0cbccbe52b31c36c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199477"
---
# <a name="delete-androidmanagedappprotection"></a><span data-ttu-id="b8193-103">Excluir androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="b8193-103">Delete androidManagedAppProtection</span></span>

> <span data-ttu-id="b8193-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8193-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8193-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8193-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8193-106">Exclui [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b8193-106">Deletes a [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8193-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8193-107">Prerequisites</span></span>
<span data-ttu-id="b8193-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8193-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8193-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8193-110">Permission type</span></span>|<span data-ttu-id="b8193-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8193-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8193-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8193-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b8193-113">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="b8193-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="b8193-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8193-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="b8193-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="b8193-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b8193-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8193-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b8193-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8193-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8193-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8193-118">Not supported.</span></span>|
|<span data-ttu-id="b8193-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8193-119">Application</span></span>||
| <span data-ttu-id="b8193-120">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="b8193-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="b8193-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8193-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="b8193-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="b8193-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b8193-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8193-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8193-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8193-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="b8193-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8193-125">Request headers</span></span>
|<span data-ttu-id="b8193-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8193-126">Header</span></span>|<span data-ttu-id="b8193-127">Valor</span><span class="sxs-lookup"><span data-stu-id="b8193-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8193-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8193-128">Authorization</span></span>|<span data-ttu-id="b8193-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8193-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8193-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8193-130">Accept</span></span>|<span data-ttu-id="b8193-131">application/json</span><span class="sxs-lookup"><span data-stu-id="b8193-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8193-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8193-132">Request body</span></span>
<span data-ttu-id="b8193-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8193-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8193-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8193-134">Response</span></span>
<span data-ttu-id="b8193-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b8193-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b8193-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8193-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8193-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8193-137">Request</span></span>
<span data-ttu-id="b8193-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8193-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="b8193-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8193-139">Response</span></span>
<span data-ttu-id="b8193-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8193-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




