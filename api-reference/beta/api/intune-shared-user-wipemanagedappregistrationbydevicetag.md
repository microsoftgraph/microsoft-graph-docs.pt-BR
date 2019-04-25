---
title: Ação wipeManagedAppRegistrationByDeviceTag
description: Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 650ff602101cead593d39603beb0b361ac0421dc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526871"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="3373d-103">Ação wipeManagedAppRegistrationByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="3373d-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

> <span data-ttu-id="3373d-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3373d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3373d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3373d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3373d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3373d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3373d-107">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="3373d-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3373d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3373d-108">Prerequisites</span></span>

<span data-ttu-id="3373d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3373d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3373d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3373d-111">Permission type</span></span>|<span data-ttu-id="3373d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3373d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3373d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3373d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3373d-114">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="3373d-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3373d-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3373d-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3373d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3373d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3373d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3373d-117">Not supported.</span></span>|
|<span data-ttu-id="3373d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3373d-118">Application</span></span>|<span data-ttu-id="3373d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3373d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3373d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3373d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="3373d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3373d-121">Request headers</span></span>

|<span data-ttu-id="3373d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3373d-122">Header</span></span>|<span data-ttu-id="3373d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3373d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3373d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3373d-124">Authorization</span></span>|<span data-ttu-id="3373d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3373d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3373d-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3373d-126">Accept</span></span>|<span data-ttu-id="3373d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3373d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3373d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3373d-128">Request body</span></span>

<span data-ttu-id="3373d-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3373d-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3373d-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3373d-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3373d-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3373d-131">Property</span></span>|<span data-ttu-id="3373d-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="3373d-132">Type</span></span>|<span data-ttu-id="3373d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3373d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3373d-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="3373d-134">deviceTag</span></span>|<span data-ttu-id="3373d-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3373d-135">String</span></span>|<span data-ttu-id="3373d-136">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="3373d-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="3373d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3373d-137">Response</span></span>

<span data-ttu-id="3373d-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3373d-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3373d-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3373d-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="3373d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3373d-140">Request</span></span>

<span data-ttu-id="3373d-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3373d-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="3373d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3373d-142">Response</span></span>

<span data-ttu-id="3373d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3373d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






