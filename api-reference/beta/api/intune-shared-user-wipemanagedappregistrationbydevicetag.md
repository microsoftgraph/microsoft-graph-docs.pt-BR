---
title: Ação wipeManagedAppRegistrationByDeviceTag
description: Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e65a82c3ae10f182b68bd3cac038682c42bc5dbf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447413"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="df043-103">Ação wipeManagedAppRegistrationByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="df043-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

<span data-ttu-id="df043-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df043-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df043-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="df043-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="df043-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="df043-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df043-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df043-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df043-108">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="df043-108">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df043-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df043-109">Prerequisites</span></span>

<span data-ttu-id="df043-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df043-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df043-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df043-112">Permission type</span></span>|<span data-ttu-id="df043-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df043-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df043-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df043-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="df043-115">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="df043-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="df043-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df043-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="df043-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df043-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df043-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df043-118">Not supported.</span></span>|
|<span data-ttu-id="df043-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df043-119">Application</span></span>||
| <span data-ttu-id="df043-120">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="df043-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="df043-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df043-121">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df043-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df043-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="df043-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df043-123">Request headers</span></span>

|<span data-ttu-id="df043-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df043-124">Header</span></span>|<span data-ttu-id="df043-125">Valor</span><span class="sxs-lookup"><span data-stu-id="df043-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df043-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="df043-126">Authorization</span></span>|<span data-ttu-id="df043-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df043-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df043-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df043-128">Accept</span></span>|<span data-ttu-id="df043-129">application/json</span><span class="sxs-lookup"><span data-stu-id="df043-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df043-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df043-130">Request body</span></span>

<span data-ttu-id="df043-131">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="df043-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="df043-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="df043-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="df043-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df043-133">Property</span></span>|<span data-ttu-id="df043-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="df043-134">Type</span></span>|<span data-ttu-id="df043-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="df043-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df043-136">deviceTag</span><span class="sxs-lookup"><span data-stu-id="df043-136">deviceTag</span></span>|<span data-ttu-id="df043-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df043-137">String</span></span>|<span data-ttu-id="df043-138">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="df043-138">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="df043-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="df043-139">Response</span></span>

<span data-ttu-id="df043-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="df043-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df043-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df043-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="df043-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df043-142">Request</span></span>

<span data-ttu-id="df043-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df043-143">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="df043-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="df043-144">Response</span></span>

<span data-ttu-id="df043-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df043-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```












