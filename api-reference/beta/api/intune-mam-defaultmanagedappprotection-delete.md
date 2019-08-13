---
title: Excluir defaultManagedAppProtection
description: Exclui defaultManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2709df125ddb1fa332ade1aa11c8353f767df422
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36354356"
---
# <a name="delete-defaultmanagedappprotection"></a><span data-ttu-id="f9921-103">Excluir defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="f9921-103">Delete defaultManagedAppProtection</span></span>

> <span data-ttu-id="f9921-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9921-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9921-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9921-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9921-106">Exclui [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f9921-106">Deletes a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9921-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9921-107">Prerequisites</span></span>
<span data-ttu-id="f9921-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9921-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9921-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9921-110">Permission type</span></span>|<span data-ttu-id="f9921-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9921-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9921-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9921-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9921-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9921-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f9921-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9921-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9921-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9921-115">Not supported.</span></span>|
|<span data-ttu-id="f9921-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9921-116">Application</span></span>|<span data-ttu-id="f9921-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9921-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9921-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9921-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="f9921-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9921-119">Request headers</span></span>
|<span data-ttu-id="f9921-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9921-120">Header</span></span>|<span data-ttu-id="f9921-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f9921-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9921-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9921-122">Authorization</span></span>|<span data-ttu-id="f9921-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9921-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9921-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9921-124">Accept</span></span>|<span data-ttu-id="f9921-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9921-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9921-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9921-126">Request body</span></span>
<span data-ttu-id="f9921-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9921-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9921-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9921-128">Response</span></span>
<span data-ttu-id="f9921-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f9921-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f9921-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9921-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9921-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9921-131">Request</span></span>
<span data-ttu-id="f9921-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9921-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="f9921-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9921-133">Response</span></span>
<span data-ttu-id="f9921-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9921-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






