---
title: ação de desassociar
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b575d7be487dcda1e95d90987a7a7f1cfa626275
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402619"
---
# <a name="unbind-action"></a><span data-ttu-id="c9580-103">ação de desassociar</span><span class="sxs-lookup"><span data-stu-id="c9580-103">unbind action</span></span>

> <span data-ttu-id="c9580-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c9580-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c9580-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c9580-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9580-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c9580-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9580-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c9580-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9580-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c9580-108">Prerequisites</span></span>
<span data-ttu-id="c9580-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c9580-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c9580-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9580-111">Permission type</span></span>|<span data-ttu-id="c9580-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c9580-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9580-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9580-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9580-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9580-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9580-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9580-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9580-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9580-116">Not supported.</span></span>|
|<span data-ttu-id="c9580-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9580-117">Application</span></span>|<span data-ttu-id="c9580-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9580-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9580-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9580-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/unbind
```

## <a name="request-headers"></a><span data-ttu-id="c9580-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9580-120">Request headers</span></span>
|<span data-ttu-id="c9580-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9580-121">Header</span></span>|<span data-ttu-id="c9580-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c9580-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9580-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9580-123">Authorization</span></span>|<span data-ttu-id="c9580-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9580-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9580-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c9580-125">Accept</span></span>|<span data-ttu-id="c9580-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9580-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9580-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9580-127">Request body</span></span>
<span data-ttu-id="c9580-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9580-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9580-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9580-129">Response</span></span>
<span data-ttu-id="c9580-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c9580-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c9580-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9580-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9580-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9580-132">Request</span></span>
<span data-ttu-id="c9580-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9580-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/unbind
```

### <a name="response"></a><span data-ttu-id="c9580-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9580-134">Response</span></span>
<span data-ttu-id="c9580-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9580-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




