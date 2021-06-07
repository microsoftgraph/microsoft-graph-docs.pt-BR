---
title: Ação wipeManagedAppRegistrationsByDeviceTag
description: Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e389eb6fb871cc1a6d827b25e40332066657383d
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732304"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="16374-103">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="16374-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

<span data-ttu-id="16374-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16374-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16374-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16374-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16374-106">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="16374-106">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16374-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16374-107">Prerequisites</span></span>
<span data-ttu-id="16374-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16374-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16374-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16374-110">Permission type</span></span>|<span data-ttu-id="16374-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16374-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16374-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16374-112">Delegated (work or school account)</span></span>| <span data-ttu-id="16374-113">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="16374-113">_varies by context_</span></span> |
| <span data-ttu-id="16374-114">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="16374-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="16374-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16374-115">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="16374-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16374-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16374-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16374-117">Not supported.</span></span>|
|<span data-ttu-id="16374-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16374-118">Application</span></span>|<span data-ttu-id="16374-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16374-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16374-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16374-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="16374-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16374-121">Request headers</span></span>
|<span data-ttu-id="16374-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16374-122">Header</span></span>|<span data-ttu-id="16374-123">Valor</span><span class="sxs-lookup"><span data-stu-id="16374-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16374-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="16374-124">Authorization</span></span>|<span data-ttu-id="16374-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16374-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16374-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16374-126">Accept</span></span>|<span data-ttu-id="16374-127">application/json</span><span class="sxs-lookup"><span data-stu-id="16374-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16374-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16374-128">Request body</span></span>
<span data-ttu-id="16374-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="16374-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="16374-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="16374-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="16374-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16374-131">Property</span></span>|<span data-ttu-id="16374-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="16374-132">Type</span></span>|<span data-ttu-id="16374-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="16374-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16374-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="16374-134">deviceTag</span></span>|<span data-ttu-id="16374-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16374-135">String</span></span>|<span data-ttu-id="16374-136">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="16374-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="16374-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="16374-137">Response</span></span>
<span data-ttu-id="16374-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="16374-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="16374-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16374-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="16374-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16374-140">Request</span></span>
<span data-ttu-id="16374-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16374-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="16374-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="16374-142">Response</span></span>
<span data-ttu-id="16374-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16374-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









