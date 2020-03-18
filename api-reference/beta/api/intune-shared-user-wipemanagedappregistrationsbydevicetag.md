---
title: Ação wipeManagedAppRegistrationsByDeviceTag
description: Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 36e4b75e4868fa40003b5fdb58c0eb1fdd7b8566
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800505"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="3a153-103">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="3a153-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="3a153-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3a153-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3a153-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3a153-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a153-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a153-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a153-107">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="3a153-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a153-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3a153-108">Prerequisites</span></span>

<span data-ttu-id="3a153-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a153-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a153-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a153-111">Permission type</span></span>|<span data-ttu-id="3a153-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3a153-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a153-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a153-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3a153-114">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="3a153-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3a153-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a153-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3a153-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a153-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a153-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a153-117">Not supported.</span></span>|
|<span data-ttu-id="3a153-118">Application</span><span class="sxs-lookup"><span data-stu-id="3a153-118">Application</span></span>||
| <span data-ttu-id="3a153-119">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="3a153-119">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3a153-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a153-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a153-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a153-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="3a153-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a153-122">Request headers</span></span>

|<span data-ttu-id="3a153-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a153-123">Header</span></span>|<span data-ttu-id="3a153-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3a153-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a153-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a153-125">Authorization</span></span>|<span data-ttu-id="3a153-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a153-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a153-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3a153-127">Accept</span></span>|<span data-ttu-id="3a153-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3a153-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a153-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a153-129">Request body</span></span>

<span data-ttu-id="3a153-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3a153-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3a153-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3a153-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3a153-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a153-132">Property</span></span>|<span data-ttu-id="3a153-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a153-133">Type</span></span>|<span data-ttu-id="3a153-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a153-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a153-135">deviceTag</span><span class="sxs-lookup"><span data-stu-id="3a153-135">deviceTag</span></span>|<span data-ttu-id="3a153-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a153-136">String</span></span>|<span data-ttu-id="3a153-137">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="3a153-137">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="3a153-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a153-138">Response</span></span>

<span data-ttu-id="3a153-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3a153-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3a153-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a153-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a153-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a153-141">Request</span></span>

<span data-ttu-id="3a153-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a153-142">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="3a153-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a153-143">Response</span></span>

<span data-ttu-id="3a153-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a153-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```













