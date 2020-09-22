---
title: Excluir iosManagedAppProtection
description: Exclui iosManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 25c661e4539b9cff4a38c751a03eb0db1161cd32
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031939"
---
# <a name="delete-iosmanagedappprotection"></a><span data-ttu-id="c263f-103">Excluir iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="c263f-103">Delete iosManagedAppProtection</span></span>

<span data-ttu-id="c263f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c263f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c263f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c263f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c263f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c263f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c263f-107">Exclui [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="c263f-107">Deletes a [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c263f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c263f-108">Prerequisites</span></span>
<span data-ttu-id="c263f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c263f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c263f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c263f-111">Permission type</span></span>|<span data-ttu-id="c263f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c263f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c263f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c263f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c263f-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="c263f-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="c263f-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c263f-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c263f-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="c263f-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c263f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c263f-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c263f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c263f-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c263f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c263f-119">Not supported.</span></span>|
|<span data-ttu-id="c263f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c263f-120">Application</span></span>||
| <span data-ttu-id="c263f-121">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="c263f-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="c263f-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c263f-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c263f-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="c263f-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c263f-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c263f-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c263f-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c263f-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="c263f-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c263f-126">Request headers</span></span>
|<span data-ttu-id="c263f-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c263f-127">Header</span></span>|<span data-ttu-id="c263f-128">Valor</span><span class="sxs-lookup"><span data-stu-id="c263f-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c263f-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="c263f-129">Authorization</span></span>|<span data-ttu-id="c263f-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c263f-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c263f-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c263f-131">Accept</span></span>|<span data-ttu-id="c263f-132">application/json</span><span class="sxs-lookup"><span data-stu-id="c263f-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c263f-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c263f-133">Request body</span></span>
<span data-ttu-id="c263f-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c263f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c263f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c263f-135">Response</span></span>
<span data-ttu-id="c263f-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c263f-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c263f-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c263f-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c263f-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c263f-138">Request</span></span>
<span data-ttu-id="c263f-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c263f-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="c263f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c263f-140">Response</span></span>
<span data-ttu-id="c263f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c263f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









