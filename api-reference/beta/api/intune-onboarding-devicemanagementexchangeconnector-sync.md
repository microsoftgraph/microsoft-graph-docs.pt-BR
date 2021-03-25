---
title: ação sync
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b349998eb1ece4fdb5544420d5ea29305c86519
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158756"
---
# <a name="sync-action"></a><span data-ttu-id="460cc-103">Ação sync</span><span class="sxs-lookup"><span data-stu-id="460cc-103">sync action</span></span>

<span data-ttu-id="460cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="460cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="460cc-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="460cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="460cc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="460cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="460cc-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="460cc-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="460cc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="460cc-108">Prerequisites</span></span>
<span data-ttu-id="460cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="460cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="460cc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="460cc-111">Permission type</span></span>|<span data-ttu-id="460cc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="460cc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="460cc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="460cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="460cc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="460cc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="460cc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="460cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="460cc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="460cc-116">Not supported.</span></span>|
|<span data-ttu-id="460cc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="460cc-117">Application</span></span>|<span data-ttu-id="460cc-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="460cc-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="460cc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="460cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="460cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="460cc-120">Request headers</span></span>
|<span data-ttu-id="460cc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="460cc-121">Header</span></span>|<span data-ttu-id="460cc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="460cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="460cc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="460cc-123">Authorization</span></span>|<span data-ttu-id="460cc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="460cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="460cc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="460cc-125">Accept</span></span>|<span data-ttu-id="460cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="460cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="460cc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="460cc-127">Request body</span></span>
<span data-ttu-id="460cc-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="460cc-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="460cc-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="460cc-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="460cc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="460cc-130">Property</span></span>|<span data-ttu-id="460cc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="460cc-131">Type</span></span>|<span data-ttu-id="460cc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="460cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="460cc-133">syncType</span><span class="sxs-lookup"><span data-stu-id="460cc-133">syncType</span></span>|[<span data-ttu-id="460cc-134">deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="460cc-134">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="460cc-135">O tipo de sincronização que será executado: sincronização completa ou sincronização delta.</span><span class="sxs-lookup"><span data-stu-id="460cc-135">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="460cc-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="460cc-136">Response</span></span>
<span data-ttu-id="460cc-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="460cc-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="460cc-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="460cc-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="460cc-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="460cc-139">Request</span></span>
<span data-ttu-id="460cc-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="460cc-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="460cc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="460cc-141">Response</span></span>
<span data-ttu-id="460cc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="460cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




