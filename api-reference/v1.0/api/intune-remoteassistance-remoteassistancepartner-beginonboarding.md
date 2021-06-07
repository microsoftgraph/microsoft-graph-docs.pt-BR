---
title: Ação beginOnboarding
description: Uma solicitação para iniciar a integração.  Deve estar juntamente com as informações apropriadas da conta do TeamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc4285513e9ea847bee5014aeab6e62afd8d6f17
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759034"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="9e146-104">Ação beginOnboarding</span><span class="sxs-lookup"><span data-stu-id="9e146-104">beginOnboarding action</span></span>

<span data-ttu-id="9e146-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e146-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e146-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e146-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e146-107">Uma solicitação para iniciar a integração.</span><span class="sxs-lookup"><span data-stu-id="9e146-107">A request to start onboarding.</span></span>  <span data-ttu-id="9e146-108">Deve estar juntamente com as informações apropriadas da conta do TeamViewer</span><span class="sxs-lookup"><span data-stu-id="9e146-108">Must be coupled with the appropriate TeamViewer account information</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e146-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e146-109">Prerequisites</span></span>
<span data-ttu-id="9e146-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e146-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e146-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e146-112">Permission type</span></span>|<span data-ttu-id="9e146-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e146-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e146-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e146-114">Delegated (work or school account)</span></span>|<span data-ttu-id="9e146-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e146-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9e146-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e146-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e146-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e146-117">Not supported.</span></span>|
|<span data-ttu-id="9e146-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e146-118">Application</span></span>|<span data-ttu-id="9e146-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e146-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e146-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e146-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="9e146-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e146-121">Request headers</span></span>
|<span data-ttu-id="9e146-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e146-122">Header</span></span>|<span data-ttu-id="9e146-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9e146-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e146-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e146-124">Authorization</span></span>|<span data-ttu-id="9e146-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e146-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e146-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e146-126">Accept</span></span>|<span data-ttu-id="9e146-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9e146-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e146-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e146-128">Request body</span></span>
<span data-ttu-id="9e146-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e146-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e146-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e146-130">Response</span></span>
<span data-ttu-id="9e146-131">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9e146-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9e146-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e146-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e146-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e146-133">Request</span></span>
<span data-ttu-id="9e146-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e146-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="9e146-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e146-135">Response</span></span>
<span data-ttu-id="9e146-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e146-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




