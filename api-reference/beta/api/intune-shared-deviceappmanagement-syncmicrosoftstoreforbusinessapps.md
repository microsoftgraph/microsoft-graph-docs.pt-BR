---
title: Ação syncMicrosoftStoreForBusinessApps
description: Sincroniza a conta do Intune com o Microsoft Store For Business
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4071e90884edde1d1d3d6ad3740d736d2acedfd8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993687"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="9cbc3-103">Ação syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="9cbc3-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="9cbc3-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9cbc3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9cbc3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9cbc3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cbc3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9cbc3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cbc3-107">Sincroniza a conta do Intune com o Microsoft Store For Business</span><span class="sxs-lookup"><span data-stu-id="9cbc3-107">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9cbc3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9cbc3-108">Prerequisites</span></span>
<span data-ttu-id="9cbc3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cbc3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cbc3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cbc3-111">Permission type</span></span>|<span data-ttu-id="9cbc3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9cbc3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cbc3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cbc3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9cbc3-114">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="9cbc3-114">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="9cbc3-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cbc3-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9cbc3-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cbc3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cbc3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cbc3-117">Not supported.</span></span>|
|<span data-ttu-id="9cbc3-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cbc3-118">Application</span></span>|<span data-ttu-id="9cbc3-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cbc3-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cbc3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cbc3-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="9cbc3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cbc3-121">Request headers</span></span>
|<span data-ttu-id="9cbc3-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9cbc3-122">Header</span></span>|<span data-ttu-id="9cbc3-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9cbc3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cbc3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cbc3-124">Authorization</span></span>|<span data-ttu-id="9cbc3-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cbc3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cbc3-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9cbc3-126">Accept</span></span>|<span data-ttu-id="9cbc3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9cbc3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cbc3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cbc3-128">Request body</span></span>
<span data-ttu-id="9cbc3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9cbc3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cbc3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cbc3-130">Response</span></span>
<span data-ttu-id="9cbc3-131">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9cbc3-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9cbc3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cbc3-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="9cbc3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cbc3-133">Request</span></span>
<span data-ttu-id="9cbc3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cbc3-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="9cbc3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cbc3-135">Response</span></span>
<span data-ttu-id="9cbc3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cbc3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



