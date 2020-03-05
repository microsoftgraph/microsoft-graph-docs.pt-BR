---
title: Ação wipeManagedAppRegistrationByDeviceTag
description: Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 25ed60b6965fe9b03e87bbd09ee1aeea27ec7ba3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457997"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="7514d-103">Ação wipeManagedAppRegistrationByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="7514d-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

<span data-ttu-id="7514d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7514d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7514d-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7514d-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7514d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7514d-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7514d-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7514d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7514d-108">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="7514d-108">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7514d-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7514d-109">Prerequisites</span></span>

<span data-ttu-id="7514d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7514d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7514d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7514d-112">Permission type</span></span>|<span data-ttu-id="7514d-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7514d-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7514d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7514d-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7514d-115">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="7514d-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="7514d-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7514d-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7514d-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7514d-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7514d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7514d-118">Not supported.</span></span>|
|<span data-ttu-id="7514d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7514d-119">Application</span></span>||
| <span data-ttu-id="7514d-120">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="7514d-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="7514d-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7514d-121">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7514d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7514d-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="7514d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7514d-123">Request headers</span></span>

|<span data-ttu-id="7514d-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7514d-124">Header</span></span>|<span data-ttu-id="7514d-125">Valor</span><span class="sxs-lookup"><span data-stu-id="7514d-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7514d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7514d-126">Authorization</span></span>|<span data-ttu-id="7514d-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7514d-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7514d-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7514d-128">Accept</span></span>|<span data-ttu-id="7514d-129">application/json</span><span class="sxs-lookup"><span data-stu-id="7514d-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7514d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7514d-130">Request body</span></span>

<span data-ttu-id="7514d-131">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7514d-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7514d-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7514d-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7514d-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7514d-133">Property</span></span>|<span data-ttu-id="7514d-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="7514d-134">Type</span></span>|<span data-ttu-id="7514d-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="7514d-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7514d-136">deviceTag</span><span class="sxs-lookup"><span data-stu-id="7514d-136">deviceTag</span></span>|<span data-ttu-id="7514d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7514d-137">String</span></span>|<span data-ttu-id="7514d-138">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="7514d-138">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="7514d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7514d-139">Response</span></span>

<span data-ttu-id="7514d-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7514d-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7514d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7514d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="7514d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7514d-142">Request</span></span>

<span data-ttu-id="7514d-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7514d-143">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="7514d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7514d-144">Response</span></span>

<span data-ttu-id="7514d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7514d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```














