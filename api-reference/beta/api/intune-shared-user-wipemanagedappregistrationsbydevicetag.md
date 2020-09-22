---
title: Ação wipeManagedAppRegistrationsByDeviceTag
description: Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0730e8414924f0b974796bec1d1c7c865c76a244
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004729"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="496d6-103">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="496d6-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

<span data-ttu-id="496d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="496d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="496d6-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="496d6-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="496d6-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="496d6-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="496d6-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="496d6-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="496d6-108">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="496d6-108">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="496d6-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="496d6-109">Prerequisites</span></span>

<span data-ttu-id="496d6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="496d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="496d6-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="496d6-112">Permission type</span></span>|<span data-ttu-id="496d6-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="496d6-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="496d6-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="496d6-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="496d6-115">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="496d6-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="496d6-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="496d6-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="496d6-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="496d6-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="496d6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="496d6-118">Not supported.</span></span>|
|<span data-ttu-id="496d6-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="496d6-119">Application</span></span>||
| <span data-ttu-id="496d6-120">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="496d6-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="496d6-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="496d6-121">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="496d6-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="496d6-122">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="496d6-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="496d6-123">Request headers</span></span>

|<span data-ttu-id="496d6-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="496d6-124">Header</span></span>|<span data-ttu-id="496d6-125">Valor</span><span class="sxs-lookup"><span data-stu-id="496d6-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="496d6-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="496d6-126">Authorization</span></span>|<span data-ttu-id="496d6-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="496d6-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="496d6-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="496d6-128">Accept</span></span>|<span data-ttu-id="496d6-129">application/json</span><span class="sxs-lookup"><span data-stu-id="496d6-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="496d6-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="496d6-130">Request body</span></span>

<span data-ttu-id="496d6-131">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="496d6-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="496d6-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="496d6-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="496d6-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="496d6-133">Property</span></span>|<span data-ttu-id="496d6-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="496d6-134">Type</span></span>|<span data-ttu-id="496d6-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="496d6-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="496d6-136">deviceTag</span><span class="sxs-lookup"><span data-stu-id="496d6-136">deviceTag</span></span>|<span data-ttu-id="496d6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="496d6-137">String</span></span>|<span data-ttu-id="496d6-138">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="496d6-138">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="496d6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="496d6-139">Response</span></span>

<span data-ttu-id="496d6-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="496d6-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="496d6-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="496d6-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="496d6-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="496d6-142">Request</span></span>

<span data-ttu-id="496d6-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="496d6-143">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="496d6-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="496d6-144">Response</span></span>

<span data-ttu-id="496d6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="496d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```















