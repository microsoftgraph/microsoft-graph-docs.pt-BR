---
title: Ação wipeManagedAppRegistrationsByDeviceTag
description: Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 473c57670a026e538585e98338d202238428a1b3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411208"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="7f81e-103">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="7f81e-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

<span data-ttu-id="7f81e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f81e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f81e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f81e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f81e-106">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="7f81e-106">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f81e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7f81e-107">Prerequisites</span></span>
<span data-ttu-id="7f81e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f81e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f81e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f81e-110">Permission type</span></span>|<span data-ttu-id="7f81e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7f81e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f81e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f81e-112">Delegated (work or school account)</span></span>| <span data-ttu-id="7f81e-113">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="7f81e-113">_varies by context_</span></span> |
| <span data-ttu-id="7f81e-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="7f81e-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="7f81e-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f81e-115">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="7f81e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f81e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f81e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f81e-117">Not supported.</span></span>|
|<span data-ttu-id="7f81e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f81e-118">Application</span></span>|<span data-ttu-id="7f81e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f81e-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f81e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f81e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="7f81e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f81e-121">Request headers</span></span>
|<span data-ttu-id="7f81e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f81e-122">Header</span></span>|<span data-ttu-id="7f81e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7f81e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f81e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f81e-124">Authorization</span></span>|<span data-ttu-id="7f81e-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f81e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f81e-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7f81e-126">Accept</span></span>|<span data-ttu-id="7f81e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7f81e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f81e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f81e-128">Request body</span></span>
<span data-ttu-id="7f81e-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7f81e-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7f81e-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7f81e-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7f81e-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f81e-131">Property</span></span>|<span data-ttu-id="7f81e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f81e-132">Type</span></span>|<span data-ttu-id="7f81e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f81e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f81e-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="7f81e-134">deviceTag</span></span>|<span data-ttu-id="7f81e-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f81e-135">String</span></span>|<span data-ttu-id="7f81e-136">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="7f81e-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="7f81e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f81e-137">Response</span></span>
<span data-ttu-id="7f81e-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7f81e-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7f81e-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f81e-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f81e-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f81e-140">Request</span></span>
<span data-ttu-id="7f81e-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f81e-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="7f81e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f81e-142">Response</span></span>
<span data-ttu-id="7f81e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f81e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






