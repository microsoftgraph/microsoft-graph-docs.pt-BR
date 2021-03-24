---
title: Excluir vulnerableManagedDevice
description: Exclui um vulnerableManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 98abc4d6c40f724343a5b860c378298f7b08aec7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134729"
---
# <a name="delete-vulnerablemanageddevice"></a><span data-ttu-id="28a49-103">Excluir vulnerableManagedDevice</span><span class="sxs-lookup"><span data-stu-id="28a49-103">Delete vulnerableManagedDevice</span></span>

<span data-ttu-id="28a49-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28a49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28a49-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="28a49-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28a49-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28a49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28a49-107">Exclui um [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="28a49-107">Deletes a [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28a49-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="28a49-108">Prerequisites</span></span>
<span data-ttu-id="28a49-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28a49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28a49-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28a49-111">Permission type</span></span>|<span data-ttu-id="28a49-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28a49-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28a49-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28a49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28a49-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28a49-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="28a49-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28a49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28a49-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28a49-116">Not supported.</span></span>|
|<span data-ttu-id="28a49-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28a49-117">Application</span></span>|<span data-ttu-id="28a49-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28a49-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28a49-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28a49-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE ** Entity URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

## <a name="request-headers"></a><span data-ttu-id="28a49-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28a49-120">Request headers</span></span>
|<span data-ttu-id="28a49-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28a49-121">Header</span></span>|<span data-ttu-id="28a49-122">Valor</span><span class="sxs-lookup"><span data-stu-id="28a49-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28a49-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="28a49-123">Authorization</span></span>|<span data-ttu-id="28a49-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28a49-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28a49-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="28a49-125">Accept</span></span>|<span data-ttu-id="28a49-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28a49-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28a49-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28a49-127">Request body</span></span>
<span data-ttu-id="28a49-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28a49-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28a49-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="28a49-129">Response</span></span>
<span data-ttu-id="28a49-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="28a49-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="28a49-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28a49-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="28a49-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28a49-132">Request</span></span>
<span data-ttu-id="28a49-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28a49-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta** Entity URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

### <a name="response"></a><span data-ttu-id="28a49-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="28a49-134">Response</span></span>
<span data-ttu-id="28a49-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28a49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




