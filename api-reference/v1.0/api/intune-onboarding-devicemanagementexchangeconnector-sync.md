---
title: ação sync
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cfb392b6849ac66ad163c5641ef0420b7e5dc52a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974686"
---
# <a name="sync-action"></a><span data-ttu-id="51a66-103">Ação sync</span><span class="sxs-lookup"><span data-stu-id="51a66-103">sync action</span></span>

> <span data-ttu-id="51a66-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51a66-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51a66-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="51a66-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51a66-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51a66-106">Prerequisites</span></span>
<span data-ttu-id="51a66-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51a66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51a66-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51a66-109">Permission type</span></span>|<span data-ttu-id="51a66-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51a66-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51a66-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51a66-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51a66-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51a66-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="51a66-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51a66-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51a66-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51a66-114">Not supported.</span></span>|
|<span data-ttu-id="51a66-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51a66-115">Application</span></span>|<span data-ttu-id="51a66-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51a66-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51a66-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51a66-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="51a66-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51a66-118">Request headers</span></span>
|<span data-ttu-id="51a66-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51a66-119">Header</span></span>|<span data-ttu-id="51a66-120">Valor</span><span class="sxs-lookup"><span data-stu-id="51a66-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51a66-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="51a66-121">Authorization</span></span>|<span data-ttu-id="51a66-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51a66-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51a66-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51a66-123">Accept</span></span>|<span data-ttu-id="51a66-124">application/json</span><span class="sxs-lookup"><span data-stu-id="51a66-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51a66-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51a66-125">Request body</span></span>
<span data-ttu-id="51a66-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="51a66-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="51a66-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="51a66-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="51a66-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51a66-128">Property</span></span>|<span data-ttu-id="51a66-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="51a66-129">Type</span></span>|<span data-ttu-id="51a66-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="51a66-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51a66-131">syncType</span><span class="sxs-lookup"><span data-stu-id="51a66-131">syncType</span></span>|[<span data-ttu-id="51a66-132">deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="51a66-132">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="51a66-133">O tipo de sincronização que será executado: sincronização completa ou sincronização delta.</span><span class="sxs-lookup"><span data-stu-id="51a66-133">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="51a66-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="51a66-134">Response</span></span>
<span data-ttu-id="51a66-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="51a66-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="51a66-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51a66-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="51a66-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51a66-137">Request</span></span>
<span data-ttu-id="51a66-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51a66-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="51a66-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="51a66-139">Response</span></span>
<span data-ttu-id="51a66-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51a66-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



