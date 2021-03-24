---
title: Ação beginOnboarding
description: Uma solicitação para iniciar a integração.  Deve estar juntamente com as informações apropriadas da conta do TeamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d4ffc6dc5ded86e7007c3a3b87fdd2007c792eab
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134463"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="b677b-104">Ação beginOnboarding</span><span class="sxs-lookup"><span data-stu-id="b677b-104">beginOnboarding action</span></span>

<span data-ttu-id="b677b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b677b-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b677b-106">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b677b-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b677b-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b677b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b677b-108">Uma solicitação para iniciar a integração.</span><span class="sxs-lookup"><span data-stu-id="b677b-108">A request to start onboarding.</span></span>  <span data-ttu-id="b677b-109">Deve estar juntamente com as informações apropriadas da conta do TeamViewer</span><span class="sxs-lookup"><span data-stu-id="b677b-109">Must be coupled with the appropriate TeamViewer account information</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b677b-110">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b677b-110">Prerequisites</span></span>
<span data-ttu-id="b677b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b677b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b677b-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b677b-113">Permission type</span></span>|<span data-ttu-id="b677b-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b677b-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b677b-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b677b-115">Delegated (work or school account)</span></span>|<span data-ttu-id="b677b-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b677b-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b677b-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b677b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b677b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b677b-118">Not supported.</span></span>|
|<span data-ttu-id="b677b-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b677b-119">Application</span></span>|<span data-ttu-id="b677b-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b677b-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b677b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b677b-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="b677b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b677b-122">Request headers</span></span>
|<span data-ttu-id="b677b-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b677b-123">Header</span></span>|<span data-ttu-id="b677b-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b677b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b677b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b677b-125">Authorization</span></span>|<span data-ttu-id="b677b-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b677b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b677b-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b677b-127">Accept</span></span>|<span data-ttu-id="b677b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b677b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b677b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b677b-129">Request body</span></span>
<span data-ttu-id="b677b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b677b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b677b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b677b-131">Response</span></span>
<span data-ttu-id="b677b-132">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b677b-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b677b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b677b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b677b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b677b-134">Request</span></span>
<span data-ttu-id="b677b-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b677b-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="b677b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b677b-136">Response</span></span>
<span data-ttu-id="b677b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b677b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




