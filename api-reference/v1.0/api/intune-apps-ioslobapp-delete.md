---
title: Excluir iosLobApp
description: Exclui iosLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4547709a843d3ebfd79c327279ab55928d934347
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196228"
---
# <a name="delete-ioslobapp"></a><span data-ttu-id="6a49b-103">Excluir iosLobApp</span><span class="sxs-lookup"><span data-stu-id="6a49b-103">Delete iosLobApp</span></span>

> <span data-ttu-id="6a49b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a49b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a49b-105">Exclui [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a49b-105">Deletes a [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a49b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a49b-106">Prerequisites</span></span>
<span data-ttu-id="6a49b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6a49b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6a49b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a49b-109">Permission type</span></span>|<span data-ttu-id="6a49b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a49b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a49b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a49b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a49b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a49b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6a49b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a49b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a49b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a49b-114">Not supported.</span></span>|
|<span data-ttu-id="6a49b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a49b-115">Application</span></span>|<span data-ttu-id="6a49b-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a49b-116">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a49b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a49b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="6a49b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a49b-118">Request headers</span></span>
|<span data-ttu-id="6a49b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a49b-119">Header</span></span>|<span data-ttu-id="6a49b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6a49b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a49b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a49b-121">Authorization</span></span>|<span data-ttu-id="6a49b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a49b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a49b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a49b-123">Accept</span></span>|<span data-ttu-id="6a49b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6a49b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a49b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a49b-125">Request body</span></span>
<span data-ttu-id="6a49b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a49b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a49b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a49b-127">Response</span></span>
<span data-ttu-id="6a49b-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6a49b-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6a49b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a49b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a49b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a49b-130">Request</span></span>
<span data-ttu-id="6a49b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a49b-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="6a49b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a49b-132">Response</span></span>
<span data-ttu-id="6a49b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a49b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



