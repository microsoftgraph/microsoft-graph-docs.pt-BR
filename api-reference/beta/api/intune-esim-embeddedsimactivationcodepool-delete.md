---
title: Excluir embeddedSIMActivationCodePool
description: Exclui um EMBEDDEDSIMActivationCodePool incorporado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 06cbd3f073ef43fdd098c91e98df4840ad505e85
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126168"
---
# <a name="delete-embeddedsimactivationcodepool"></a><span data-ttu-id="56aca-103">Excluir embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="56aca-103">Delete embeddedSIMActivationCodePool</span></span>

<span data-ttu-id="56aca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56aca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56aca-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="56aca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56aca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56aca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56aca-107">Exclui um [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span><span class="sxs-lookup"><span data-stu-id="56aca-107">Deletes a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56aca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56aca-108">Prerequisites</span></span>
<span data-ttu-id="56aca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56aca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56aca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56aca-111">Permission type</span></span>|<span data-ttu-id="56aca-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56aca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56aca-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56aca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56aca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56aca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56aca-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56aca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56aca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56aca-116">Not supported.</span></span>|
|<span data-ttu-id="56aca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56aca-117">Application</span></span>|<span data-ttu-id="56aca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56aca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56aca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56aca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="56aca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56aca-120">Request headers</span></span>
|<span data-ttu-id="56aca-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56aca-121">Header</span></span>|<span data-ttu-id="56aca-122">Valor</span><span class="sxs-lookup"><span data-stu-id="56aca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56aca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="56aca-123">Authorization</span></span>|<span data-ttu-id="56aca-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56aca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56aca-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="56aca-125">Accept</span></span>|<span data-ttu-id="56aca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56aca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56aca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56aca-127">Request body</span></span>
<span data-ttu-id="56aca-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56aca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56aca-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="56aca-129">Response</span></span>
<span data-ttu-id="56aca-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="56aca-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="56aca-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56aca-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="56aca-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56aca-132">Request</span></span>
<span data-ttu-id="56aca-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56aca-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

### <a name="response"></a><span data-ttu-id="56aca-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="56aca-134">Response</span></span>
<span data-ttu-id="56aca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56aca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




