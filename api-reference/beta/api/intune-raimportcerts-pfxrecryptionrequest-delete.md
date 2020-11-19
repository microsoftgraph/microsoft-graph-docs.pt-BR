---
title: Excluir pfxRecryptionRequest
description: Exclui pfxRecryptionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a4a18752dd693f5a34575eda90938841498f64d3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49226920"
---
# <a name="delete-pfxrecryptionrequest"></a><span data-ttu-id="76908-103">Excluir pfxRecryptionRequest</span><span class="sxs-lookup"><span data-stu-id="76908-103">Delete pfxRecryptionRequest</span></span>

<span data-ttu-id="76908-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76908-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76908-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76908-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76908-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76908-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76908-107">Exclui [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="76908-107">Deletes a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76908-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76908-108">Prerequisites</span></span>
<span data-ttu-id="76908-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76908-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76908-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76908-111">Permission type</span></span>|<span data-ttu-id="76908-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="76908-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76908-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76908-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76908-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76908-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76908-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76908-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76908-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76908-116">Not supported.</span></span>|
|<span data-ttu-id="76908-117">Application</span><span class="sxs-lookup"><span data-stu-id="76908-117">Application</span></span>|<span data-ttu-id="76908-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76908-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76908-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76908-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

## <a name="request-headers"></a><span data-ttu-id="76908-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76908-120">Request headers</span></span>
|<span data-ttu-id="76908-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76908-121">Header</span></span>|<span data-ttu-id="76908-122">Valor</span><span class="sxs-lookup"><span data-stu-id="76908-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76908-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="76908-123">Authorization</span></span>|<span data-ttu-id="76908-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76908-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76908-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76908-125">Accept</span></span>|<span data-ttu-id="76908-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76908-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76908-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76908-127">Request body</span></span>
<span data-ttu-id="76908-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="76908-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76908-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="76908-129">Response</span></span>
<span data-ttu-id="76908-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="76908-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="76908-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76908-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="76908-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76908-132">Request</span></span>
<span data-ttu-id="76908-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76908-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

### <a name="response"></a><span data-ttu-id="76908-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="76908-134">Response</span></span>
<span data-ttu-id="76908-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76908-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




