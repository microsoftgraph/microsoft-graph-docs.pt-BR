---
title: Excluir managedIOSStoreApp
description: Exclui managedIOSStoreApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 69c0b16fd9d1a012116290c89485d4a715a019e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516156"
---
# <a name="delete-managediosstoreapp"></a><span data-ttu-id="b272c-103">Excluir managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="b272c-103">Delete managedIOSStoreApp</span></span>

<span data-ttu-id="b272c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b272c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b272c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b272c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b272c-106">Exclui [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b272c-106">Deletes a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b272c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b272c-107">Prerequisites</span></span>
<span data-ttu-id="b272c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b272c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b272c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b272c-110">Permission type</span></span>|<span data-ttu-id="b272c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b272c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b272c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b272c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b272c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b272c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b272c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b272c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b272c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b272c-115">Not supported.</span></span>|
|<span data-ttu-id="b272c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b272c-116">Application</span></span>|<span data-ttu-id="b272c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b272c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b272c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b272c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b272c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b272c-119">Request headers</span></span>
|<span data-ttu-id="b272c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b272c-120">Header</span></span>|<span data-ttu-id="b272c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b272c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b272c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b272c-122">Authorization</span></span>|<span data-ttu-id="b272c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b272c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b272c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b272c-124">Accept</span></span>|<span data-ttu-id="b272c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b272c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b272c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b272c-126">Request body</span></span>
<span data-ttu-id="b272c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b272c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b272c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b272c-128">Response</span></span>
<span data-ttu-id="b272c-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b272c-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b272c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b272c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b272c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b272c-131">Request</span></span>
<span data-ttu-id="b272c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b272c-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="b272c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b272c-133">Response</span></span>
<span data-ttu-id="b272c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b272c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




