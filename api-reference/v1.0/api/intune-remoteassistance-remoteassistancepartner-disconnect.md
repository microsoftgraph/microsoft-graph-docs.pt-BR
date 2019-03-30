---
title: Ação desconectar
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14105698ef39601b2c4b96df1163ae5439db9022
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967941"
---
# <a name="disconnect-action"></a><span data-ttu-id="8f6dc-103">Ação disconnect</span><span class="sxs-lookup"><span data-stu-id="8f6dc-103">disconnect action</span></span>

> <span data-ttu-id="8f6dc-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8f6dc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f6dc-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8f6dc-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f6dc-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8f6dc-106">Prerequisites</span></span>
<span data-ttu-id="8f6dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f6dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f6dc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f6dc-109">Permission type</span></span>|<span data-ttu-id="8f6dc-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8f6dc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f6dc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f6dc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8f6dc-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f6dc-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8f6dc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f6dc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f6dc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f6dc-114">Not supported.</span></span>|
|<span data-ttu-id="8f6dc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f6dc-115">Application</span></span>|<span data-ttu-id="8f6dc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f6dc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f6dc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f6dc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/disconnect
```

## <a name="request-headers"></a><span data-ttu-id="8f6dc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f6dc-118">Request headers</span></span>
|<span data-ttu-id="8f6dc-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f6dc-119">Header</span></span>|<span data-ttu-id="8f6dc-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8f6dc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f6dc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f6dc-121">Authorization</span></span>|<span data-ttu-id="8f6dc-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f6dc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f6dc-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8f6dc-123">Accept</span></span>|<span data-ttu-id="8f6dc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8f6dc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f6dc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f6dc-125">Request body</span></span>
<span data-ttu-id="8f6dc-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f6dc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f6dc-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f6dc-127">Response</span></span>
<span data-ttu-id="8f6dc-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8f6dc-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8f6dc-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f6dc-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f6dc-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f6dc-130">Request</span></span>
<span data-ttu-id="8f6dc-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f6dc-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/disconnect
```

### <a name="response"></a><span data-ttu-id="8f6dc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f6dc-132">Response</span></span>
<span data-ttu-id="8f6dc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f6dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



