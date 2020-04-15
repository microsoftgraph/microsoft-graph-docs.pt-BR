---
title: Excluir iosLobApp
description: Exclui iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6207ef40ec2c0af75e472a37aac7859f1b3ab05
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446537"
---
# <a name="delete-ioslobapp"></a><span data-ttu-id="f6411-103">Excluir iosLobApp</span><span class="sxs-lookup"><span data-stu-id="f6411-103">Delete iosLobApp</span></span>

<span data-ttu-id="f6411-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6411-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6411-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6411-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6411-106">Exclui [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6411-106">Deletes a [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6411-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f6411-107">Prerequisites</span></span>
<span data-ttu-id="f6411-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f6411-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f6411-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6411-110">Permission type</span></span>|<span data-ttu-id="f6411-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f6411-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6411-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6411-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6411-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6411-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f6411-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6411-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6411-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6411-115">Not supported.</span></span>|
|<span data-ttu-id="f6411-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6411-116">Application</span></span>|<span data-ttu-id="f6411-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6411-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6411-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6411-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f6411-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6411-119">Request headers</span></span>
|<span data-ttu-id="f6411-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6411-120">Header</span></span>|<span data-ttu-id="f6411-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f6411-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6411-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6411-122">Authorization</span></span>|<span data-ttu-id="f6411-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6411-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6411-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f6411-124">Accept</span></span>|<span data-ttu-id="f6411-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f6411-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6411-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6411-126">Request body</span></span>
<span data-ttu-id="f6411-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f6411-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6411-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6411-128">Response</span></span>
<span data-ttu-id="f6411-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f6411-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f6411-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6411-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6411-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6411-131">Request</span></span>
<span data-ttu-id="f6411-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6411-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="f6411-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6411-133">Response</span></span>
<span data-ttu-id="f6411-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6411-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






