---
title: Ação wipeManagedAppRegistrationsByDeviceTag
description: Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e389eb6fb871cc1a6d827b25e40332066657383d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038477"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="1dbce-103">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="1dbce-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

<span data-ttu-id="1dbce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dbce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1dbce-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1dbce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dbce-106">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="1dbce-106">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dbce-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1dbce-107">Prerequisites</span></span>
<span data-ttu-id="1dbce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dbce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dbce-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dbce-110">Permission type</span></span>|<span data-ttu-id="1dbce-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1dbce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dbce-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dbce-112">Delegated (work or school account)</span></span>| <span data-ttu-id="1dbce-113">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="1dbce-113">_varies by context_</span></span> |
| <span data-ttu-id="1dbce-114">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="1dbce-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="1dbce-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dbce-115">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="1dbce-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dbce-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dbce-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dbce-117">Not supported.</span></span>|
|<span data-ttu-id="1dbce-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dbce-118">Application</span></span>|<span data-ttu-id="1dbce-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dbce-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dbce-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dbce-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="1dbce-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dbce-121">Request headers</span></span>
|<span data-ttu-id="1dbce-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1dbce-122">Header</span></span>|<span data-ttu-id="1dbce-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1dbce-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dbce-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dbce-124">Authorization</span></span>|<span data-ttu-id="1dbce-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dbce-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dbce-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1dbce-126">Accept</span></span>|<span data-ttu-id="1dbce-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1dbce-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dbce-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1dbce-128">Request body</span></span>
<span data-ttu-id="1dbce-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1dbce-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1dbce-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="1dbce-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1dbce-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1dbce-131">Property</span></span>|<span data-ttu-id="1dbce-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dbce-132">Type</span></span>|<span data-ttu-id="1dbce-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dbce-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dbce-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="1dbce-134">deviceTag</span></span>|<span data-ttu-id="1dbce-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dbce-135">String</span></span>|<span data-ttu-id="1dbce-136">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="1dbce-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="1dbce-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dbce-137">Response</span></span>
<span data-ttu-id="1dbce-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1dbce-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1dbce-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1dbce-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dbce-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dbce-140">Request</span></span>
<span data-ttu-id="1dbce-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dbce-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="1dbce-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dbce-142">Response</span></span>
<span data-ttu-id="1dbce-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1dbce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









