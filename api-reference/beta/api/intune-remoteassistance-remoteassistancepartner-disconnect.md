---
title: Ação desconectar
description: Uma solicitação para remover o conector do TeamViewer ativo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b13d787ab2fdc3325838dfb48cf0e667cd2940b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49308218"
---
# <a name="disconnect-action"></a><span data-ttu-id="15238-103">Ação disconnect</span><span class="sxs-lookup"><span data-stu-id="15238-103">disconnect action</span></span>

<span data-ttu-id="15238-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15238-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15238-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="15238-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15238-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15238-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15238-107">Uma solicitação para remover o conector do TeamViewer ativo</span><span class="sxs-lookup"><span data-stu-id="15238-107">A request to remove the active TeamViewer connector</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15238-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15238-108">Prerequisites</span></span>
<span data-ttu-id="15238-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15238-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15238-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15238-111">Permission type</span></span>|<span data-ttu-id="15238-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15238-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15238-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15238-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15238-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15238-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="15238-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15238-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15238-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15238-116">Not supported.</span></span>|
|<span data-ttu-id="15238-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15238-117">Application</span></span>|<span data-ttu-id="15238-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15238-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15238-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15238-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/disconnect
```

## <a name="request-headers"></a><span data-ttu-id="15238-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15238-120">Request headers</span></span>
|<span data-ttu-id="15238-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15238-121">Header</span></span>|<span data-ttu-id="15238-122">Valor</span><span class="sxs-lookup"><span data-stu-id="15238-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15238-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="15238-123">Authorization</span></span>|<span data-ttu-id="15238-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15238-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15238-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15238-125">Accept</span></span>|<span data-ttu-id="15238-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15238-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15238-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15238-127">Request body</span></span>
<span data-ttu-id="15238-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15238-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15238-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="15238-129">Response</span></span>
<span data-ttu-id="15238-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="15238-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="15238-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15238-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="15238-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15238-132">Request</span></span>
<span data-ttu-id="15238-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15238-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/disconnect
```

### <a name="response"></a><span data-ttu-id="15238-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="15238-134">Response</span></span>
<span data-ttu-id="15238-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15238-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




