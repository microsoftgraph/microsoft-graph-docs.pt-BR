---
title: Ação wipeManagedAppRegistrationsByDeviceTag
description: Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.
author: tfitzmac
ms.openlocfilehash: c08ba0bb670b2429cd97f7a23a8790ccc6c5c487
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318967"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="3b46f-103">Ação wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="3b46f-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="3b46f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3b46f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b46f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3b46f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b46f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3b46f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b46f-107">Emite uma operação de apagamento em um registro de aplicativo com uma marcação de dispositivo específica.</span><span class="sxs-lookup"><span data-stu-id="3b46f-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b46f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b46f-108">Prerequisites</span></span>

<span data-ttu-id="3b46f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b46f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b46f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b46f-111">Permission type</span></span>|<span data-ttu-id="3b46f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b46f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b46f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b46f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3b46f-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="3b46f-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3b46f-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b46f-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3b46f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b46f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b46f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b46f-117">Not supported.</span></span>|
|<span data-ttu-id="3b46f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b46f-118">Application</span></span>|<span data-ttu-id="3b46f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b46f-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b46f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b46f-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="3b46f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b46f-121">Request headers</span></span>

|<span data-ttu-id="3b46f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b46f-122">Header</span></span>|<span data-ttu-id="3b46f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3b46f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b46f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b46f-124">Authorization</span></span>|<span data-ttu-id="3b46f-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b46f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b46f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3b46f-126">Accept</span></span>|<span data-ttu-id="3b46f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3b46f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b46f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b46f-128">Request body</span></span>

<span data-ttu-id="3b46f-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3b46f-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3b46f-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3b46f-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3b46f-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b46f-131">Property</span></span>|<span data-ttu-id="3b46f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b46f-132">Type</span></span>|<span data-ttu-id="3b46f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b46f-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b46f-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="3b46f-134">deviceTag</span></span>|<span data-ttu-id="3b46f-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b46f-135">String</span></span>|<span data-ttu-id="3b46f-136">marca de dispositivo</span><span class="sxs-lookup"><span data-stu-id="3b46f-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="3b46f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b46f-137">Response</span></span>

<span data-ttu-id="3b46f-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3b46f-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3b46f-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b46f-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b46f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b46f-140">Request</span></span>

<span data-ttu-id="3b46f-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b46f-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="3b46f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b46f-142">Response</span></span>

<span data-ttu-id="3b46f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b46f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






