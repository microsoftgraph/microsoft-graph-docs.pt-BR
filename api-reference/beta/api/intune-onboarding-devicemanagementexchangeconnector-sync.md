---
title: ação sync
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6dd3d593078b306058d48eb4e4c119ff2f58f33f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49211744"
---
# <a name="sync-action"></a><span data-ttu-id="ebba3-103">Ação sync</span><span class="sxs-lookup"><span data-stu-id="ebba3-103">sync action</span></span>

<span data-ttu-id="ebba3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebba3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebba3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ebba3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebba3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebba3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebba3-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ebba3-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebba3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ebba3-108">Prerequisites</span></span>
<span data-ttu-id="ebba3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebba3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebba3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebba3-111">Permission type</span></span>|<span data-ttu-id="ebba3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ebba3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebba3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebba3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ebba3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebba3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ebba3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebba3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebba3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebba3-116">Not supported.</span></span>|
|<span data-ttu-id="ebba3-117">Application</span><span class="sxs-lookup"><span data-stu-id="ebba3-117">Application</span></span>|<span data-ttu-id="ebba3-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebba3-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebba3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebba3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="ebba3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebba3-120">Request headers</span></span>
|<span data-ttu-id="ebba3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebba3-121">Header</span></span>|<span data-ttu-id="ebba3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ebba3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebba3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebba3-123">Authorization</span></span>|<span data-ttu-id="ebba3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebba3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebba3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ebba3-125">Accept</span></span>|<span data-ttu-id="ebba3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebba3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebba3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebba3-127">Request body</span></span>
<span data-ttu-id="ebba3-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ebba3-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ebba3-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ebba3-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ebba3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebba3-130">Property</span></span>|<span data-ttu-id="ebba3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebba3-131">Type</span></span>|<span data-ttu-id="ebba3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebba3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebba3-133">syncType</span><span class="sxs-lookup"><span data-stu-id="ebba3-133">syncType</span></span>|[<span data-ttu-id="ebba3-134">deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="ebba3-134">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="ebba3-135">O tipo de sincronização que será executado: sincronização completa ou sincronização delta.</span><span class="sxs-lookup"><span data-stu-id="ebba3-135">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="ebba3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebba3-136">Response</span></span>
<span data-ttu-id="ebba3-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ebba3-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ebba3-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebba3-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebba3-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebba3-139">Request</span></span>
<span data-ttu-id="ebba3-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebba3-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="ebba3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebba3-141">Response</span></span>
<span data-ttu-id="ebba3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebba3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




