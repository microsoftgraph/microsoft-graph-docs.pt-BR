---
title: Ação wipeManagedAppRegistrationByDeviceTag
description: Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ef01d77a36224a9cf4d680c5cc1abfda4af5a9b1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157054"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="0c191-103">Ação wipeManagedAppRegistrationByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="0c191-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

> <span data-ttu-id="0c191-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0c191-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0c191-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0c191-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c191-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c191-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c191-107">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="0c191-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c191-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c191-108">Prerequisites</span></span>

<span data-ttu-id="0c191-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c191-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="0c191-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c191-111">Permission type</span></span>|<span data-ttu-id="0c191-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c191-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c191-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c191-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0c191-114">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="0c191-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="0c191-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c191-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0c191-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c191-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c191-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c191-117">Not supported.</span></span>|
|<span data-ttu-id="0c191-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c191-118">Application</span></span>|<span data-ttu-id="0c191-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c191-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c191-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c191-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="0c191-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c191-121">Request headers</span></span>

|<span data-ttu-id="0c191-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c191-122">Header</span></span>|<span data-ttu-id="0c191-123">Valor</span><span class="sxs-lookup"><span data-stu-id="0c191-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c191-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c191-124">Authorization</span></span>|<span data-ttu-id="0c191-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c191-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c191-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c191-126">Accept</span></span>|<span data-ttu-id="0c191-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0c191-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c191-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c191-128">Request body</span></span>

<span data-ttu-id="0c191-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0c191-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0c191-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="0c191-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0c191-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c191-131">Property</span></span>|<span data-ttu-id="0c191-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c191-132">Type</span></span>|<span data-ttu-id="0c191-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c191-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c191-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="0c191-134">deviceTag</span></span>|<span data-ttu-id="0c191-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c191-135">String</span></span>|<span data-ttu-id="0c191-136">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="0c191-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="0c191-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c191-137">Response</span></span>

<span data-ttu-id="0c191-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0c191-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0c191-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c191-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c191-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c191-140">Request</span></span>

<span data-ttu-id="0c191-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c191-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="0c191-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c191-142">Response</span></span>

<span data-ttu-id="0c191-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c191-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






