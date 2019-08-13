---
title: Ação wipeManagedAppRegistrationByDeviceTag
description: Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8085faaf612cb782fd4f82a2c33b77ed675ca6d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350584"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="f67ab-103">Ação wipeManagedAppRegistrationByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="f67ab-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

> <span data-ttu-id="f67ab-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f67ab-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f67ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f67ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f67ab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f67ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f67ab-107">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="f67ab-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f67ab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f67ab-108">Prerequisites</span></span>

<span data-ttu-id="f67ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f67ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f67ab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f67ab-111">Permission type</span></span>|<span data-ttu-id="f67ab-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f67ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f67ab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f67ab-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f67ab-114">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="f67ab-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="f67ab-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f67ab-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f67ab-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f67ab-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f67ab-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f67ab-117">Not supported.</span></span>|
|<span data-ttu-id="f67ab-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f67ab-118">Application</span></span>|<span data-ttu-id="f67ab-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f67ab-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f67ab-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f67ab-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="f67ab-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f67ab-121">Request headers</span></span>

|<span data-ttu-id="f67ab-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f67ab-122">Header</span></span>|<span data-ttu-id="f67ab-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f67ab-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f67ab-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f67ab-124">Authorization</span></span>|<span data-ttu-id="f67ab-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f67ab-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f67ab-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f67ab-126">Accept</span></span>|<span data-ttu-id="f67ab-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f67ab-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f67ab-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f67ab-128">Request body</span></span>

<span data-ttu-id="f67ab-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f67ab-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f67ab-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f67ab-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f67ab-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f67ab-131">Property</span></span>|<span data-ttu-id="f67ab-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f67ab-132">Type</span></span>|<span data-ttu-id="f67ab-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f67ab-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f67ab-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="f67ab-134">deviceTag</span></span>|<span data-ttu-id="f67ab-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f67ab-135">String</span></span>|<span data-ttu-id="f67ab-136">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="f67ab-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="f67ab-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f67ab-137">Response</span></span>

<span data-ttu-id="f67ab-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f67ab-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f67ab-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f67ab-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="f67ab-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f67ab-140">Request</span></span>

<span data-ttu-id="f67ab-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f67ab-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="f67ab-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f67ab-142">Response</span></span>

<span data-ttu-id="f67ab-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f67ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









