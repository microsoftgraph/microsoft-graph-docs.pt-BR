---
title: Excluir iosManagedAppProtection
description: Exclui iosManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 650c16cba55adeab5b03360dd2a1e6bf17092d69
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958624"
---
# <a name="delete-iosmanagedappprotection"></a><span data-ttu-id="535cd-103">Excluir iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="535cd-103">Delete iosManagedAppProtection</span></span>

> <span data-ttu-id="535cd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="535cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="535cd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="535cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="535cd-106">Exclui [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="535cd-106">Deletes a [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="535cd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="535cd-107">Prerequisites</span></span>
<span data-ttu-id="535cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="535cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="535cd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="535cd-110">Permission type</span></span>|<span data-ttu-id="535cd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="535cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="535cd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="535cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="535cd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="535cd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="535cd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="535cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="535cd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="535cd-115">Not supported.</span></span>|
|<span data-ttu-id="535cd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="535cd-116">Application</span></span>|<span data-ttu-id="535cd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="535cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="535cd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="535cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="535cd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="535cd-119">Request headers</span></span>
|<span data-ttu-id="535cd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="535cd-120">Header</span></span>|<span data-ttu-id="535cd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="535cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="535cd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="535cd-122">Authorization</span></span>|<span data-ttu-id="535cd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="535cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="535cd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="535cd-124">Accept</span></span>|<span data-ttu-id="535cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="535cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="535cd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="535cd-126">Request body</span></span>
<span data-ttu-id="535cd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="535cd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="535cd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="535cd-128">Response</span></span>
<span data-ttu-id="535cd-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="535cd-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="535cd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="535cd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="535cd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="535cd-131">Request</span></span>
<span data-ttu-id="535cd-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="535cd-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="535cd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="535cd-133">Response</span></span>
<span data-ttu-id="535cd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="535cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




