---
title: ação revokeLicenses
description: Revogar licenças associadas a um determinado appleVolumePurchaseProgramToken
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73d4f82899d3b7cda27e02418f2d140cea828834
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352270"
---
# <a name="revokelicenses-action"></a><span data-ttu-id="6dde1-103">ação revokeLicenses</span><span class="sxs-lookup"><span data-stu-id="6dde1-103">revokeLicenses action</span></span>

> <span data-ttu-id="6dde1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6dde1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dde1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6dde1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dde1-106">Revogar licenças associadas a um determinado appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="6dde1-106">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dde1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6dde1-107">Prerequisites</span></span>
<span data-ttu-id="6dde1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dde1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dde1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6dde1-110">Permission type</span></span>|<span data-ttu-id="6dde1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6dde1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dde1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6dde1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6dde1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dde1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6dde1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6dde1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dde1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6dde1-115">Not supported.</span></span>|
|<span data-ttu-id="6dde1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6dde1-116">Application</span></span>|<span data-ttu-id="6dde1-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dde1-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dde1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6dde1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses
```

## <a name="request-headers"></a><span data-ttu-id="6dde1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6dde1-119">Request headers</span></span>
|<span data-ttu-id="6dde1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6dde1-120">Header</span></span>|<span data-ttu-id="6dde1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6dde1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dde1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6dde1-122">Authorization</span></span>|<span data-ttu-id="6dde1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6dde1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dde1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6dde1-124">Accept</span></span>|<span data-ttu-id="6dde1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6dde1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dde1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6dde1-126">Request body</span></span>
<span data-ttu-id="6dde1-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6dde1-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6dde1-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="6dde1-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6dde1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6dde1-129">Property</span></span>|<span data-ttu-id="6dde1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dde1-130">Type</span></span>|<span data-ttu-id="6dde1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dde1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dde1-132">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="6dde1-132">notifyManagedDevices</span></span>|<span data-ttu-id="6dde1-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="6dde1-133">Boolean</span></span>|<span data-ttu-id="6dde1-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6dde1-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6dde1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dde1-135">Response</span></span>
<span data-ttu-id="6dde1-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6dde1-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6dde1-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6dde1-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dde1-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dde1-138">Request</span></span>
<span data-ttu-id="6dde1-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6dde1-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="6dde1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dde1-140">Response</span></span>
<span data-ttu-id="6dde1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6dde1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






