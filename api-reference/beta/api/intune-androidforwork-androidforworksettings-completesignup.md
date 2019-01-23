---
title: Ação completeSignup
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 37ee45f218c56bb3a42553bbd9a79b04406d9c33
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394583"
---
# <a name="completesignup-action"></a><span data-ttu-id="c87fe-103">Ação completeSignup</span><span class="sxs-lookup"><span data-stu-id="c87fe-103">completeSignup action</span></span>

> <span data-ttu-id="c87fe-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c87fe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c87fe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c87fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c87fe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c87fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c87fe-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c87fe-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c87fe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c87fe-108">Prerequisites</span></span>
<span data-ttu-id="c87fe-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c87fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c87fe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c87fe-111">Permission type</span></span>|<span data-ttu-id="c87fe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c87fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c87fe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c87fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c87fe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87fe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c87fe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c87fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c87fe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c87fe-116">Not supported.</span></span>|
|<span data-ttu-id="c87fe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c87fe-117">Application</span></span>|<span data-ttu-id="c87fe-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c87fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c87fe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c87fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/completeSignup
```

## <a name="request-headers"></a><span data-ttu-id="c87fe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c87fe-120">Request headers</span></span>
|<span data-ttu-id="c87fe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c87fe-121">Header</span></span>|<span data-ttu-id="c87fe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c87fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c87fe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c87fe-123">Authorization</span></span>|<span data-ttu-id="c87fe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c87fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c87fe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c87fe-125">Accept</span></span>|<span data-ttu-id="c87fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c87fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c87fe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c87fe-127">Request body</span></span>
<span data-ttu-id="c87fe-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c87fe-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c87fe-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c87fe-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c87fe-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c87fe-130">Property</span></span>|<span data-ttu-id="c87fe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c87fe-131">Type</span></span>|<span data-ttu-id="c87fe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c87fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c87fe-133">enterpriseToken</span><span class="sxs-lookup"><span data-stu-id="c87fe-133">enterpriseToken</span></span>|<span data-ttu-id="c87fe-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c87fe-134">String</span></span>|<span data-ttu-id="c87fe-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c87fe-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c87fe-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c87fe-136">Response</span></span>
<span data-ttu-id="c87fe-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c87fe-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c87fe-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c87fe-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c87fe-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c87fe-139">Request</span></span>
<span data-ttu-id="c87fe-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c87fe-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/completeSignup

Content-type: application/json
Content-length: 51

{
  "enterpriseToken": "Enterprise Token value"
}
```

### <a name="response"></a><span data-ttu-id="c87fe-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c87fe-141">Response</span></span>
<span data-ttu-id="c87fe-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c87fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




