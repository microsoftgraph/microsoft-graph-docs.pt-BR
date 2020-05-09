---
title: Excluir remoteAssistancePartner
description: Exclui remoteAssistancePartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e56f255e0f7e51510502bbc66d1c06a203df830
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177734"
---
# <a name="delete-remoteassistancepartner"></a><span data-ttu-id="b8314-103">Excluir remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="b8314-103">Delete remoteAssistancePartner</span></span>

<span data-ttu-id="b8314-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8314-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8314-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8314-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8314-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8314-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8314-107">Exclui [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="b8314-107">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8314-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8314-108">Prerequisites</span></span>
<span data-ttu-id="b8314-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8314-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8314-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8314-111">Permission type</span></span>|<span data-ttu-id="b8314-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8314-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8314-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8314-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8314-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8314-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b8314-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8314-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8314-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8314-116">Not supported.</span></span>|
|<span data-ttu-id="b8314-117">Application</span><span class="sxs-lookup"><span data-stu-id="b8314-117">Application</span></span>|<span data-ttu-id="b8314-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8314-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8314-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8314-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="b8314-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8314-120">Request headers</span></span>
|<span data-ttu-id="b8314-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8314-121">Header</span></span>|<span data-ttu-id="b8314-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b8314-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8314-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8314-123">Authorization</span></span>|<span data-ttu-id="b8314-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8314-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8314-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8314-125">Accept</span></span>|<span data-ttu-id="b8314-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8314-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8314-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8314-127">Request body</span></span>
<span data-ttu-id="b8314-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8314-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8314-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8314-129">Response</span></span>
<span data-ttu-id="b8314-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b8314-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b8314-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8314-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8314-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8314-132">Request</span></span>
<span data-ttu-id="b8314-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8314-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

### <a name="response"></a><span data-ttu-id="b8314-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8314-134">Response</span></span>
<span data-ttu-id="b8314-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8314-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



